# Venkata Pathuri

**Security Engineer · Detection Engineering · Incident Response**

`x0vrpp` · [LinkedIn](https://www.linkedin.com/in/vpathuri/) · [Public repositories](https://github.com/RajendraPathuri?tab=repositories)

I build detections, investigate incidents, and engineer security controls that hold up in practice. My progression runs from SOC analysis and SIEM engineering through incident response, detection development, and threat hunting, with cloud and identity security throughout.

I care about what an alert tells the analyst, which evidence supports the investigation, and what needs to change after containment.

## How I approach the work

- **Detection:** start with the behavior and telemetry, then define the investigation steps, false positives, and coverage limits.
- **Response:** correlate identity, endpoint, network, and cloud activity. Keep observed evidence separate from assumptions.
- **Engineering:** version the content, validate the behavior, document the gaps, and leave a clear rollback path.

## Selected work

**Detection Coverage Lab — MITRE ATT&CK & Atomic Red Team**

Ran 20+ simulations in a Windows, Sysmon, and Splunk lab, including PowerShell (T1059.001), LSASS access (T1003.001), and Registry Run keys (T1547.001). Wrote SPL detections and Sigma rules using Sysmon event IDs 1, 10, 11, and 13.

**Identity Attack Detection Engineering**

Built logic for suspicious OAuth grants, service principal credential changes, privilege escalation, and atypical sign-ins. Correlated identity events with endpoint and network telemetry, with reusable validation scenarios and rule-testing documentation.

**Detection-as-Code Automation Pipeline**

Designed a Git-based workflow for security content, with illustrative checks for rule structure, metadata, ATT&CK mapping, and deployment readiness. Documented testing outcomes, change tracking, and rollback requirements.

**GrandNode2 Secure Code Review**

Reviewed an ASP.NET Core commerce application using manual analysis, SonarQube SAST, and Snyk SCA. Documented CWE-mapped findings involving XSS, insecure deserialization, and vulnerable NuGet dependencies, alongside code-level fixes.

These are lab and engineering projects; lab matches do not establish production detection coverage.

**Public code:** [JSecPy](https://github.com/RajendraPathuri/jsecpy) — a Python-based Java security analyzer using parsing and pattern matching to flag potential OWASP-related issues for review.

## Tools & focus areas

| Area | Tools and practices |
| --- | --- |
| Detection engineering | Sigma, KQL, SPL, YARA, MITRE ATT&CK, detection-as-code, behavioral analytics, threat modeling, detection validation, purple teaming, Atomic Red Team |
| SIEM & analytics | Microsoft Sentinel, Splunk Enterprise Security, Elastic Security, Microsoft Defender XDR |
| Endpoint & identity | CrowdStrike Falcon, Microsoft Defender for Endpoint, Windows Event Logs, Sysmon, Entra ID, Okta, OAuth threat detection |
| Cloud security | AWS CloudTrail, GuardDuty, Azure Activity Logs, Azure Monitor, IAM, Kubernetes security telemetry |
| Threat detection & response | Threat hunting, incident investigation, log correlation, IOC enrichment, adversary simulation, detection tuning, SOAR |
| Engineering & automation | Python, SQL, PowerShell, Bash, Git, GitHub Actions, REST APIs, JSON, YAML, Terraform |
| AI security research | OWASP Top 10 for LLM Applications, MITRE ATLAS, prompt injection detection, LLM audit telemetry, AI API anomaly detection, sensitive-data exposure monitoring |

## Independent research in progress

I’m exploring **AI security observability** and open-source tooling around **Claude and MCP**: how to connect identity, model requests, retrieval, and tool execution without turning audit logs into another store of sensitive data.

Current research questions:

- How can third-party connectors and untrusted content redirect an agent’s authorized access?
- What distinguishes a DAN-style jailbreak attempt from indirect prompt injection and a legitimate security discussion?
- How should agents access private repositories and APIs while keeping credentials and sensitive code within the intended boundary?

The work includes illustrative reference architectures, proposed Python normalization and KQL/Sigma-style analytics, validation plans, and documented limitations. It is independent work in progress; proposed designs are not claims of live exploitation testing or production efficacy.

## Connect

I’m interested in collaboration on practical detections, investigation workflows, cloud identity security, and privacy-aware AI telemetry. [Find me on LinkedIn](https://www.linkedin.com/in/vpathuri/).

Also happy to talk biryani.
