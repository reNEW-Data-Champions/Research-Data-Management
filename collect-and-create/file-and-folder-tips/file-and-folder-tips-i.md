---
description: Organizing Your Data
layout:
  width: wide
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
---

# 🟢 File and Folder  Structure Tips

## 1. Why Organize?

A data management workflow streamlines research data and processes to ensure understandability and reproducibility for those unfamiliar with the project. To achieve this objective, team members need clear, concise guidelines and tasks, responsibility for their work, and a means to share progress and feedback.

Four essential components of an effective data management workflow:

1. Consistent file organization and naming conventions facilitate easy navigation and comprehension of folder and file contents.
2. Code and data cleaning protocols and upload procedures enable team members to understand, verify, and collaborate on each other's work.
3. Transparent data management roles within the group to ensure file security, adherence to established procedures, and regulatory compliance.
4. A research group wiki that serves as a central hub for team members to share vital lab documents, such as lab notebooks, project updates, and published research data.

Motivation. Once you initiate data creation, collection, or manipulation, it can quickly become disorganized. To save time and avoid errors in the long run, you and your colleagues must establish a consistent approach to naming and structuring files and folders and incorporating documentation (or "metadata". Adds context to your data, enabling you and others to understand better and utilize it in the short, medium, and long term.

## 2. Collection & Creation Stage: Essentials for Research Groups

The collection and creation stage in the research data management lifecycle is critical, as it sets the foundation for the entire research process. The following elements should be addressed.

| Element                               | Guidance                                                                                                                                                                                                             |
| ------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Planning and preparation              | Develop a data management plan (DMP. outlining strategies, resources, and best practices for handling research data throughout the project. Define storage requirements, backup policies, and sharing strategies.    |
| Ethical considerations and compliance | Ensure collection/creation processes comply with ethical guidelines, institutional policies, and relevant regulations. Obtain informed consent where applicable, anonymize data, and adhere to data protection laws. |
| Data format and structure             | Determine suitable formats and structure for analysis compatibility, long-term preservation, and ease of sharing. Prefer standardized formats.                                                                       |
| Metadata and documentation            | Create metadata and documentation describing the data (origin, context, processing steps. to ensure understandability and reuse inside/outside the group.                                                            |
| Data quality and validation           | Implement quality procedures (validation checks, QC. to minimize errors and inconsistencies.                                                                                                                         |
| File organization and naming          | Establish clear, consistent folder structures and naming conventions to facilitate collaboration and simplify management across the project lifecycle.                                                               |
| Collaboration and communication       | Encourage open communication; hold regular meetings; define roles and responsibilities for data management tasks.                                                                                                    |

Outcome. By addressing these elements early, research groups lay a strong foundation for effective data management, high-quality research, and successful collaboration.

## 3. Documentation & Metadata: Steps and Best Practices

Organizing your data using documentation and metadata is essential for maintaining a clear understanding of your data and facilitating its discoverability and use by others. Implement the following:

* Choose appropriate metadata standards. Each standard is designed for specific data types or disciplines. Identify the most relevant standard for your data and use it as the basis for organizing and documenting it.
* Create a data dictionary. Describe each variable/data element (names, descriptions, data types, units, allowable values) so that others can interpret the data accurately.
* Document data collection and processing methods. Clearly describe procedures for collecting, processing, and analyzing your data for reproducibility and quality evaluation.
* Use consistent naming conventions. Adopt consistent conventions for files, folders, and variables to improve findability.
* Add descriptive file names and folder structures. Clear, informative names and a logical folder structure will help users quickly identify and access data.
* Include version control information. Track updates/revisions with change logs and version numbers (or use a VCS like Git/SVN..
* Store documentation and metadata with the data. Keep READMEs and metadata in the same location as the data (same folder or nearby README..
* Update documentation and metadata as needed. Review and update regularly, especially as data changes or new data are added.\


## 4. Naming and Organizing Files: Practical Guidance

### 4.1  Tips for Naming Files

* Descriptive file names: Indicate content and purpose; include project name, date, version number, and author initials where relevant.
* Consistent naming convention: Standardize across the project to prevent confusion and improve retrieval.
* Avoid special characters and spaces: Do not use @ # & \* or spaces; these may cause system/software issues.
* Appropriate file extensions: Always include the correct file extension so files open correctly.\


### 4.2  Tips for Organizing Files

* Logical folders: Group related files and reflect project hierarchy for quick access.
* Clear folder names: Accurately represent folder contents and purpose.
* Separate working vs final: Maintain separate locations for drafts/intermediate data vs published/cleaned outputs.
* Version control: To track changes, use version numbers (e.g., v1, v2, v3) or a VCSUse version numbers (e.g., v1, v2, v3. or a VCS to track changes.
* Keep documentation with data: Store data dictionaries, README, and metadata alongside datasets.
* Regular review: Periodically assess and reorganize to keep the structure effective and current.\


## 5. Organizing Your Files: Best Practices in Detail

Create a logical folder structure. Design a hierarchy that reflects the structure of your project or research (e.g., main folders for data, analysis, and reports, and subfolders for specific tasks or datasets).

1. Use clear and descriptive folder names. Make navigation intuitive by accurately naming each folder.
2. Adopt a consistent naming convention. Include project name, date, version number, author initials, or descriptors.
3. Avoid special characters and spaces. Use underscores \_ or hyphens - to separate words/elements when needed.
4. Use appropriate file extensions. Always include .txt, .csv, .docx, etc., as applicable.
5. Separate working files from final versions. Prevent confusion by keeping drafts and final versions apart.
6. Implement version control. Incorporate version numbers or use Git/SVN to manage iterations.
7. Keep documentation and metadata together with data. Provide context within the same folders.
8. Regularly review and update your file organization. Consolidate, rename, or reorganize as the project evolves.

## 6. Creating File Names: What to Consider

When creating a file name in the context of research data management, consider the following to ensure clarity, organization, and accessibility:

* Descriptiveness: Indicate content and purpose; include project name, subject, or a brief descriptor.
* Consistency: Follow a consistent convention across all files.
* Date and version: Include dates in YYYYMMDD format and a version number (e.g., v1, v2, v3..
* Author initials or identifier: Where multiple contributors exist, include initials or an identifier.
* Avoid special characters and spaces: Prefer \_ or - as separators.
* Use lowercase letters: Helps with case-sensitive file systems and cross-platform compatibility.
* File extension: Always include the correct extension (e.g., .txt, .csv, .docx..

Considering these aspects improves organization and accessibility, making collaboration and sharing easier.

## 7. Directory Structure & Naming Convention Example.

Efficient organization of research data in bioinformatics, genomics, and imaging within a biomedical research environment is vital for optimizing productivity, eliminating redundancy, and preserving data integrity. A systematic, carefully crafted directory structure and naming convention are paramount. The following guide establishes a coherent, well‑organized plan tailored for reNEW Copenhagen.

### 7.1  Root Directory

Create a root directory for your research project. Name it with a relevant and easily identifiable project name, for example:

#### **Jensen\_Skin\_Intestine\_Project/**

### 7.2  Subdirectories (Major Research Areas).

Within the root directory, create subdirectories for each major research area (bioinformatics, genomics, and imaging.. Use a clear, consistent naming convention, such as:

01\_Bioinformatics\_Data/

02\_Genomics\_Data/

03\_Imaging\_Data/

### 7.3  Research Themes

Within each research area, create subdirectories for different research themes or topics. For instance:

**01\_Bioinformatics\_Data/**

├── 01\_Protein\_Structure\_Analysis/

├── 02\_Gene\_Expression\_Analysis/

└── 03\_Metagenomics\_Analysis/

**02\_Genomics\_Data/**

├── 01\_Whole\_Genome\_Sequencing/

├── 02\_Transcriptomics/

└── 03\_Metagenomics/

**03\_Microscopy\_Data/**

├── 01\_Confocal\_microscopy/

├── 02\_Brightfield\_microscopy/

└── 03\_Light\_microscopy

### 7.4  Experiments and Timepoints

Create subdirectories for specific experiments or time points for each research theme or topic. Use a consistent naming convention that includes the date (YYYY-MM-DD). and a short description, e.g.:

**01\_Whole\_Genome\_Sequencing/**

├── 2023-04-01\_Mouse\_Genome\_Seq/

└── 2023-04-02\_Human\_Genome\_Seq/

### 7.5  Data Types and Formats (per Experiment/Timepoint.

Within each experiment/timepoint directory, create subdirectories for different data types or formats, for example:

**2023-04-01\_Mouse\_Genome\_Seq/**

├── 01\_Raw\_Data/

├── 02\_Processed\_Data/

└── 03\_Analysis\_Results/

### 7.6  Naming Files (Examples.

Use a consistent naming convention for all files, including details like the date, sample identifier, data type, and version (if applicable.:

**01\_Raw\_Data/**

├── 2023-04-01\_Mouse\_Genome\_Seq\_Sample01\_Raw\_v1.fastq

└── 2023-04-01\_Mouse\_Genome\_Seq\_Sample02\_Raw\_v1.fastq

**02\_Processed\_Data/**

├── 2023-04-01\_Mouse\_Genome\_Seq\_Sample01\_Processed\_v1.fasta

└── 2023-04-01\_Mouse\_Genome\_Seq\_Sample02\_Processed\_v1.fasta

**03\_Analysis\_Results/**

├── 2023-04-01\_Mouse\_Genome\_Seq\_Sample01\_Variants\_v1.vcf

└── 2023-04-01\_Mouse\_Genome\_Seq\_Sample02\_Variants\_v1.vcf

### 7.7  Metadata and Documentation (per Experiment/Timepoint.

Include a metadata file and a README with detailed information about the experiment, data types, formats, and processing steps. Suggested names:

Metadata\_2023-04-01\_Mouse\_Genome\_Seq.csv

README\_2023-04-01\_Mouse\_Genome\_Seq.txt

### 7.8 Backup and Version Control

Ensure regular backups and use version control (e.g., Git. to track script changes, analysis pipelines, and other relevant files.

Outcome. By adhering to these principles, you establish a systematic, user‑friendly framework for managing and storing research data at reNEW Copenhagen, streamlining access, facilitating entry, and enabling seamless collaboration across diverse teams.

## 8. Developing Your Naming Schema

* Be Consistent!  For related files, use the same elements (e.g., date, experiment number, version number) in the same order.
* Document It! Record your naming schemas in plain text in the README file with your data files.\


## 9. Best Practice — Detailed Examples

### 9.1 Length

* Guideline: Limit the file name to 32 characters (preferably less!..
* Example: 32CharactersLooksExactlyLikeThis.csv

### 9.2 Spaces, Periods & Special Characters

**Don’t use**

* spaces
* hyphens & dashes
* periods (except before file extension.
* other special characters (& , \* % # ; \* ! @$ ^ \~ ' { } \[ ] ? < >.\


**Use**

* underscores \_
* camelCase\


**Examples**

* NO name.date.txt
* NO name date v1.txt
* NO name-date-v1.txt (hyphen.
* NO name–date–v1.txt (en dash.
* NO name—date—v1.txt (em dash.
* NO name\&date.txt
* YES name\_date.txt
* YES Handout\_fileNaming\_20180215.pdf\


### 9.3 Dates

* Guideline: Use a consistent date format for sorting and easy file finding.
* Recommended: YYYYMMDD as a suitable default format.

### 9.4 Numbering

* Guideline: When using sequential numbering, use leading zeros to allow for multi‑digit versionsUse leading zeros to allow for multi‑digit versions when using sequential numbering. This keeps files in the intended order when sorting by name.\

* Sequences:



* For 1–10 → 01–10
* For 1–100 → 001–010–100\
  \

* Examples:
* NO ProjID\_v1.csv vs ProjID\_v12.csv
* YES ProjID\_v01.csv and ProjID\_v12.csv\


## 10. Example Directory Tree (Extended.

reNEW\_Group/

├── Genomics\_GNM/

│   ├── Project\_GNM\_ProjectName/

│   │   ├── Raw\_Data\_RD\_GNM\_ProjectName\_YYYYMMDD\_v1/

│   │   │   └── SampleName\_GNM\_RD\_ProjectName\_YYYYMMDD\_v1.fastq

│   │   ├── Processed\_Data\_PD\_GNM\_ProjectName\_YYYYMMDD\_v1/

│   │   │   └── SampleName\_GNM\_PD\_ProjectName\_YYYYMMDD\_v1.csv

│   │   └── Reports\_RPT\_GNM\_ProjectName\_YYYYMMDD\_v1.pdf

│   ├── Protocols\_PTCL\_GNM\_YYYYMMDD.pdf

│   ├── Tools\_TLC\_GNM\_YYYYMMDD/

│   └── Resources\_RSC\_GNM\_YYYYMMDD/

├── Microscopy\_MIC/

│   ├── Project\_MIC\_ProjectName/

│   │   ├── Raw\_Data\_RD\_MIC\_ProjectName\_YYYYMMDD\_v1/

│   │   │   └── SampleName\_MIC\_RD\_ProjectName\_YYYYMMDD\_v1.tiff

│   │   ├── Processed\_Data\_PD\_MIC\_ProjectName\_YYYYMMDD\_v1/

│   │   │   └── SampleName\_MIC\_PD\_ProjectName\_YYYYMMDD\_v1.jpg

│   │   └── Reports\_RPT\_MIC\_ProjectName\_YYYYMMDD\_v1.pdf

│   ├── Protocols\_PTCL\_MIC\_YYYYMMDD.pdf

│   ├── Tools\_TLC\_MIC\_YYYYMMDD/

│   └── Resources\_RSC\_MIC\_YYYYMMDD/

├── Tissue\_Culture\_TC/

│   ├── Project\_TC\_ProjectName/

│   │   ├── Raw\_Data\_RD\_TC\_ProjectName\_YYYYMMDD\_v1/

│   │   │   └── SampleName\_TC\_RD\_ProjectName\_YYYYMMDD\_v1.csv

│   │   ├── Processed\_Data\_PD\_TC\_ProjectName\_YYYYMMDD\_v1/

│   │   │   └── SampleName\_TC\_PD\_ProjectName\_YYYYMMDD\_v1.csv

│   │   └── Reports\_RPT\_TC\_ProjectName\_YYYYMMDD\_v1.pdf

│   ├── Protocols\_PTCL\_TC\_YYYYMMDD.pdf

│   ├── Tools\_TLC\_TC\_YYYYMMDD/

│   └── Resources\_RSC\_TC\_YYYYMMDD/

└── Flow\_Cytometry\_FC/

&#x20;   ├── Project\_FC\_ProjectName/

&#x20;   │   ├── Raw\_Data\_RD\_FC\_ProjectName\_YYYYMMDD\_v1/

&#x20;   │   │   └── SampleName\_FC\_RD\_ProjectName\_YYYYMMDD\_v1.fcs

&#x20;   │   ├── Processed\_Data\_PD\_FC\_ProjectName\_YYYYMMDD\_v1/

&#x20;   │   │   └── SampleName\_FC\_PD\_ProjectName\_YYYYMMDD\_v1.csv

&#x20;   │   └── Reports\_RPT\_FC\_ProjectName\_YYYYMMDD\_v1.pdf

&#x20;   ├── Protocols\_PTCL\_FC\_YYYYMMDD.pdf

&#x20;   ├── Tools\_TLC\_FC\_YYYYMMDD/

&#x20;   └── Resources\_RSC\_FC\_YYYYMMDD/\


Abbreviations (for quick reference):

* GNM: Genomics
* MIC: Microscopy
* TC: Tissue Culture
* FC: Flow Cytometry
* RD: Raw Data
* PD: Processed Data
* RPT: Reports
* PTCL: Protocols
* TLC: Tools
* RSC: Resources\


About file extensions (examples.:

* .fastq — standard format for genetic sequence data.
* .tiff or .jpg — standard image formats, commonly used in microscopy.
* .fcs — format for flow cytometry data.
* .csv — tabular data in a simple, widely used format.
* .pdf — documents such as reports or protocols.\


Readme practice. A README file can be maintained in each project directory and subdirectory to explain the content and record other essential details.

Key principle. Maintain consistency with the organization's naming convention and directory structure to ensure ease of navigation, data retrieval, and understanding among all team members.

***

## 11. Final Checklist (Actionable Summary).

* Establish DMP, storage, backup, and sharing policies.
* Confirm ethical compliance (consent, anonymization, data protection..
* Select standardized, analysis‑friendly formats.
* Create metadata, documentation, and a data dictionary.
* Define folder hierarchy and naming conventions.
* Implement QC/validation.
* Separate working vs final deliverables; version everything.
* Store documentation with data; keep READMEs current.
* Schedule periodic reviews and audits of the structure and naming.



\
