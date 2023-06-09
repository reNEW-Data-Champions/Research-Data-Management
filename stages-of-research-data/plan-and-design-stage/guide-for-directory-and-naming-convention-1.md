---
description: Document
---

# Guide for Directory and Naming Convention

Efficient organization of research data in bioinformatics, genomics, and imaging within a biomedical research environment is vital for optimizing productivity, eliminating redundancy, and preserving data integrity. A systematic and carefully crafted directory structure and naming convention system are paramount to accomplish this. The following directory structure and naming convention guide aim to establish a coherent and well-organized plan explicitly tailored for reNEW Copenhagen's research endeavors.

### 1. Root Directory:

Create a root directory for your research project. Name it with a relevant and easily identifiable project name, for example,

&#x20;"Jensen\_Skin\_Intestine\_Project."

### 2. Subdirectories:

Within the root directory, create subdirectories for each major research area (bioinformatics, genomics, and imaging). Use a clear, consistent naming convention, such as:

* 01\_Bioinformatics\_Data
* 02\_Genomics\_Data
* 03\_Imaging\_Data

### 3. Research Themes:

Within each research area, create subdirectories for different research themes or topics. For instance:

#### 01\_Bioinformatics\_Data:

* 01\_Protein\_Structure\_Analysis
* 02\_Gene\_Expression\_Analysis
* 03\_Metagenomics\_Analysis

#### 02\_Genomics\_Data:

* 01\_Whole\_Genome\_Sequencing
* 02\_Transcriptomics
* 03\_Metagenomics

#### 03\_Microscopy\_Data:

* 01\_Confocal\_microscopy:
* 02\_Brightfield\_microscopy
* 03\_Light\_microscopy

### 4. Experiments and Timepoints:

Create subdirectories for specific experiments or time points for each research theme or topic. Use a consistent naming convention that includes the date (YYYY-MM-DD) and a short description:

#### 01\_Whole\_Genome\_Sequencing:

* 2023-04-01\_Mouse\_Genome\_Seq
* 2023-04-02\_Human\_Genome\_Seq

### 5. Data Types and Formats:

Create subdirectories for different data types or formats within each experiment or timepoint directory. Examples:

#### 2023-04-01\_Mouse\_Genome\_Seq:

* 01\_Raw\_Data
* 02\_Processed\_Data
* 03\_Analysis\_Results

### 6. Naming Files:

Use a consistent naming convention for all files, including details like the date, sample identifier, data type, and version (if applicable).

Examples:

#### 01\_Raw\_Data:

* 2023-04-01\_Mouse\_Genome\_Seq\_Sample01\_Raw\_v1.fastq
* 2023-04-01\_Mouse\_Genome\_Seq\_Sample02\_Raw\_v1.fastq

#### &#x20;02\_Processed\_Data:

* 2023-04-01\_Mouse\_Genome\_Seq\_Sample01\_Processed\_v1.fasta
* 2023-04-01\_Mouse\_Genome\_Seq\_Sample02\_Processed\_v1.fasta

#### &#x20;03\_Analysis\_Results:

* 2023-04-01\_Mouse\_Genome\_Seq\_Sample01\_Variants\_v1.vcf
* 2023-04-01\_Mouse\_Genome\_Seq\_Sample02\_Variants\_v1.vcf

### &#x20;7. Metadata and Documentation:

Include a metadata file and a README file in each experiment or timepoint directory, with detailed information about the experiment, data types, formats, and processing steps.

Name these files:&#x20;

* Metadata\_2023-04-01\_Mouse\_Genome\_Seq.csv
* README\_2023-04-01\_Mouse\_Genome\_Seq.txt

### 8. Backup and Version Control:

Ensure regular data backups and use a version control system (e.g., Git) to track script changes, analysis pipelines, and other relevant files.

&#x20;

By adhering to the principles outlined in this directory structure and naming convention guide, you can establish a systematic, user-friendly framework for managing and storing research data at reNEW Copenhagen, streamlining access to crucial information and facilitating entry and facilitating entry and facilitating seamless collaboration across diverse research teams.
