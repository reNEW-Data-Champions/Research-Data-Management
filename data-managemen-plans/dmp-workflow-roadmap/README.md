---
description: DMP Workflow Roadmap
icon: e
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

# DMP Workflow Roadmap

DMP Workflow Roadmap

<table data-header-hidden><thead><tr><th width="109"></th><th width="196"></th><th width="298"></th><th></th></tr></thead><tbody><tr><td><strong>Stage</strong></td><td><strong>Goal</strong></td><td><strong>Recommended Tools / Resources</strong></td><td><strong>Notes / Examples</strong></td></tr><tr><td><strong>1. Plan</strong></td><td>Define how data will be managed before collection begins</td><td><strong>DMP Tools</strong>: DMPonline, DMPTool, Argos <strong>Policies</strong>: UCPH Research Data Policy, Horizon Europe DMP guidelines <strong>Identifiers</strong>: ORCID, ROR</td><td>Create a <strong>Data Management Plan (DMP)</strong> that describes data formats, metadata standards, storage, access control, and sharing strategy. Ensure alignment with <strong>FAIR Principles</strong> and funder mandates.</td></tr><tr><td><strong>2. Collect</strong></td><td>Acquire raw experimental data with proper structure &#x26; metadata</td><td><strong>Acquisition tools</strong>: Microscope vendor software + <strong>Bio-Formats</strong> for conversion <strong>Metadata standards</strong>: OME (bioimaging), MIAME (microarrays), MIABIS (biobanking), REMBI (bioimaging metadata)</td><td>Capture <strong>primary metadata at the point of collection</strong> (instrument type, conditions, sample info). Use controlled vocabularies/ontologies (e.g., OBO Foundry, EDAM).</td></tr><tr><td><strong>3. Store</strong></td><td>Ensure secure storage, versioning, and metadata capture during the project</td><td><strong>Institutional storage</strong>: OMERO (images), ERDA (UCPH), Dataverse, CKAN <strong>File formats</strong>: OME-TIFF, OME-Zarr, HDF5 <strong>ELNs</strong>: eLabFTW, Labguru</td><td>Store data in <strong>open formats</strong> with metadata. Use <strong>OME-Zarr</strong> for scalable N-D imaging. Document workflows in <strong>ELN systems</strong>. Maintain <strong>access control</strong> and backups.</td></tr><tr><td><strong>4. Publish</strong></td><td>Deposit datasets in repositories with persistent identifiers</td><td><strong>Repositories</strong>: BioImage Archive, IDR, EMPIAR (bioimaging); GEO, PRIDE, ENA (omics); Zenodo, Figshare (general OA) <strong>Persistent IDs</strong>: DOIs via DataCite/CrossRef</td><td>Deposit data in <strong>trusted repositories</strong> to comply with FAIR and Open Access mandates. Datasets receive <strong>DOIs</strong> for citation and linking to publications.</td></tr><tr><td><strong>5. Share</strong></td><td>Make data discoverable and accessible for the community</td><td><strong>Registries</strong>: FAIRsharing.org, re3data, OpenAIRE <strong>Policy frameworks</strong>: EOSC, GO FAIR, RDA, CODATA</td><td>Use <strong>metadata-rich records</strong> so data can be indexed in registries. Share under licenses (CC-BY, CC0) unless restricted. FAIR allows controlled access (e.g., dbGaP for genomic data).</td></tr><tr><td><strong>6. Reuse</strong></td><td>Enable reproducibility, secondary analysis, and integration</td><td><strong>Tools</strong>: Fiji, napari, QuPath, ilastik, 3D Slicer, Galaxy Imaging <strong>Citation systems</strong>: ORCID (authors), ROR (institutions), RRID (resources) <strong>Impact tracking</strong>: Altmetric, OpenAlex</td><td>Reuse is enabled by <strong>machine-actionable metadata</strong> and open formats. Reused data should be <strong>cited properly</strong> (dataset DOI). Adoption tracked via citations, reanalysis, or policy uptake.</td></tr></tbody></table>

***

## Key Insights for Life Sciences & Bioimaging

* **Planning & metadata** are the foundations of FAIR. Without capturing metadata at collection, downstream FAIRification is much harder.
* **Bioimaging-specific standards**: OME-TIFF/OME-Zarr for formats, REMBI for metadata.
* **Infrastructure integration**: Use **OMERO** for lab-scale storage and management and **BioImage Archive / IDR / EMPIAR** for long-term FAIR publication.
* **Reuse** is maximized when datasets are linked across identifiers: **dataset DOI ↔ publication DOI ↔ ORCID ↔ ROR ↔ RRID**.
* **FAIR ≠ Open**: Controlled-access data can still be FAIR if metadata is discoverable.
