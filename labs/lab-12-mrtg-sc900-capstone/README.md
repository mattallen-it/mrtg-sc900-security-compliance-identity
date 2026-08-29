# Lab 12 - MRTG SC-900 Security, Compliance, and Identity Capstone

> **Status:** In Progress

## AI Use Disclosure

AI tools may be used to support learning, troubleshooting, documentation organization, technical review, and GitHub formatting during this lab.

All hands-on work, validation, screenshots, administrative decisions, and final documentation review must be completed by the project author. AI-generated guidance must be reviewed against Microsoft documentation and observed lab results before being accepted.

---

## Lab Metadata

| Item | Value |
|---|---|
| Difficulty | Beginner / Intermediate |
| Estimated Time | 2-3 hours |
| Lab Type | Integrated discovery and incident-analysis capstone |
| SC-900 Domain | All four SC-900 domains |
| Previous Lab Dependency | Lab 11 - Microsoft Purview |
| Next Lab Dependency | None - series completion |

---

## Objective

Integrate the identity, security, threat-protection, governance, privacy, and compliance concepts from Labs 01-11 into one end-to-end SC-900 capstone scenario.

The capstone will validate that I can:

- Identify the identity and access controls involved in a security event
- Explain how Zero Trust principles apply
- Distinguish Microsoft Entra, Defender XDR, Sentinel, Defender for Cloud, and Purview responsibilities
- Explain how alerts become incidents and how investigation context is built
- Connect data protection and compliance controls to the incident
- Identify evidence sources for audit, eDiscovery, and compliance review
- Explain the shared-responsibility boundary
- Apply least privilege to administrative and investigative access
- Document a complete incident-analysis flow without creating unnecessary risk or cost

---

## Business Problem

Monroe Redstone Technology Group (MRTG) needs a repeatable way to understand and respond to a cross-domain security event involving identity compromise, malicious email, endpoint activity, cloud access, and possible sensitive-data exposure.

A real incident can cross multiple Microsoft security and compliance services. If each service is treated in isolation, analysts may miss the attack chain, apply the wrong control, or fail to preserve the evidence needed for legal and compliance review.

This capstone demonstrates how the Microsoft security, compliance, and identity ecosystem works together.

---

## Capstone Scenario

A fictional MRTG employee receives a phishing email and enters credentials into a malicious site.

The attacker then:

1. Attempts to sign in using the stolen credentials.
2. Accesses Microsoft 365 resources.
3. Executes suspicious activity from an endpoint.
4. Attempts to locate and download sensitive information.
5. Tries to share that information externally.

MRTG must determine:

- Which identity controls should reduce or block the attack
- Which services would detect suspicious activity
- How Defender XDR would correlate the attack
- How Sentinel could provide broader SIEM/SOAR visibility
- How Purview could protect, audit, retain, and investigate sensitive data
- What evidence would be required for security, legal, and compliance review
- Which administrative roles should have access to each investigation function

This is a fictional analysis scenario. No real compromise or destructive action is required.

---

## Success Criteria

The capstone will be considered successful when:

- The attack path can be explained from phishing through attempted data exfiltration
- Microsoft Entra controls are mapped to identity protection and access decisions
- Defender XDR components are mapped to email, identity, endpoint, and cloud-app signals
- Sentinel is correctly distinguished from Defender XDR
- Defender for Cloud is correctly distinguished from Defender XDR and Sentinel
- Purview controls are mapped to classification, DLP, audit, eDiscovery, retention, and records
- Zero Trust principles are applied to the scenario
- Least-privilege administrative access is documented
- Shared responsibility is explained
- A sanitized evidence set is captured
- No unnecessary paid or destructive configuration is performed
- Final project documentation is reviewed and the full 12-lab series is closed out

---

## Capstone Analysis Flow

~~~mermaid
flowchart LR
    Phish[Phishing Email] --> Creds[Credential Theft]
    Creds --> Entra[Microsoft Entra]
    Entra --> CA[Conditional Access / MFA / Risk Controls]

    Phish --> MDO[Defender for Office 365]
    Creds --> MDI[Defender for Identity]
    Endpoint[Suspicious Endpoint Activity] --> MDE[Defender for Endpoint]
    CloudApps[Cloud App Activity] --> MDCA[Defender for Cloud Apps]

    MDO --> XDR[Microsoft Defender XDR]
    MDI --> XDR
    MDE --> XDR
    MDCA --> XDR

    XDR --> Incident[Correlated Incident]
    Incident --> Sentinel[Microsoft Sentinel]
    Sentinel --> SOC[SOC Investigation / Automation]

    Sensitive[敏感 Data / Sensitive Data] --> Purview[Microsoft Purview]
    Purview --> Labels[Sensitivity Labels]
    Purview --> DLP[Data Loss Prevention]
    Purview --> Audit[Audit]
    Purview --> EDisc[eDiscovery]
    Purview --> Retention[Retention / Records]

    SOC --> Response[Containment and Response]
    Purview --> Response
