# Lab 06 - Azure Infrastructure Security

> **Status:** In Progress

## AI Use Disclosure

AI tools may be used to support learning, troubleshooting, documentation organization, and technical review during this lab. All hands-on work, validation, screenshots, administrative decisions, and final documentation review will be completed by the project author. AI-generated guidance will be reviewed against Microsoft documentation and observed lab results before being accepted.

---

## Lab Metadata

| Item | Value |
|---|---|
| Difficulty | Beginner |
| Estimated Time | 2-3 hours |
| Lab Type | Microsoft Learn + discovery |
| SC-900 Domain | Describe the capabilities of Microsoft security solutions |
| Primary Objective | Describe Azure security capabilities and infrastructure protections |
| Previous Lab Dependency | Lab 05 - Identity Governance |
| Next Lab Dependency | Lab 07 - Microsoft Defender for Cloud |

---

## Objective

Build a practical understanding of Azure infrastructure security capabilities and explain how defense in depth protects networks, applications, management access, secrets, and workloads.

This lab is expected to cover:

- Defense in depth
- Network security groups (NSGs)
- Azure DDoS Protection
- Azure Firewall
- Web Application Firewall (WAF)
- Azure Bastion
- Azure Key Vault
- Secure network segmentation and management access
- The relationship between identity controls and infrastructure controls

---

## Business Problem Solved

Monroe Redstone Technology Group (MRTG) needs to protect Azure-hosted workloads from network attacks, unauthorized administrative access, web threats, exposed secrets, and weak segmentation.

Without layered infrastructure security, MRTG could experience:

- Overly permissive network access
- Unnecessary public exposure
- Distributed denial-of-service impact
- Weak control of inbound and outbound traffic
- Web application attacks
- Direct exposure of management ports
- Insecure storage of secrets, keys, and certificates
- Excessive reliance on a single security control

---

## Scenario

MRTG has established identity, authentication, authorization, Conditional Access, and identity-governance fundamentals.

The organization must now understand the Azure infrastructure controls that protect workloads after identities and permissions have been established.

This lab will use Microsoft Learn and discovery of Azure security services. Azure consumption resources should not be deployed solely to create portfolio evidence unless the learning value clearly justifies the cost and cleanup.

---

## Success Criteria

The lab will be considered successful when:

- The relevant Microsoft Learn module is completed
- The module assessment is passed
- Defense in depth can be explained
- NSGs can be distinguished from Azure Firewall
- DDoS Protection can be explained
- WAF can be distinguished from network firewall controls
- Azure Bastion can be explained as a secure management-access capability
- Azure Key Vault can be explained for secrets, keys, and certificates
- Knowledge checks are completed
- Evidence is sanitized and uploaded

---

## Environment

```text
Organization: Monroe Redstone Technology Group (MRTG)
Lab mode: Microsoft Learn + discovery
Azure consumption resources deployed: None planned for core lab
Estimated Azure consumption cost: $0.00 for discovery-only work
```

---

## Discovery Activities

Where Azure subscription access is available, perform read-only discovery of relevant security services without creating billable resources solely for evidence.

Possible discovery targets include:

1. Network security groups
2. Azure Firewall
3. DDoS Protection
4. Web Application Firewall-related services
5. Azure Bastion
6. Azure Key Vault

If a service requires deployment to inspect meaningfully, document the concept rather than deploying it unless cost and cleanup are explicitly justified.

---

## Planned Evidence

Keep the screenshot set small and useful:

| Screenshot | Evidence |
|---|---|
| `00-azure-security-module-starting-state.png` | Microsoft Learn starting state and module objectives |
| `01-azure-network-security-or-nsg.png` | Network security / NSG concept |
| `02-azure-firewall-waf-or-ddos.png` | Strong infrastructure protection concept |
| `03-azure-bastion-or-key-vault.png` | Secure management or secrets-management concept |
| `04-azure-security-module-complete.png` | Module assessment passed and completion |

Only screenshots actually captured and sanitized will remain in the final README.

---

## Completion Checklist

- [ ] Capture starting-state screenshot
- [ ] Review defense in depth
- [ ] Review NSGs
- [ ] Review Azure DDoS Protection
- [ ] Review Azure Firewall
- [ ] Review Web Application Firewall
- [ ] Review Azure Bastion
- [ ] Review Azure Key Vault
- [ ] Pass module assessment
- [ ] Complete Azure security discovery where practical
- [ ] Complete knowledge checks
- [ ] Upload sanitized screenshots
- [ ] Perform final repository evidence review
- [ ] Mark Lab 06 complete

---

## IAM / Security Relevance

Identity security determines who can authenticate and what they are authorized to do. Infrastructure security adds another layer by controlling how workloads are exposed, how traffic flows, how administrators connect, and how sensitive secrets are protected.

A strong security design should not assume that identity controls alone are sufficient.

---

## Cost and Licensing Considerations

```text
Estimated Azure consumption cost: $0.00 for discovery-only work
```

Some Azure security services can generate consumption charges when deployed. Cost validation is required before creating Azure Firewall, DDoS Protection plans, Bastion, or other billable infrastructure solely for lab purposes.

---

## Screenshot Inventory

To be completed after final evidence selection.

---

## Next Lab

```text
Lab 07 - Microsoft Defender for Cloud
```
