---
description: Data Storage, Collaboration, and HPC Resources at reNEW, UCPH
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

# 🟤 Data Storage

## **Data Storage, Collaboration, and HPC Resources at UCPH** <a href="#qkgro3bbmczl" id="qkgro3bbmczl"></a>

## **Introduction** <a href="#qqgtgcfy7mzs" id="qqgtgcfy7mzs"></a>

Biomedical research at **reNEW – The Novo Nordisk Foundation Center for Stem Cell Medicine, UCPH,** is data-intensive, often involving large imaging datasets, sensitive patient information, and complex analyses. Effective **Research Data Management (RDM)** ensures data security, meets legal and ethical obligations (including GDPR compliance), and supports high-quality, reproducible science.

A critical component of RDM is **data storage management** throughout the **Research Data Lifecycle**. Each stage—from planning to archiving—requires careful consideration of storage infrastructure, data privacy, security protocols, and collaboration needs, especially in projects that involve personal data or multi-institutional teams.

This guide provides an overview of best practices and the University of Copenhagen (UCPH) facilities supporting data storage, sharing, and high-performance computing (HPC) tailored to the needs of biomedical researchers at reNEW.

## **UCPH Data Storage and Collaboration Solutions** <a href="#xljg3abcaty3" id="xljg3abcaty3"></a>

Below is a summary of UCPH facilities suited to various data types and collaboration needs:

### **Personal Drive** <a href="#id-5666yciottu4" id="id-5666yciottu4"></a>

* For individual use ([Windows](https://kunet.ku.dk/work-areas/research/data/facilities-for-data-storage-and-sharing-in-active-projects/Pages/default.aspx#collapseMSOZoneCell_WebPartWPQ8)/[Linux](https://kunet.ku.dk/work-areas/research/data/facilities-for-data-storage-and-sharing-in-active-projects/Pages/default.aspx#collapseMSOZoneCell_WebPartWPQ14))
* Suitable for small amounts of non-sensitive research data
* Not designed for sharing with collaborators

### **Shared Network Drive -** [**Windows**](https://kunet.ku.dk/employee-guide/Pages/IT/Network-drives.aspx?searchHitHighlight=network%20drives) **/**[ **Linux**](https://kunet.ku.dk/work-areas/research/data/facilities-for-data-storage-and-sharing-in-active-projects/Pages/default.aspx#collapseMSOZoneCell_WebPartWPQ14) <a href="#yez794mg1jih" id="yez794mg1jih"></a>

* For collaboration among UCPH employees
* Ideal for research groups needing shared access
* Not suitable for storing sensitive or personal data

### **S-Drive (**[**Shared Drive for Sensitive Data**](https://kunet.ku.dk/employee-guide/Pages/IT/S-drive.aspx)**)** <a href="#p5saddrfee6g" id="p5saddrfee6g"></a>

* Designed for sharing sensitive data among designated UCPH users
* Complies with GDPR
* Suitable for storing and sharing confidential or personal data internally

### **Microsoft** [**OneDrive**](https://kunet.ku.dk/work-areas/research/data/facilities-for-data-storage-and-sharing-in-active-projects/Pages/default.aspx#collapseMSOZoneCell_WebPartWPQ7) **for Business** <a href="#r7y49423ku70" id="r7y49423ku70"></a>

* Cloud storage meeting UCPH security standards for **non-sensitive data**
* Up to 5TB for sharing with colleagues and external partners
* Covered by a data processing agreement with Microsoft
* Recommended cloud solution (note: Dropbox and other providers do _not_ have such agreements with UCPH)

### [**ERDA**](https://www.erda.dk/) **(Electronic Research Data Archive)** <a href="#stiawi2y2sdj" id="stiawi2y2sdj"></a>

* Managed by the HPC Center, Faculty of Science
* Centralized storage, archiving, and synchronization service
* Ideal for non-sensitive research data

### **Sensitive Information Facility (**[**SIF**](https://sif.ku.dk/)**)** <a href="#id-8zxbemagixhj" id="id-8zxbemagixhj"></a>

* For storing and sharing **sensitive information**, including personal data
* Enables secure sharing with UCPH and external partners
* Requires GDPR compliance and pre-approval
* Currently provided by the SCIENCE HPC Center; expansion to all UCPH researchers under consideration.

#### [**DATA DOI**](https://kunet.ku.dk/work-areas/research/data/data-sharing/data-doi) **Service** <a href="#erx8w887rs0p" id="erx8w887rs0p"></a>

* Built on ERDA
* Data sharing is open to all UCPH employees.
* Facilitates assigning DOIs to datasets for findable, citable research outputs

## **UCPH Policy for Research Data Management** <a href="#rdslyufadkgf" id="rdslyufadkgf"></a>

&#x20;[**UCPH Policy for Research Data Management**](https://kunet.ku.dk/work-areas/research/data/Documents/UCPHPolicyforResearchDataManagement2022-EN.pdf) emphasizes:

* Choosing an appropriate, secure infrastructure
* Supporting collaboration while ensuring compliance with information security policies and legal requirements
* Protecting personal data in line with GDPR\


Researchers at **reNEW** must carefully select solutions that meet their data sensitivity and collaboration needs while upholding UCPH policies.

## **High-Performance Computing (HPC) for Biomedical Research** <a href="#sguiafl883to" id="sguiafl883to"></a>

Biomedical research at reNEW often involves large-scale imaging analyses, computational modeling, and multi-omics integration that require **HPC resources**. UCPH offers access to both local and national HPC systems tailored to diverse research needs:

#### **Key National HPC Systems Available to UCPH Researchers** <a href="#id-6gqr7s78v0n" id="id-6gqr7s78v0n"></a>

### **Type 1 – Interactive HPC**

* Focus on interactivity and easy user access
* Includes **YouGene Cluster** hosted at UCPH (via UCloud)
* Supports iterative data exploration and analysis

### **Type 2 – Throughput HPC**

* Optimized for high-volume data processing
* Systems include **Computerome 2.0**, **GenomeDK**, and **Sophia.**
* Suitable for large-scale, batch analyses

### **Type 3 – Large Memory HPC**

* Designed for workloads needing large, globally addressable memory
* Hosted at UCPH
* Ideal for complex, memory-intensive biomedical simulations

### **Type 5 – LUMI Capability HPC**

* Pan-European pre-exascale system
* Located in Finland (EuroHPC initiative)
* Suitable for cutting-edge, large-scale computational needs

## <mark style="color:red;">**Special Note: DAN HPC at reNEW**</mark> <a href="#id-3t2i2s6xpb7x" id="id-3t2i2s6xpb7x"></a>

* Owned by DanStem/reNEW, SUND, CGEN/ICMM, CPR at SUND, co-admin with KU
* Shared CPU server for Genomics Data Analysis
* Specialized GPU node for **image data analysis**
* Connects large datasets stored on KU-IT storage for advanced computation
* See[ DAN System User Guide](https://sgn102.pages.ku.dk/a-not-long-tour-of-dangpu/) for more information

### **Access and Support** <a href="#wids8ul9700p" id="wids8ul9700p"></a>

* **UCloud** provides a user-friendly interface for accessing many of these HPC resources, with guidance and application processes streamlined for researchers.
* Support is available via UCPH IT and the Faculty of Science HPC Center.\
