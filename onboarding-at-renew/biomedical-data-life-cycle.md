---
description: Biomedical Data Life Cycle
icon: binary-lock
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

# Biomedical Data Life Cycle

<figure><img src="../.gitbook/assets/4 (2).png" alt=""><figcaption><p>Biomedical Data Life Cycle</p></figcaption></figure>

**Research Data Lifecycle** by [LMA Research Data Management Working Group](https://datamanagement.hms.harvard.edu/) is licensed under a [Creative Commons Attribution-NonCommercial 4.0 International License](http://creativecommons.org/licenses/by-nc/4.0/).  [Find all versions and materials for the lifecycle in Zenodo](https://doi.org/10.5281/zenodo.8075933).



Below is a **summary table of the Biomedical Research Data Lifecycle** with all major RDM stages. It aligns with institutional, ethical, and funder expectations relevant to **reNEW, UCPH**, and **European biomedical research** environments.

## 🔄 **Biomedical Research Data Lifecycle – Summary Table**

| **Stage**                      | **Purpose & Key Outputs**                                                                                                    | **Best Practices (UCPH · reNEW · EU Funders)**                                                                                                                                                  | **Common Risks & Mitigations**                                                                                                             |
| ------------------------------ | ---------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| **1. Plan & Design**           | Define what data will be collected/created and how it will be managed. Output: **Data Management Plan (DMP)**.               | - Develop DMPs early using tools like DMPonline- Align with UCPH/reNEW policies and FAIR principles- Include GDPR compliance and storage strategy (ERDA, REDCap)                                | Risk: Static DMP → Review regularlyRisk: Poor planning → Consult Data Steward early                                                        |
| **2. Collect & Create**        | Capture primary data via experiments, instruments, surveys, etc. Output: **Raw datasets**.                                   | - Use validated protocols and SOPs- Record metadata during acquisition- Use ELNs or structured lab notebooks- Standardize file naming and folder structure                                      | Risk: Incomplete metadata → Use templatesRisk: Data loss → Implement automated backups                                                     |
| **3. Analyze & Collaborate**   | Prepare raw data for analysis. Output: **Cleaned, structured datasets**.                                                     | - Document all transformations and preprocessing steps- Use workflow automation tools (Snakemake, Galaxy)- Maintain version control of data/code (Git)                                          | Risk: Lost provenance → Track data changesRisk: Overwriting raw data → Keep raw and processed separate                                     |
| **4. Evaluate & Archive**      | Analyze processed data to generate results and insights. Output: **Figures, models, and interpretations**.                   | - Ensure analysis is reproducible (scripts, containers)- Record software versions and parameters- Use version-controlled repositories (GitHub, GitLab)                                          | Risk: Irreproducible results → Document analysis pipelineRisk: Untraceable outputs → Link outputs to input data versions                   |
| **5. Share & Publish**         | Create documentation for internal use and future reuse. Output: **Metadata files, README, data dictionary**.                 | - Use controlled vocabularies and ontologies (e.g., HCO, MIAME)- Follow metadata standards (e.g., ISA-Tab)- Provide README and data dictionary files                                            | Risk: Unusable data → Require metadata before publicationRisk: Inconsistent formats → Use templates                                        |
| **6. Storage & Backup**        | Store data securely with backups. Output: **Redundant, secure data storage**.                                                | - Use UCPH-approved solutions (ERDA, REDCap, secure servers)- Implement access controls for sensitive data- Regularly test and monitor backup systems                                           | Risk: Data loss → Enforce automated backupsRisk: Unauthorized access → Use access control policies                                         |
| **7. Data Sharing & Access**   | Share data with collaborators, public, or under controlled access. Output: **Deposited datasets or shared links**.           | - Select appropriate repository (e.g., GEO, EGA, Zenodo)- Choose licenses (e.g., CC-BY, CC0)- Ensure data are de-identified if needed- Comply with consent agreements and GDPR                  | Risk: Breach of confidentiality → Use controlled access repositoriesRisk: Misuse → Apply proper licensing                                  |
| **8. Long-Term Preservation**  | Ensure data remains accessible, understandable, and usable in the future. Output: **Archived datasets with persistent IDs**. | - Deposit in domain or institutional repositories- Use open, non-proprietary formats- Assign persistent identifiers (DOIs, handles)- Document retention periods per funder/institutional policy | Risk: Bit rot or format obsolescence → Periodically review archiveRisk: Inaccessibility → Use repositories with long-term guarantees       |
| **9. Reuse & Reproducibility** | Enable others (and yourself) to reproduce findings or reuse data. Output: **Citable, verifiable data packages**.             | - Share data/code/methods openly when possible- Publish data papers or include detailed methods in manuscripts- Use open source software when possible                                          | Risk: Irreproducible science → Run internal replication testsRisk: Low visibility → Publish metadata-rich records and link to publications |

***

Would you like this in **Markdown**, **Word**, or **HTML table format** for direct integration into your GitBook or PDF newsletters?
