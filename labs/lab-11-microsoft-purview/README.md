# Lab 11 - Microsoft Purview

> **Status:** In Progress

## AI Use Disclosure

AI tools may be used to support learning, troubleshooting, documentation organization, technical review, and GitHub formatting during this lab.

All hands-on work, validation, screenshots, administrative decisions, and final documentation review must be completed by the project author. AI-generated guidance must be reviewed against Microsoft documentation and observed lab results before being accepted.

---

## Lab Metadata

| Item | Value |
|---|---|
| Difficulty | Beginner |
| Estimated Time | 2-4 hours |
| Lab Type | Microsoft Learn + read-only Microsoft Purview discovery |
| SC-900 Domain | Describe the capabilities of Microsoft compliance solutions |
| Primary Objective | Describe Microsoft Purview data security, data lifecycle, risk, audit, and eDiscovery capabilities |
| Previous Lab Dependency | Lab 10 - Service Trust and Compliance |
| Next Lab Dependency | Lab 12 - MRTG SC-900 Security, Compliance, and Identity Capstone |

---

## Objective

Build a practical SC-900-level understanding of Microsoft Purview and the major capabilities Microsoft uses to classify, protect, govern, retain, investigate, and audit organizational data.

This lab is expected to cover the current SC-900 compliance-solution objectives, including:

- Microsoft Purview overview and solution areas
- Data classification
- Content explorer and Activity explorer
- Sensitivity labels and sensitivity label policies
- Data Loss Prevention (DLP)
- Records management
- Retention policies
- Retention labels and retention label policies
- Insider Risk Management
- eDiscovery
- Audit

The current Microsoft Learn content will drive the final lab scope and screenshot evidence. If Microsoft splits these objectives across multiple fundamentals modules, the lab will document the modules actually completed rather than force an outdated single-module structure.

---

## Business Problem

Monroe Redstone Technology Group (MRTG) needs controls for protecting sensitive information throughout its lifecycle while also meeting legal, regulatory, operational, and investigation requirements.

Without data governance and compliance controls, MRTG could face:

- Sensitive information being shared inappropriately
- Inconsistent data classification
- Excessive retention of unnecessary data
- Premature deletion of required records
- Weak visibility into risky user behavior
- Difficulty responding to legal discovery requests
- Insufficient audit evidence
- Inconsistent handling of regulated information

Microsoft Purview provides capabilities for information protection, data loss prevention, lifecycle management, records management, risk investigation, auditing, and eDiscovery.

---

## Scenario

MRTG has completed its review of Microsoft trust, privacy, and assurance resources. It now needs to understand how Microsoft Purview helps an organization govern and protect its own data.

The lab will use Microsoft Learn and read-only Microsoft Purview portal discovery where practical. No production-style retention policy, sensitivity label, DLP policy, insider-risk policy, eDiscovery hold, or other compliance control will be deployed solely to generate portfolio evidence unless a safe lab exercise explicitly requires it and the change can be clearly validated and cleaned up.

---

## Success Criteria

The lab will be considered successful when:

- The relevant current Microsoft Learn material is completed
- Module assessments are passed
- Microsoft Purview can be explained at an SC-900 level
- Data classification can be explained
- Sensitivity labels can be explained
- DLP can be explained
- Retention policies and retention labels can be distinguished
- Records management can be explained
- Insider Risk Management can be explained
- eDiscovery can be explained
- Audit can be explained
- Read-only Purview portal discovery is completed where practical
- Knowledge checks are passed
- Evidence is sanitized and uploaded

---

## Environment

```text
Organization: Monroe Redstone Technology Group (MRTG)
Lab mode: Microsoft Learn + read-only Purview discovery
Compliance policies created for lab: None planned
Retention changes performed for lab: None planned
Legal holds created for lab: None planned
Azure resources created: None planned
Estimated Azure consumption cost: $0.00
```

---

## Discovery Activities

Where access and licensing allow, review without changing configuration:

1. Microsoft Purview portal overview
2. Data classification
3. Information Protection
4. Sensitivity labels
5. Data Loss Prevention
6. Data Lifecycle Management / retention
7. Records Management
8. Insider Risk Management
9. eDiscovery
10. Audit
11. Content explorer and Activity explorer where available

Do not publish real sensitive-information matches, user activity, eDiscovery case data, audit events, insider-risk cases, personal information, or tenant-specific compliance findings.

---

## Planned Evidence

Keep the final screenshot set small and concept-focused. The current Learn content should drive the exact filenames, but a likely five-screenshot structure is:

| Screenshot | Evidence |
|---|---|
| `00-purview-module-starting-state.png` | Current Microsoft Learn scope and objectives |
| `01-purview-information-protection.png` | Classification, sensitivity labels, or information protection |
| `02-purview-dlp-retention.png` | DLP, retention, or records-management concept |
| `03-purview-ediscovery-audit-risk.png` | eDiscovery, Audit, or Insider Risk concept |
| `04-purview-module-complete.png` | Final module assessment or learning-path completion evidence |

If the current SC-900 material spans multiple modules, the evidence set may use the strongest screenshots across those modules while remaining limited and non-redundant.

---

## Completion Checklist

- [ ] Capture starting-state screenshot
- [ ] Review Microsoft Purview overview
- [ ] Review data classification
- [ ] Review Content explorer and Activity explorer
- [ ] Review sensitivity labels and label policies
- [ ] Review Data Loss Prevention
- [ ] Review retention policies and retention labels
- [ ] Review records management
- [ ] Review Insider Risk Management
- [ ] Review eDiscovery
- [ ] Review Audit
- [ ] Complete read-only Purview portal discovery
- [ ] Pass relevant module assessments
- [ ] Complete knowledge checks
- [ ] Upload sanitized screenshots
- [ ] Perform final repository evidence review
- [ ] Mark Lab 11 complete

---

## IAM / Security Relevance

Microsoft Purview connects directly to identity and security because data-protection decisions frequently depend on who the user is, what data they are accessing, where the data is moving, and what action they are attempting.

Examples include:

```text
User identity
     +
Sensitive data classification
     +
Access / sharing action
     +
Compliance policy
     ↓
Allow, warn, block, protect, retain, audit, or investigate
```

Purview therefore complements IAM controls by applying governance and protection to the data identities are allowed to access.

---

## Cost and Licensing Considerations

```text
Estimated Azure consumption cost: $0.00
```

This lab does not require Azure consumption resources.

Microsoft Purview feature availability varies by Microsoft 365 and compliance licensing. Capabilities such as advanced auto-labeling, Insider Risk Management, advanced Audit, advanced eDiscovery, and some data-classification features can depend on specific licenses.

No paid license or trial should be enabled solely for portfolio evidence. Features unavailable in the tenant will be documented conceptually rather than bypassed.

---

## Screenshot Inventory

To be completed after final evidence selection.

---

## Next Lab

```text
Lab 12 - MRTG SC-900 Security, Compliance, and Identity Capstone
```
