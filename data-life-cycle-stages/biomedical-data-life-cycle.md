---
description: Biomedical Data Life Cycle
icon: '0'
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

<p align="center"><strong>(Biomedical) Research Data Lifecycle</strong> by <a href="https://datamanagement.hms.harvard.edu/">LMA Research Data Management Working Group</a> is licensed under a <a href="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial 4.0 International License</a>.  All versions and materials for the lifecycle are available <a href="https://doi.org/10.5281/zenodo.8075933">in Zenodo</a>.</p>

Below is a **summary table of the Biomedical Research Data Lifecycle** with all major RDM stages. It aligns with institutional, ethical, and funder expectations relevant to **reNEW, UCPH**, and **European biomedical research** environments.

## 🔄 **Biomedical Research Data Lifecycle – Summary Table**

***

<table data-header-hidden><thead><tr><th width="146"></th><th width="215"></th><th width="277"></th><th></th></tr></thead><tbody><tr><td><strong>Lifecycle Stage</strong></td><td><strong>Purpose &#x26; Key Outputs</strong></td><td><strong>Best Practices</strong> </td><td><strong>Common Risks &#x26; Mitigations</strong></td></tr><tr><td><strong>1. Plan &#x26; Design</strong></td><td>Define what data will be collected, created, or reused and how it will be managed. <strong>Output:</strong> Data Management Plan (DMP).</td><td><ol><li>Use institutional/funder-compliant DMP templates (e.g., DMPonline)</li><li>Integrate UCPH-approved storage solutions (ERDA, REDCap)</li><li>Address GDPR and consent for sensitive data</li><li>Update DMP throughout the project lifecycle</li></ol></td><td><p><strong>Risk:</strong> Static or incomplete DMP </p><p><strong>Mitigation:</strong> Schedule regular DMP reviews and assign update responsibility</p></td></tr><tr><td><strong>2. Collect &#x26; Create</strong></td><td>Capture or generate data through experimental, observational, or computational methods. <strong>Output:</strong> Raw data and metadata.</td><td><ol><li>Use ELNs or digital lab notebooks to capture contextual metadata</li><li>Standardize file naming and folder structures</li><li>Implement data quality control procedures at the point of collection</li></ol></td><td><p><strong>Risk:</strong> Metadata not captured <strong>Mitigation:</strong> Require lab-level metadata templates</p><p><strong>Risk:</strong> Unsecure data storage <strong>Mitigation</strong>: Use managed network storage, not personal devices</p></td></tr><tr><td><strong>3. Analyze &#x26; Collaborate</strong> </td><td>Transform raw data into analyzable formats; conduct computational and statistical analyses. <strong>Output:</strong> Processed data, results, and analysis scripts.</td><td><ol><li>Use version control (e.g., Git) for code and datasets</li><li>Record all processing steps (e.g., workflows, software versions)</li><li>Apply reproducible workflow tools (Snakemake, Nextflow, Galaxy)</li></ol></td><td><p><strong>Risk:</strong> Untraceable changes <strong>Mitigation:</strong> Track provenance and document transformations</p><p><strong>Risk:</strong> Irreproducibility <strong>Mitigation:</strong> Automate and share workflows</p></td></tr><tr><td><ol start="4"><li><strong>Evaluate &#x26; Preserve</strong></li></ol></td><td>Securely store final datasets and documentation for long-term access. <strong>Output:</strong> Archived data package (data + metadata + documentation).</td><td><ol><li>Deposit in domain-specific or institutional repositories (e.g., Zenodo, PRIDE, ArrayExpress)</li><li>Use open, non-proprietary file formats- Assign persistent identifiers (e.g., DOIs)</li><li>Define retention periods per UCPH/funder policy</li></ol></td><td><p><strong>Risk:</strong> Data loss or inaccessibility </p><p><strong>Mitigation:</strong> Use repositories with long-term guarantees and metadata standards</p></td></tr><tr><td><strong>5. Share &#x26; Publish</strong></td><td>Make data available to others, either openly or with controlled access. <strong>Output:</strong> Public or restricted dataset, Data Availability Statement.</td><td><ol><li>Select appropriate repository (subject-specific, institutional, or controlled access)</li><li>Anonymize or pseudonymize sensitive data- Choose proper license (e.g., CC-BY, CC0)</li><li>Comply with consent and legal agreements</li></ol></td><td><p><strong>Risk:</strong> GDPR breach <strong>Mitigation:</strong> Use secure repositories with access control; consult DPO</p><p><strong>Risk:</strong> Sharing non-documented data </p><p><strong>Mitigation:</strong> Require README, dictionary, and metadata files</p></td></tr><tr><td><strong>6. Discover &#x26; Reuse</strong></td><td>Enable others (and yourself) to find and reuse data to generate new knowledge. <strong>Output:</strong> Citable, documented, reusable datasets.</td><td><ol><li>Ensure data are FAIR (Findable, Accessible, Interoperable, Reusable)</li><li> Include citations to datasets in publications- Register datasets in data catalogs or registries</li><li>Promote reuse through metadata quality and open licensing</li></ol></td><td><p><strong>Risk:</strong> Low discoverability <strong>Mitigation:</strong> Use persistent IDs, index in catalog</p><p><strong>Risk:</strong> Misuse </p><p><strong>Mitigation:</strong> Apply standard licenses and clarify reuse terms</p></td></tr></tbody></table>