~~~

---

## Capstone Tasks

### Task 1 - Identity and Zero Trust Review

Document how the following would apply to the compromised-user scenario:

- Authentication
- MFA
- Passwordless authentication
- Conditional Access
- Identity Protection / risk
- Least privilege
- Privileged Identity Management
- Access reviews
- Session revocation or account disablement where appropriate

### Task 2 - Threat Detection and Correlation

Map the attack to:

- Defender for Office 365
- Defender for Identity
- Defender for Endpoint
- Defender for Cloud Apps
- Defender XDR incidents and alerts
- Automated investigation and response

### Task 3 - SIEM / SOAR Review

Explain how Microsoft Sentinel would:

- Ingest or correlate broader security data
- Support analytics and incidents
- Support hunting
- Support automation and playbooks
- Complement Defender XDR rather than replace it

### Task 4 - Azure Security Boundary

Explain where Defender for Cloud fits:

- Cloud security posture
- Secure Score and recommendations
- Workload protection
- Regulatory compliance
- Multicloud and DevOps security

Document why Defender for Cloud is not the same as Defender XDR or Sentinel.

### Task 5 - Data Security and Compliance

Map the attempted sensitive-data exfiltration to:

- Information Protection
- Sensitivity labels
- DLP
- Insider Risk Management
- Adaptive Protection
- Data Security Posture Management
- Audit
- eDiscovery
- Data Lifecycle Management
- Records Management
- Compliance Manager

### Task 6 - Trust, Privacy, and Shared Responsibility

Explain:

- What the Service Trust Portal provides
- What Microsoft is responsible for
- What MRTG remains responsible for
- Why Microsoft certifications do not automatically make MRTG compliant
- How privacy principles such as data control, location, security, and defense relate to the scenario

### Task 7 - Portal Walkthrough

Perform a read-only walkthrough of the major portals where available:

- Microsoft Entra admin center
- Microsoft Defender portal
- Microsoft Sentinel
- Defender for Cloud
- Microsoft Purview
- Service Trust Portal

Do not expose real incidents, user identities, device names, tenant IDs, or sensitive compliance findings in screenshots.

---

## Planned Evidence

Keep the capstone evidence concise. The strongest final set will likely be five or six screenshots:

| Screenshot | Evidence |
|---|---|
| `00-capstone-scenario-and-objectives.png` | Capstone starting state or scenario checklist |
| `01-capstone-entra-zero-trust.png` | Identity / Conditional Access / risk concept |
| `02-capstone-defender-xdr-incident.png` | Defender XDR correlation or incident concept |
| `03-capstone-sentinel-security-operations.png` | Sentinel SIEM/SOAR concept |
| `04-capstone-purview-data-protection.png` | Purview protection / compliance concept |
| `05-capstone-series-complete.png` | Final project completion evidence |

The final evidence names can be adjusted to match the strongest actual screenshots collected.

---

## Cost and Licensing

~~~text
Estimated Azure consumption cost: $0.00
~~~

The capstone should not deploy billable resources solely for portfolio evidence.

Feature availability can vary by Microsoft 365, Entra, Defender, Sentinel, Purview, and Azure licensing. Unavailable features should be documented conceptually rather than enabled through unnecessary trials or purchases.

---

## Completion Checklist

- [ ] Review capstone scenario
- [ ] Complete identity and Zero Trust mapping
- [ ] Complete Defender XDR mapping
- [ ] Complete Sentinel SIEM/SOAR mapping
- [ ] Complete Defender for Cloud distinction
- [ ] Complete Purview data-security and compliance mapping
- [ ] Complete Service Trust / shared-responsibility mapping
- [ ] Complete read-only portal walkthrough
- [ ] Capture and sanitize final evidence
- [ ] Verify evidence in GitHub
- [ ] Complete final SC-900 concept review
- [ ] Mark Lab 12 complete
- [ ] Update root README to 12 of 12 complete
- [ ] Close the MRTG SC-900 project

---

## Series Completion

This lab will complete the **MRTG Security, Compliance & Identity Fundamentals** project.

The completed series will demonstrate practical foundations in:

- Security, compliance, and identity concepts
- Shared responsibility
- Zero Trust
- Microsoft Entra ID
- Authentication and authorization
- MFA and passwordless authentication
- Conditional Access
- Least privilege
- Identity governance
- Azure security
- Defender for Cloud
- Microsoft Sentinel
- Microsoft Defender XDR
- Service Trust Portal
- Microsoft Purview
- Data protection
- Compliance
- Threat detection and response
- Professional technical documentation
- Secure evidence handling
