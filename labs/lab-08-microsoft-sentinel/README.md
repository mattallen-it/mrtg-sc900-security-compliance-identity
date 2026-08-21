# Lab 08 - Microsoft Sentinel

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
| Primary Objective | Describe security operations capabilities with Microsoft Sentinel |
| Previous Lab Dependency | Lab 07 - Microsoft Defender for Cloud |
| Next Lab Dependency | Lab 09 - Microsoft Defender XDR |

---

## Objective

Build a practical understanding of Microsoft Sentinel and explain how a cloud-native SIEM and SOAR platform collects security data, detects suspicious activity, creates incidents, supports hunting, visualizes security information, and automates response.

This lab is expected to cover:

- SIEM concepts
- SOAR concepts
- Microsoft Sentinel overview
- Data connectors
- Analytics rules
- Alerts and incidents
- Hunting
- Workbooks
- Automation rules and playbooks
- Security investigation and response workflows
- The relationship between Microsoft Sentinel and other Microsoft security services

---

## Business Problem Solved

Monroe Redstone Technology Group (MRTG) needs a centralized way to collect and correlate security data from multiple sources, detect threats, investigate incidents, and automate repetitive response actions.

Without centralized security operations capabilities, MRTG could experience:

- Fragmented security logs
- Slow incident detection
- Alert overload
- Difficulty correlating activity across multiple systems
- Limited threat-hunting capability
- Inconsistent incident-response processes
- Manual repetitive response work
- Weak visibility across cloud, identity, endpoint, and other security data sources

---

## Scenario

MRTG has completed cloud posture and workload-protection review with Microsoft Defender for Cloud.

The organization must now understand how Microsoft Sentinel supports broader security operations by collecting data, applying analytics, generating alerts and incidents, supporting threat hunting, and automating response.

This lab will use Microsoft Learn plus read-only discovery where possible. No Log Analytics workspace, Microsoft Sentinel instance, data connector, analytics rule, automation rule, or playbook should be deployed solely to create portfolio evidence unless the learning value clearly justifies cost, licensing, and cleanup.

---

## Success Criteria

The lab will be considered successful when:

- The relevant Microsoft Learn Sentinel module is completed
- The module assessment is passed
- SIEM and SOAR can be distinguished
- Data connectors can be explained
- Analytics rules can be explained
- Alerts and incidents can be distinguished
- Hunting can be explained
- Workbooks can be explained
- Automation rules and playbooks can be explained
- Read-only Sentinel discovery is completed where practical
- Knowledge checks are passed
- Evidence is sanitized and uploaded

---

## Environment

```text
Organization: Monroe Redstone Technology Group (MRTG)
Lab mode: Microsoft Learn + read-only discovery
Microsoft Sentinel deployment created for lab: None planned
Log Analytics workspace created for lab: None planned
Data connectors enabled for lab: None planned
Analytics rules created for lab: None planned
Automation rules or playbooks created for lab: None planned
Estimated Azure consumption cost: $0.00 for discovery-only work
```

---

## Discovery Activities

Where access allows, review the following without changing configuration:

1. Microsoft Sentinel overview
2. Data connectors
3. Analytics
4. Incidents
5. Hunting
6. Workbooks
7. Automation

Do not create a workspace, onboard Sentinel, enable data connectors, create analytics rules, run remediation actions, create Logic App playbooks, or modify production incidents solely for portfolio evidence.

---

## Planned Evidence

Keep the screenshot set small and useful:

| Screenshot | Evidence |
|---|---|
| `00-sentinel-module-starting-state.png` | Microsoft Learn starting state and module objectives |
| `01-sentinel-siem-soar-or-data-connectors.png` | SIEM/SOAR or data-ingestion concept |
| `02-sentinel-analytics-incidents.png` | Analytics, alerts, or incident-management concept |
| `03-sentinel-hunting-automation-or-workbooks.png` | Hunting, automation, or visualization concept |
| `04-sentinel-module-complete.png` | Module assessment passed and completion |

Only screenshots actually captured and sanitized will remain in the final README.

---

## Completion Checklist

- [ ] Capture starting-state screenshot
- [ ] Review SIEM
- [ ] Review SOAR
- [ ] Review Microsoft Sentinel overview
- [ ] Review data connectors
- [ ] Review analytics rules
- [ ] Review alerts and incidents
- [ ] Review hunting
- [ ] Review workbooks
- [ ] Review automation rules and playbooks
- [ ] Pass module assessment
- [ ] Complete read-only Sentinel discovery
- [ ] Complete knowledge checks
- [ ] Upload sanitized screenshots
- [ ] Perform final repository evidence review
- [ ] Mark Lab 08 complete

---

## IAM / Security Relevance

Identity systems, endpoints, applications, cloud resources, and network devices all generate security signals. Microsoft Sentinel helps a security operations team bring those signals together so suspicious activity can be correlated and investigated across multiple sources.

For IAM-focused security work, Sentinel can help surface and correlate identity-related events such as risky sign-ins, unusual authentication activity, privilege changes, and other security signals when relevant data sources are connected.

---

## Cost and Licensing Considerations

```text
Estimated Azure consumption cost: $0.00 for discovery-only work
```

Microsoft Sentinel can generate Azure consumption charges based on data ingestion, retention, analytics, automation, and related services. Logic App playbooks can also incur charges.

No paid deployment should be created solely to generate portfolio evidence. Any unavailable capability will be documented conceptually rather than bypassed.

---

## Screenshot Inventory

To be completed after final evidence selection.

---

## Next Lab

```text
Lab 09 - Microsoft Defender XDR
```
