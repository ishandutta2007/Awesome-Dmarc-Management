# Awesome-Dmarc-Management

## Top DMARC Management Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on DMARC Report Analysis, SPF/DKIM Monitoring, Email Authentication Enforcement & Brand Protection*  

**Last updated: September 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **DMARC Management**. These systems collect aggregate and forensic DMARC reports, visualize sender compliance, and guide organizations from monitoring (`p=none`) to enforcement (`p=quarantine`/`reject`) to stop email spoofing.



**Examples** include EasyDMARC, PowerDMARC, dmarcian, Valimail, Red Sift OnDMARC, URIports, DMARC Advisor, Mimecast DMARC Analyzer, Proofpoint Email Fraud Defense, and Sendmarc (the category leaders).



**Open-source emphasis**: DMARC has excellent open tooling. **parsedmarc**, **checkdmarc**, **Open DMARC Analyzer**, and related parsers enable fully self-hosted report processing and DNS validation. This section is heavily expanded.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[dmarcian, Valimail, Red Sift OnDMARC](https://dmarcian.com/)**  

  Leading DMARC platforms for report aggregation, source identification, and guided enforcement across large domains.



- **[EasyDMARC, PowerDMARC, Sendmarc, URIports, DMARC Advisor](https://easydmarc.com/)**  

  Full-lifecycle DMARC management—monitoring, SPF/DKIM alignment, and progressive policy rollout.



- **[Mimecast DMARC Analyzer, Proofpoint Email Fraud Defense](https://www.mimecast.com/)**  

  Enterprise email security suites with integrated DMARC analytics and brand-protection workflows.



- **[Other commercial DMARC platforms](https://dmarcian.com/)**  

  Additional managed services for multi-domain authentication and BIMI readiness.



## Open-Source GitHub Projects



- **[parsedmarc](https://github.com/domainaware/parsedmarc)**  

  Leading open-source DMARC report parser and CLI—aggregate and forensic reports, IMAP/Graph/Gmail ingestion, export to Elasticsearch, OpenSearch, Splunk, or PostgreSQL for self-hosted dashboards.



- **[checkdmarc](https://github.com/domainaware/checkdmarc)**  

  Open-source SPF and DMARC DNS record validator—CLI, API, and web interfaces for record correctness, lookup limits, and policy warnings.



- **[Open DMARC Analyzer](https://github.com/userjack6880/Open-DMARC-Analyzer)**  

  Open web UI for analyzing parsed DMARC data—built to work with open report parsers for medium-to-large report volumes.



- **[dmarcts-report-parser / Open Report Parser](https://github.com/techsneeze/dmarcts-report-parser)**  

  Widely used open parsers that ingest RUA reports into SQL databases for downstream analysis.



- **[dmarc-js-analyzer](https://github.com/dmarctrust/dmarc-js-analyzer)**  

  Client-side open DMARC aggregate report analyzer—runs entirely in the browser with no upload of report data.



- **[parsedmarc Docker / ELK stacks](https://github.com/search?q=parsedmarc+docker+OR+parsedmarc+kibana)**  

  Community dockerized deployments pairing parsedmarc with Elasticsearch/Kibana or Grafana for full self-hosted DMARC visibility.



- **[mailauth / open authentication libraries](https://github.com/search?q=DMARC+SPF+DKIM+library+open+source)**  

  Libraries for verifying SPF, DKIM, and DMARC in custom MTAs and security tooling.



- **[TLS-RPT & SMTP TLS reporting tools](https://github.com/domainaware/parsedmarc)**  

  parsedmarc and related projects also process SMTP TLS Reporting (TLS-RPT) alongside DMARC.



### Additional Strong Open-Source Options



- **Full self-hosted pipeline**: parsedmarc → Elasticsearch/OpenSearch → Kibana/Grafana.

- **DNS validation**: checkdmarc before and during policy changes.

- **Quick local analysis**: dmarc-js-analyzer for one-off report inspection.

- **Composable stacks**: Report mailbox → parsedmarc → SQL/ES → Open DMARC Analyzer or Kibana.

- Commercial platforms still lead in multi-tenant UX, managed rua infrastructure, and guided remediation at scale.



**Frameworks for building custom systems**:  

**parsedmarc** + **checkdmarc** are the core open DMARC toolkit.  

Add **Open DMARC Analyzer** or ELK/Grafana for visualization.  

Commercial platforms (dmarcian, Valimail, EasyDMARC, PowerDMARC, OnDMARC, etc.) provide turnkey rua hosting and analyst workflows.  

Security teams often self-host parsedmarc for data control and use commercial tools for complex multi-domain programs. Fully open DMARC monitoring is production-viable.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Moving to `p=reject` can block legitimate mail if sources are incomplete. Always monitor thoroughly, maintain accurate SPF/DKIM, and coordinate with all senders before enforcement. DMARC does not replace secure email gateways or user awareness.

- Open-source tools offer full data ownership but require you to operate mailboxes, parsers, and storage securely. Commercial platforms shift operational burden to the vendor. Neither replaces ongoing DNS and sender hygiene.



---



**Made for email security engineers, domain owners, and teams stopping spoofing with DMARC.**  

Let's expand open DMARC analytics while recognizing the guided enforcement and scale that leading commercial platforms deliver.
