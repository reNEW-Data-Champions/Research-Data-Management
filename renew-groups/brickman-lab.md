# Brickman Lab

This section provides guidelines for effective research data management within our lab. By adopting these guidelines, we aim to improve data organization and naming conventions, leading to enhanced data governance and research efficiency. The guidelines include the following steps:

1. Adhere to folder structure and naming conventions for `Assays` and `Projects` folders.
2. Add relevant metadata to a `metadata.yml` in each folder
3. Create a database from metadata files in `Assays` and `Projects` folders.
4. Visualize database with a [Panel python app](https://panel.holoviz.org/).
5. `Projects` folders will be version controlled with Github and the [Brickman organization](https://github.com/brickmanlab).
6. `Projects` reports will be displayed under the [Brickman organization GitHub Pages](https://gbrickmanlab.github.io/).
7. `Projects` will be syncronized and archived in [Zenodo](https://zenodo.org/), which will give a DOI that can be used in a publication.
8. NGS `Assays` folder will be uploaded to GEO, with the information provided in the metadata file.
9. Create a Data Management Plan template that it is prefilled with repetitive information using [DMPonline](https://dmponline.deic.dk/)

### 1. Folder structure and organization <a href="#1-folder-structure-and-organization" id="1-folder-structure-and-organization"></a>

To ensure efficient data management, it is important to establish a consistent approach to organizing research data. We consider the following practices:

* Folder structure: we aim to a logical and intuitive folder structure that reflects the organization of research projects and experimental data. We use descriptive folder names to make it easy to locate and access specific data files.
* Subfolders: Use subfolders to further categorize data based on their contents, such as code notebooks, results, reports, etc. This helps to keep data organized and facilitates quick retrieval.
* File naming conventions: implement a standardized file naming convention to ensure consistency and clarity. Use descriptive names that include relevant information, such as type of plots, results tables, etc.

#### 1.1 Template engine <a href="#11-template-engine" id="11-template-engine"></a>

We are currently using a [cookiecutter](https://github.com/cookiecutter/cookiecutter) template to generate a [folder structure](https://github.com/brickmanlab/ngs-template). Use [cruft](https://github.com/cruft/cruft) when generating assay and project folders to allow us to validate and sync old templates with the latest version.

#### 1.2 Assay folder <a href="#12-assay-folder" id="12-assay-folder"></a>

For each NGS experiment there should be an `Assay` folder that will contain all experimental datasets (raw files and pipeline processed files). Inside `Assay` there will be subfolders named after a unique NGS ID and the date it was created:

**Assay ID code names**

* `CHIP`: ChIP-seq
* `RNA`: RNA-seq
* `ATAC`: ATAC-seq
* `SCR`: scRNA-seq
* `PROT`: Mass Spectrometry Assay
* `CAT`: Cut\&Tag
* `CAR`: Cut\&Run
* `RIME`: Rapid Immunoprecipitation Mass spectrometry of Endogenous proteins

For example `CHIP_20230101` is a ChIPseq assay made on 1st January 2023.

**Folder Structure**

```
CHIP_20230424
├── description.yaml
├── metadata.yaml
├── pipeline.md
├── processed
└── raw
   ├── .fastq.gz
   └── samplesheet.csv
```

* **description.yaml**: short and long descriptions of the assay in yaml format.
* **metadata.yaml**: metadata file for the assay describing different keys ([see below](broken-reference)).
* **pipeline.md**: description of the pipeline used to process raw data.
* **processed**: folder with results of the preprocessing pipeline. Contents depend on the pipeline used.
* **raw**: folder with the raw data.
* _.fastq.gz_:In the case of NGS assays, there should be fastq files.
* _samplesheet.csv_: file that contains metadata information for the samples. This file is used to run the nf-core pipelines. Ideally, it will also contain a column with info regarding the experimental variables and batches so it can be used for down stream analysis as well.

#### 1.3 Project folder <a href="#13-project-folder" id="13-project-folder"></a>

There should be another folder called `Projects` that will contain project information and data analysis.

A project may use one or more assays to answer a scientific question. This should be, for example, all the data analysis related to a publication.

The project folder should be named after a unique identifier, such as:

`<Project-ID>` should be the surname of the owner of the project folder and the publication year, e.g. `JARH_etal_20230101`.

**Folder structure**

```
<Project-ID>_20230424
├── data
│  ├── assays
│  ├── external
│  └── processed
├── documents
├── notebooks
├── README.md
├── reports
│  └── figures
├── requirements.txt
├── results
└── scripts
```

* **data**: folder that contains symlinks or shortcuts to where the data is, avoiding copying and modification of original files.
* **documents**: folder containing word documents, slides or pdfs related to the project, such as explanations of the data or project, papers, etc.
* **notebooks**: folder containing Jupyter, R markdown or Quarto notebooks with the actual data analysis. Using annotated notebooks is ideal for reproducibility and readability purposes. Notebooks should be labeled numerically in order they were created e.g. `00_preprocessing`
* **README.md**: detailed description of the project in markdown format.
* **reports**: notebooks rendered as html/docx/pdf versions, ideal for sharing with colleagues and also as a formal report of the data analysis procedure.
* _figures_: figures produced upon rendering notebooks. The figures will be saved under a subfolder named after the notebook that created them. This is for provenance purposes so we know which notebook created which figures.
* **results**: results from the data analysis, such as tables with differentially expressed genes, enrichment results, etc. These results should be saved under a subfolder named after the notebook that created them. This is for provenance purposes so we know which notebook created which results.
* **scripts**: folder containing helper scripts needed to run data analysis or reproduce the work of the folder

#### 1.4 Synchronization with DanGPU server <a href="#14-synchronization-with-dangpu-server" id="14-synchronization-with-dangpu-server"></a>

We will have to setup a cron job to perform one-way sync between the `/projects` folder and `NGS_data` folder. All the analysis will be done on danGPU server, with **no exceptions**!

After project is done and published, it will be moved to `NGS_data`.

#### 1.5 General naming conventions and more info <a href="#15-general-naming-conventions-and-more-info" id="15-general-naming-conventions-and-more-info"></a>

* date format: `YYYYMMDD`

[Transcriptomics metadata standards and fields](https://faircookbook.elixir-europe.org/content/recipes/interoperability/transcriptomics-metadata.html#analysis-metadata)

More info on naming conventions for different types of files and analysis is in development.

Accurate documentation and metadata play a crucial role in facilitating data discovery and interpretation. Consider the following guidelines:

* Metadata capture: Record essential metadata for each dataset, including type of experiment, date, organisms, etc. This information provides context and helps others understand and reuse the data effectively.
* Readme files: Create readme files for each project or dataset. These files should provide a brief overview of the project, list the files and their descriptions, and explain any specific instructions or dependencies required for data analysis.

#### 2.1 Assay metadata fields <a href="#21-assay-metadata-fields" id="21-assay-metadata-fields"></a>

| Metadata field      | Definition                                                                                                     | Format                     | ontology                                       | example                         |
| ------------------- | -------------------------------------------------------------------------------------------------------------- | -------------------------- | ---------------------------------------------- | ------------------------------- |
| assay\_ID           | Identifier for the assay that is at least unique within the project                                            | \<code\_name>\_YYYYMMDD    | nan                                            | CHIP\_20200101                  |
| assay\_type         | The type of experiment performed, eg ATAC-seq or seqFISH                                                       | nan                        | ontology field- e.g. EFO or OBI                | ChIPseq                         |
| assay\_subtype      | More specific type or assay like bulk nascent RNAseq or single cell ATACseq                                    | nan                        | ontology field- e.g. EFO or OBI                | bulk ChIPseq                    |
| owner               | Owner of the assay (who made the experiment?).                                                                 | \<First Name> \<Last Name> | nan                                            | Jose Romero                     |
| platform            | The type of instrument used to perform the assay, eg Illumina HiSeq 4000 or Fluidigm C1 microfluidics platform | nan                        | ontology field- e.g. EFO or OBI                | Illumina                        |
| extraction\_method  | Technique used to extract the nucleic acid from the cell                                                       | nan                        | ontology field- e.g. EFO or OBI                | nan                             |
| library\_method     | Technique used to amplify a cDNA library                                                                       | nan                        | ontology field- e.g. EFO or OBI                | nan                             |
| external accessions | Accession numbers from external resources to which assay or protocol information was submitted                 | nan                        | eg protocols.io, AE, GEO accession number, etc | GSEXXXXX                        |
| codename            | Internal code name for easy identification (like a keyword)                                                    | nan                        | nan                                            | Oct4\_ChIP                      |
| date                | Date of assay creation                                                                                         | YYYYMMDD                   | nan                                            | 20200101                        |
| nsamples            | Number of samples analyzed in this assay                                                                       | \<integer>                 | nan                                            | 9                               |
| is\_paired          | Paired fastq files or not                                                                                      | \<single OR paired>        | nan                                            | single                          |
| pipeline            | Pipeline used to process data                                                                                  | nan                        | nan                                            | nf-core/chipseq                 |
| strandedness        | The strandedness of the cDNA library                                                                           | <+ OR - OR \*>             | nan                                            | \*                              |
| processed\_by       | Who processed the data                                                                                         | \<First Name> \<Last Name> | nan                                            | Sarah Lundregan                 |
| organism            | Organism origin                                                                                                | \<Genus species>           | nan                                            | Mus musculus                    |
| origin              | If it is internal or external data                                                                             | \<internal OR external>    | nan                                            | nan                             |
| path                | Path to files                                                                                                  | \</path/to/file>           | nan                                            | nan                             |
| short\_desc         | Short description of the assay                                                                                 | plain text                 | nan                                            | Oct4 ChIP after pERK activation |

#### 2.2 Project metadata fields <a href="#22-project-metadata-fields" id="22-project-metadata-fields"></a>

In development.

### 3. Data management catalogue <a href="#3-data-management-catalogue" id="3-data-management-catalogue"></a>

@SLundregan is in the process of building a prototype for `Assay`, using the metadata contained in all `description.yml` and `metadata.yml` files in the assay folder. This will be in the form of an SQLite database that that is easily updatable by running a helper script.

### 4. Database browser <a href="#4-database-browser" id="4-database-browser"></a>

@SLundregan is also working on a browsable database using [Panel python app](https://panel.holoviz.org/). The app will display the latest version of the SQLite database. Clicking on an item from the database will open a tab containing all available metadata for the assay.

Also, it would be nice if you can create an `Assay` folder directly from there, making it easy to fill up the info for the metadata and GEO submission ([see below](broken-reference))

In the future, you could ideally visualize an analysed single cell RNAseq dataset by opening [Cirrocumulus](https://cirrocumulus.readthedocs.io/en/latest/) session.

### 5. `Projects` version control <a href="#5-projects-version-control" id="5-projects-version-control"></a>

All projects should be version controlled using GitHub under the [Brickman organization](https://github.com/brickmanlab/). After creating a cookiecutter template, initiate a git repository on the folder. The Git repository can stay private until it is ready for publication.

### 6. `Projects` GitHub pages <a href="#6-projects-github-pages" id="6-projects-github-pages"></a>

Using GitHub pages, it is possible to display your data analyses (or anything related to the project) inside the `Projects` folder so that they are open to the public in a html format. This is great for transparency and reproducibility purposes. This can be done after the paper has been made public (it is not possible to do with a private repository without paying).

**Info on how this is done should be put here**

### 7. `Project` archiving in Zenodo <a href="#7-project-archiving-in-zenodo" id="7-project-archiving-in-zenodo"></a>

Before submitting, link the repository to [Zenodo](https://zenodo.org/) and then create a Git release. This release will be caught by Zenodo and will give you a DOI that you can submit along the manuscript.

### 8. Data upload to GEO <a href="#8-data-upload-to-geo" id="8-data-upload-to-geo"></a>

The raw data from NGS experiments will be uploaded to the [Gene Expression Omnibus (GEO)](https://www.ncbi.nlm.nih.gov/geo/). Whenever a new Assay folder is created, the data owner must fill up the required documentation and information needed to make the GEO submission as smooth as possible.

### 9. Create a Data Management Plan <a href="#9-create-a-data-management-plan" id="9-create-a-data-management-plan"></a>

We are currently working on a DMP template that it is prefilled with repetitive information using [DMPonline](https://dmponline.deic.dk/) and the KU guidelines. This template will contain all the necessary information regarding common practices that we will use, the repositories we use for NGS, etc etc.

**more info on what is a DMP and how to use it**

***

Last update: June 8, 2023\
Created: May 18, 2023
