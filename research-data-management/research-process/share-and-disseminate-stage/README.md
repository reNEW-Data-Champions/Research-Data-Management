---
description: Share & Publish Stage
icon: '5'
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

# Share & Disseminate Stage

<figure><img src="../../../.gitbook/assets/Share and Disseminate.jpg" alt=""><figcaption><p>Share &#x26; Publish Stage</p></figcaption></figure>

## Share & Disseminate Stage — Detailed Summary

| **Category**                               | **Details & Best Practices (UCPH · reNEW · EU funders)**                                                                                                                                                                                                                                                                                                                                     |
| ------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Stage Purpose**                          | Make research outputs **discoverable, accessible, and reusable** in line with **FAIR** and Open Science expectations; enable verification, reuse, and impact tracking.                                                                                                                                                                                                                       |
| **Drivers & Policies**                     | **Journals:** data availability statements and links to repositories.**EU funders (e.g., Horizon Europe/ERC):** require open access to publications and **responsible sharing of underlying data** when possible; justify restrictions.**UCPH/reNEW:** align with institutional RDM and Open Science guidance.                                                                               |
| **When to Share (Timing/Triggers)**        | **Pre‑publication** (preprints) when appropriate; **upon journal acceptance** (common); **project milestones/close**; **funder‑mandated timelines**; whenever a dataset is sufficiently curated to be reused.                                                                                                                                                                                |
| **What to Share (Scope)**                  | **Data:** underlying datasets that support figures/tables/claims; derived datasets where raw data cannot be shared.**Code & Workflows:** scripts, notebooks, containers, pipelines, environment files.**Documentation:** README, data dictionary, methodology, provenance (who/what/when/how).                                                                                               |
| **Where to Deposit (Repositories)**        | **Discipline‑specific:** GEO, PRIDE, ENA, ArrayExpress, PANGAEA, etc.**Generalist:** Zenodo, Figshare, Dataverse.**Institutional/National:** UCPH/ERDA or approved national services.Choose a repository that issues **PIDs (DOIs)**, supports **metadata indexing**, and offers **access controls** for sensitive data.                                                                     |
| **How to Cite & Identify (PIDs)**          | **Datasets:** DOI (preferably DataCite).**Publications:** DOI.**People:** ORCID iDs in author/creator fields.**Affiliations:** ROR IDs for institutions (e.g., UCPH/reNEW).**Projects/Grants:** include grant numbers in metadata.                                                                                                                                                           |
| **Metadata & Documentation (Minimum Set)** | **Descriptive metadata:** title, creators (with ORCID), abstract, keywords/subjects, funder, grant, affiliation (ROR), DOI.**Technical metadata:** file formats, units, instruments/platforms, software versions, parameters.**Provenance:** methods, processing steps, links to code/workflows.**README + Data Dictionary:** variable names, definitions, value ranges, missing‑data codes. |
| **File Formats (Interoperability)**        | Prefer **open, non‑proprietary** formats where feasible: **CSV/TSV**, **JSON**, **TIFF**, **HDF5**, **NetCDF**, **PNG**, **TXT**, **XML**; include conversion notes when proprietary formats are unavoidable.                                                                                                                                                                                |
| **Licensing & Terms of Use**               | Assign an appropriate **open data license** (e.g., **CC BY 4.0**, **CC0**, **ODC‑BY/ODbL**) when possible; for code use **OSI‑approved** licenses (MIT, Apache‑2.0, GPL). Clearly state **reuse conditions** in metadata and README.                                                                                                                                                         |
| **Sensitive/Restricted Data (GDPR)**       | If data contain **personal/clinical/confidential** information, share via **controlled access**: keep **metadata public** (to enable discovery) and provide **access request procedures** (DUA/ethics approvals). Use **pseudonymization/anonymization**, aggregation, or **synthetic data** where appropriate.                                                                              |
| **Data Availability Statement (DAS)**      | Every publication should include a **DAS** with: repository name + **persistent link/DOI**, **access conditions** (open, embargoed, controlled), license, and contact/steward info for requests.                                                                                                                                                                                             |
| **Quality Control Before Release**         | Validate files and **checksums** (e.g., SHA‑256); verify **completeness** vs. figures/tables; run **schema/format checks**; confirm **metadata fields** and **PID links**; ensure README/data dictionary are present; test **download and openability**.                                                                                                                                     |
| **Roles & Responsibilities**               | **PI:** approves scope and timing; ensures compliance.**Data Steward/Manager:** curates metadata, selects repository, prepares DUA/embargo, validates QC checklist.**Researchers/Analysts:** finalize datasets, code, and documentation; respond to reviewer queries.**IT/Support:** storage, transfer, and repository onboarding.                                                           |
| **Access Models**                          | **Open:** immediate public access.**Embargoed:** released after a defined period (journal/funder policy).**Controlled:** access via application/DUA/ethics approval. Document rationale and procedures.                                                                                                                                                                                      |
| **Records to Keep (Audit Trail)**          | Copies of **submitted datasets**, exact **metadata exports**, **DAS text**, license files, **reviewer exchanges**, approval emails, and repository **receipt/DOI assignment**.                                                                                                                                                                                                               |
| **Post‑Publication Maintenance**           | Versioning policy (e.g., **v1.0 → v1.1** for minor fixes); maintain **changelogs**; update links if article moves; respond to **data access requests**; plan for **long‑term preservation** or migration to archival tiers.                                                                                                                                                                  |
| **Benefits & Impact**                      | Increases **citations and visibility**, supports **reproducibility**, meets **UCPH/reNEW/EU** mandates, enables **societal and scientific reuse**, and strengthens grant/reporting narratives.                                                                                                                                                                                               |
| **Common Risks & Mitigations**             | **Risk:** sharing incomplete/undocumented data → **Mitigation:** enforce QC checklist & steward review.**Risk:** GDPR breach → **Mitigation:** de‑identify, controlled access, DUA, steward sign‑off.**Risk:** link rot → **Mitigation:** use DOIs, archive code with releases.                                                                                                              |

