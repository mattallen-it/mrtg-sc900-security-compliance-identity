# Lab 09 - Microsoft Defender XDR

> **Status:** In Progress

## AI Use Disclosure

AI tools may be used to support learning, troubleshooting, documentation organization, technical review, and GitHub formatting during this lab.

All hands-on configuration, validation, screenshots, administrative decisions, and final documentation review must be completed by the project author. AI-generated guidance must be reviewed against Microsoft documentation and the observed behavior of the lab environment before being accepted.

---

## Lab Metadata

| Item | Value |
|---|---|
| Difficulty | Beginner |
| Estimated Time | 2-3 hours |
| Lab Type | Microsoft Learn + read-only discovery |
| SC-900 Domain | Describe the capabilities of Microsoft security solutions |
| Primary Objective | Describe Microsoft Defender XDR and integrated threat protection capabilities |
| Previous Lab Dependency | Lab 08 - Microsoft Sentinel |
| Next Lab Dependency | Lab 10 - Service Trust and Compliance |

---

## Objective

Build a practical understanding of Microsoft Defender XDR and explain how Microsoft security products work together to provide integrated threat detection, investigation, and response across identities, endpoints, email and collaboration, cloud applications, and other security signals.

This lab is expected to cover:

- Microsoft Defender XDR overview
- Unified incidents and alerts
- Cross-domain detection, investigation, and response
- Microsoft Defender for Endpoint
- Microsoft Defender for Office 365
- Microsoft Defender for Identity
- Microsoft Defender for Cloud Apps
- Vulnerability management concepts
- Threat intelligence concepts
- Automated investigation and response concepts
- The relationship between Defender XDR and Microsoft Sentinel

---

## Business Problem Solved

Monroe Redstone Technology Group (MRTG) needs a way to correlate security activity across identities, endpoints, email, collaboration tools, and cloud applications instead of investigating each security product in isolation.

Without integrated extended detection and response, MRTG could experience:

- Fragmented security alerts
- Slow cross-domain investigations
- Difficulty identifying attack chains
- Repetitive analyst work
- Poor visibility into identity, endpoint, email, and cloud-app relationships
- Delayed containment and response

---

## Scenario

MRTG has completed its Microsoft Sentinel SIEM/SOAR review and now needs to understand Microsoft Defender XDR as the integrated threat-protection layer across Microsoft security workloads.

The lab will use Microsoft Learn and read-only discovery where available. No endpoint onboarding, policy deployment, connector enablement, remediation action, or licensing change should be performed solely to generate portfolio evidence.

---

## Success Criteria

The lab will be considered successful when:

- The relevant Microsoft Learn module is completed
- The module assessment is passed
- Defender XDR can be explained
- Integrated incidents and alerts can be explained
- Defender for Endpoint can be explained
- Defender for Office 365 can be explained
- Defender for Identity can be explained
- Defender for Cloud Apps can be explained
- Vulnerability management and threat-intelligence concepts can be explained at an SC-900 level
- Defender XDR can be distinguished from Microsoft Sentinel
- Read-only Defender portal discovery is completed where practical
- Knowledge checks are passed
- Evidence is sanitized and uploaded

---

## Environment

```text
Organization: Monroe Redstone Technology Group (MRTG)
Lab mode: Microsoft Learn + read-only discovery
Endpoint onboarding performed for lab: None planned
Security policies modified for lab: None planned
Remediation actions performed for lab: None planned
Licensing changes performed for lab: None planned
Estimated Azure consumption cost: $0.00 for discovery-only work
```

---

## Discovery Activities

Where access and licensing allow, review without changing configuration:

1. Microsoft Defender portal overview
2. Incidents and alerts
3. Endpoints / Defender for Endpoint areas
4. Email & collaboration / Defender for Office 365 areas
5. Identities / Defender for Identity areas
6. Cloud Apps / Defender for Cloud Apps areas
7. Vulnerability management
8. Threat intelligence
9. Automated investigation / response areas where visible

Do not onboard devices, isolate devices, remediate vulnerabilities, modify email policies, change identity sensors, enable connectors, or alter licensing solely for portfolio evidence.

---

## Planned Evidence

Keep the screenshot set small and useful:

| Screenshot | Evidence |
|---|---|
| `00-defender-xdr-module-starting-state.png` | Microsoft Learn starting state and current objectives |
| `01-defender-xdr-integrated-protection.png` | XDR architecture, integrated incidents, or cross-domain protection |
| `02-defender-xdr-products.png` | Defender product family or workload coverage |
| `03-defender-xdr-investigation-response.png` | Investigation, response, vulnerability, or threat-intelligence concept |
| `04-defender-xdr-module-complete.png` | Module assessment passed and completion |

Only screenshots actually captured and sanitized will remain in the final README.

---

## Completion Checklist

- [ ] Capture starting-state screenshot
- [ ] Review Defender XDR overview
- [ ] Review integrated incidents and alerts
- [ ] Review Defender for Endpoint
- [ ] Review Defender for Office 365
- [ ] Review Defender for Identity
- [ ] Review Defender for Cloud Apps
- [ ] Review vulnerability management
- [ ] Review threat intelligence
- [ ] Review automated investigation and response concepts
- [ ] Distinguish Defender XDR from Sentinel
- [ ] Pass module assessment
- [ ] Complete read-only Defender portal discovery
- [ ] Complete knowledge checks
- [ ] Upload sanitized screenshots
- [ ] Perform final repository evidence review
- [ ] Mark Lab 09 complete

---

## IAM / Security Relevance

Defender XDR is especially relevant to identity-focused security because attackers often move across multiple domains during a compromise.

A single investigation may involve:

```text
Suspicious identity activity
        +
Malicious email
        +
Endpoint execution
        +
Cloud application activity
        ↓
Correlated XDR incident
```

Integrated visibility helps analysts understand the broader attack chain instead of treating each alert as an isolated event.

---

## Cost and Licensing Considerations

```text
Estimated Azure consumption cost: $0.00 for discovery-only work
```

Many Microsoft Defender XDR capabilities depend on Microsoft 365, Defender, or related security licensing. Features available in the Defender portal can vary by tenant and license.

No paid license, trial, sensor, endpoint onboarding, or policy change should be enabled solely for portfolio evidence. Unavailable features will be documented conceptually rather than bypassed.

---

## Screenshot Inventory

To be completed after final evidence selection.

---

## Next Lab

```text
Lab 10 - Service Trust and Compliance
```
