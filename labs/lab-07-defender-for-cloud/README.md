# Lab 07 - Microsoft Defender for Cloud

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
| Primary Objective | Describe the capabilities of Microsoft Defender for Cloud |
| Previous Lab Dependency | Lab 06 - Azure Infrastructure Security |
| Next Lab Dependency | Lab 08 - Microsoft Sentinel |

---

## Objective

Build a practical understanding of Microsoft Defender for Cloud and explain how it supports cloud security posture management and workload protection across Azure and multicloud environments.

This lab is expected to cover:

- Microsoft Defender for Cloud overview
- Cloud Security Posture Management (CSPM)
- Secure Score
- Security recommendations
- Regulatory compliance views
- Defender plans and workload protection concepts
- Security alerts and threat protection concepts
- Multicloud and hybrid coverage concepts
- The relationship between preventive posture management and active threat protection

---

## Business Problem Solved

Monroe Redstone Technology Group (MRTG) needs a way to continuously assess cloud security posture, identify weaknesses, prioritize remediation, and understand how workload protection can detect threats against cloud resources.

Without centralized cloud security posture management and workload protection, MRTG could experience:

- Misconfigured cloud resources
- Weak security baselines
- Poor visibility into security recommendations
- Difficulty prioritizing remediation work
- Limited regulatory-compliance visibility
- Inconsistent protection across workloads
- Delayed detection of attacks against cloud resources
- Fragmented security management across environments

---

## Scenario

MRTG has completed foundational Azure infrastructure-security review and now needs to understand how Microsoft Defender for Cloud evaluates security posture and helps protect workloads.

This lab will use Microsoft Learn plus sanitized read-only discovery in Microsoft Defender for Cloud where available. No Defender plan will be enabled, no billable workload-protection capability will be turned on, and no production security configuration will be changed solely to create portfolio evidence.

---

## Success Criteria

The lab will be considered successful when:

- The relevant Microsoft Learn Defender for Cloud module is completed
- The module assessment is passed
- CSPM can be explained
- Secure Score can be explained
- Security recommendations can be explained
- Regulatory compliance views can be explained at an SC-900 level
- Defender workload-protection concepts can be explained
- CSPM can be distinguished from workload protection
- Read-only Defender for Cloud discovery is completed where practical
- Knowledge checks are passed
- Evidence is sanitized and uploaded

---

## Environment

```text
Organization: Monroe Redstone Technology Group (MRTG)
Lab mode: Microsoft Learn + read-only discovery
Defender plans enabled for lab: None
Security policies modified: None
Azure resources created for lab: None
Estimated Azure consumption cost: $0.00 for discovery-only work
```

---

## Discovery Activities

Where tenant and subscription access allow, review the following without changing configuration:

1. Microsoft Defender for Cloud overview
2. Secure Score
3. Recommendations
4. Regulatory compliance
5. Environment settings / Defender plans
6. Security alerts or workload-protection areas, if visible without enabling new plans

Do not enable paid Defender plans, change policy assignments, dismiss recommendations, remediate production resources, or alter regulatory-compliance settings solely for portfolio evidence.

---

## Planned Evidence

Keep the screenshot set small and useful:

| Screenshot | Evidence |
|---|---|
| `00-defender-for-cloud-module-starting-state.png` | Microsoft Learn starting state and module objectives |
| `01-defender-for-cloud-secure-score.png` | Secure Score / posture-management concept |
| `02-defender-for-cloud-recommendations.png` | Security recommendations / remediation prioritization concept |
| `03-defender-for-cloud-workload-protection-or-compliance.png` | Workload protection or regulatory-compliance concept |
| `04-defender-for-cloud-module-complete.png` | Module assessment passed and completion |

Only screenshots actually captured and sanitized will remain in the final README.

---

## Completion Checklist

- [ ] Capture starting-state screenshot
- [ ] Review Defender for Cloud overview
- [ ] Review CSPM
- [ ] Review Secure Score
- [ ] Review security recommendations
- [ ] Review regulatory compliance
- [ ] Review Defender plans and workload protection
- [ ] Review alerts / threat-protection concepts
- [ ] Pass module assessment
- [ ] Complete read-only Defender for Cloud discovery
- [ ] Complete knowledge checks
- [ ] Upload sanitized screenshots
- [ ] Perform final repository evidence review
- [ ] Mark Lab 07 complete

---

## IAM / Security Relevance

Identity and access controls determine who can reach cloud resources and what they can do. Defender for Cloud adds another layer by assessing whether those resources are configured securely and by providing security recommendations and threat-protection capabilities.

A secure cloud environment requires both strong identity controls and continuous resource-security posture management.

---

## Cost and Licensing Considerations

```text
Estimated Azure consumption cost: $0.00 for discovery-only work
```

Microsoft Defender for Cloud includes posture-management capabilities, while additional Defender plans and workload-protection features can create Azure charges or licensing dependencies.

No paid Defender plan should be enabled solely to generate portfolio evidence. Any premium capability that is unavailable will be documented conceptually rather than bypassed.

---

## Screenshot Inventory

To be completed after final evidence selection.

---

## Next Lab

```text
Lab 08 - Microsoft Sentinel
```
