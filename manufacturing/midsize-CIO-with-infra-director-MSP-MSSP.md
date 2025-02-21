# IT Infrastructure and Security RACI Matrix

Below is a RACI matrix for various infrastructure and cybersecurity functions (i.e., a table reflecting the roles and responsibilites across these functions).

RACI stands for: responsible, accountable, consulted, and informed.
Single letters are used in the table below to indicate each party's role in the IT function.

## Organization Information

This RACI matrix is an example for a midsize manufacturing business that has a mix of IT and OT operations.
As it relates to infrastructure and cybersecurity, the internal IT organization consists of a CIO and a director of infrastructure.
There is also a managed services provider (MSP) and a managed security services provider (MSSP), each contracted for various functions.

## RACI Matrix

| **#** | **Activity / Function** | **CIO** | **Infrastructure Director** | **MSP** | **MSSP** |
| --- | --- | --- | --- | --- | --- |
| **Strategy & Governance** | --- | --- | --- | --- | --- |
| 1 | **IT Strategy & Governance** | A | C (Technical Input) | I | I |
| 1a | **OT-IT Convergence Strategy** | A | R (Defines Approach) | C (Ops Integration) | C (Security Integration) |
| 2 | **Policy & Compliance** | A | C (Reviews) | R (Enforces Ops Policies) | R (Audits Security Compliance) |
| 2a | **Risk Assessment & Mitigation** | A | C (Reviews IT/OT Risks) | C (Ops Risks) | R (Security Risk Mitigation) |
| 3 | **Budgeting & Major Vendor Management** | A | R | C | I |
| 4 | **Asset Procurement & Ordering** | C | A | R (Executes) | I |
| 5 | **IT Invoice Validation & Payment** | A | R | C | I |
| **Infrastructure & Operations** | --- | --- | --- | --- | --- |
| 6 | **On-prem Server Administration** | I | R (OT Oversight) | A (Hands-on) | R (Security Input) |
| 7 | **Network (LAN/WAN) Administration (Cisco, Meraki, carriers)** | I | C (Oversight) | A & R (Config, Ops) | I |
| 7a | **Firewall Administration (Palo Alto)** | I | C (Approves Major Changes) | R (Implements Configs) | A (Defines Security Policies) |
| 8 | **Azure Resource Management** | I | C (Oversight) | A (Hands-on) | R (Security Checks via Defender for Cloud or Similar) |
| 9 | **Patch Management & Deployment** | I | C (Approves OT Patching Windows) | A (Deploys) | C (Prioritizes Vulnerabilities) |
| 10 | **Endpoint Management** (Intune - Workstations/Mobile + Windows Autopilot) | I | C (Policy Oversight) | A (Hands-on) | C (Security Best Practices) |
| 11 | **Microsoft 365 Administration** | I | C (Approves Configs) | A & R (Hands-on) | I |
| 11a | **Telephony** (Teams Voice, incl. AudioCodes ATAs, Neat Devices) | I | C (Approves Configs, Analyzes Plant/OT Needs) | A & R (Config, Ops, QoS) | C (Security Input) |
| 12 | **Defender for Office 365** (Email Hygiene, Anti-Phishing, etc.) - **Policy Configuration** | I | C (Approves Policies) | A (Configures) | C (Recommends Adjustments) |
| 12a | **Defender for Office 365** (Email Hygiene, Anti-Phishing, etc.) - **Monitoring & MDR** | I | C (Sev 1-2 Alerts Only) | R (Performs Containment per MSSP) | A (Monitors, Alerts, Initial Triage & Containment) |
| **OT Operations** | --- | --- | --- | --- | --- |
| 13 | **OT System Management** | C (Strategic Oversight) | A (Owns OT Policy) | R (Manages IT-OT Segmentation) | R (Security Input) |
| 13a | **OT Network Segmentation** | I | A (Approves Design) | R (Implements Changes) | R (Security Validation) |
| 14 | **OT Patch & Change Management** | I | A (Approves Changes) | R (Implements) | R (Security Validation) |
| **Identity & Access Management** | --- | --- | --- | --- | --- |
| 15 | **IAM – User Onboarding & Offboarding (AD/Entra ID)** | I | C (Approves) | A (Provisions) | R (Security Best Practices) |
| 15a | **IAM – Ongoing Access Reviews** | I | A (Approves) | R (Implements) | R (Monitors and Flags Risks) |
| **Security & Monitoring** | --- | --- | --- | --- | --- |
| 16 | **Defender for Endpoint** (AV/EDR) | I | R (OT Config Oversight) | R (Deploys/Config Changes) | A (Monitoring & Threat Analysis) |
| 16a | **Defender for Cloud Apps (CASB) & Identity (UEBA)** | I | C (Reviews) | R (Config Changes) | A (Monitoring & Threat Analysis) |
| 17 | **Security Monitoring (SIEM, Logs)** | I | R (OT Log Oversight) & C (Reviews SIEM Config & Major Alerts) | R (Configures Log Forwarding) | A (Monitoring, Hunting via Azure Sentinel) |
| 17a | **Network Security Monitoring (Proprietary Tool)** | I | C (Sev 1-2 Alerts Only) | R (Configures Devices per MSSP Guidance) | A (Monitors, Alerts, Recommends Network Adjustments) |
| 17b | **OT Security Monitoring (Nozomi/Claroty)** | I | C (Sev 1-2 Alerts Only) | R (Implements Immediate OT Fixes per MSSP) | A (Monitors, Alerts, Recommends OT Adjustments) |
| 18 | **Incident Response (Triage & Remediation)** | C (Sev 1-2) | R (OT Escalation) | R (Sev 3-4 Triage) | A (Forensics, Sev 1-2) |
| 18a | **Major Incident Coordination & Communication** | A | R (Stakeholders) | C (Ops Coordination) | C (Security Guidance) |
| 19 | **Vulnerability Management (Scanning & Remediation)** | I | R (OT Remediation Oversight)  | A (Scans, Remediates per MSSP Priorities) | R (Ingests Scans into SIEM, Prioritizes with Threat Intel) |
| 20 | **Performance & Security Reporting** | I | A (Reviews) | R (Ops Reports) | R (Security Reports) |
| 21 | **Security Awareness Training** | A | C (Approves Plant Staff Training Needs) | R (Configures Email Platform to Allow Phishing Tests) | A & R (Designs, Delivers, Tracks) |
| **Service Desk/Support** | --- | --- | --- | --- | --- |
| 22 | **L0/L1/L2 Service Desk (Remote Support)** | I | R (OT Issue Oversight) | A (Hands-on, incl. OT issue intake) | I |
| 23 | **L3 SMEs (Remote Support)** | I | C | A (Hands-on) | C (Security Support) |
| 24 | **On-Site Support (Field Services)** | I | R (OT Field Oversight) | A (Hands-on) | I |
| **BC/DR & Backup** | --- | --- | --- | --- | --- |
| 25 | **Disaster Recovery / Business Continuity** | A | R (Owns Plans) | R (Executes Tests) | C (Validates Security) |
| 25a | **Backup & Recovery Ownership** | I | C | A (Schedules, Verifies) | C (Advises) |
| **Projects** | --- | --- | --- | --- | --- |
| 26 | **Infrastructure Project Work** via separate contract or "bucket of hours" | I | C | A (Executes, Incl. End User Communications/Training When Applicable) | C (Security Input) |
| 26a | **Cybersecurity Project Work** via separate contract or "bucket of hours" | I | C | C (Operations Input) | A (Executes, Incl. End User Communications/Training, When Applicable) |
| **Architecture** | --- | --- | --- | --- | --- |
| 27 | **Enterprise Architecture / Engineering** | A | R (Design) | C (Input) | I |
| 28 | **Deployment & Provisioning** | I | R (OT Deployment Oversight) | A (Hands-on) | I |
| **General Responsibilities** | --- | --- | --- | --- | --- |
| 29 | **Configuration & Administration (General)** | I | R (OT Config Oversight) | A (Hands-on) | R (Security Input) |
| 30 | **Monitoring & Availability** | I | R (OT Availability Oversight) | A (Proactive) | R (Security Monitoring) |
| **Coordination** | --- | --- | --- | --- | --- |
| 31 | **MSP-MSSP Coordination** | C (Strategic Alignment) | R (Mediates OT Alignment) | A (Ops Lead) | R (Security Lead) |
| 32 | **Vendor Support Coordination** | I | A (Escalates Unresolved) | R (Ops Vendors) | R (Security Vendors) |
| 33 | **Contingency for Director Absence** | A (Oversees Contingency) | C (Defines Contingency Plan) | R (Ops Lead) | R (Security Lead) |
| 34 | **OT-IT-Security Conflict Resolution** | C (Strategic Oversight) | A (Resolves Disputes) | R (Ops Lead) | R (Security Lead) |

### Severity Levels

Note: as a placeholder, these are definitions of severity levels:

- A Severity 1 (Sev 1) incident, as used above, is a significant outage that stops the production or shipment of materials. For example, it might be a plant-wide outage.
- Sev 2 might be a critical app failure (e.g., ERP) - but one where business can continue for some time using offline/manual processes.
- Sev 3 is meant to be an incident affecting a noticeable portion of users or systems (e.g., 10-25% of workstations, a single production line, or a less-critical application), causing moderate disruption but not halting core manufacturing operations.
- Sev 4 might be a single-user issue.
