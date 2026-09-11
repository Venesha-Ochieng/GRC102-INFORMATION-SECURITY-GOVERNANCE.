# INTERNATIONAL CYBERSECURITY AND DIGITAL FORENSICS ACADEMY

## GRC102: INFORMATION SECURITY GOVERNANCE

### Week 1 Practical Laboratory: Information Security Governance in Action

| Field | Details |
|---------|---------|
| Full Name | Venesha Adhiambo Ochieng |
| Registration Number | C11/26/CGRCE/17566 |
| Email Address | c11.cgrce2617566@icdfa.edu.ng |
| Cohort / Batch | Cohort11 |
| Date Submitted | 11th September 2026 |

---
# Summary

GlobalHealth Connect (GHC) has grown rapidly through two acquisitions and now operates a cloud-based patient management platform without a formal information security governance function. A contained data-leakage near-miss has prompted the Board to commission a governance uplift. This report responds to that mandate across five interlocking work packages: (1) a governance blueprint establishing structure and accountability; (2) a formal Information Security Charter giving the programme a mandate; (3) a Board-level security metrics briefing; (4) a Security Steering Committee (SSC) to resolve cross-functional conflict, tested against a live password-policy dispute between the CTO and IT Manager; and (5) a governance maturity assessment with a 12–18 month roadmap to Level 3 (Defined) across all six governance domains.

The overarching design principle is proportionate, risk-based governance that is fast enough not to obstruct GHC's growth and innovation agenda, but disciplined enough to protect patient trust and regulatory standing. Governance decisions (direction, policy approval, risk appetite) are separated from management decisions (implementation, day-to-day control operation), consistent with COBIT's distinction between governance and management and with ISO/IEC 27014's principles for governing information security.

# Key Stakeholders

| Stakeholder | Role | Primary Concerns |
|------------|------|------------------|
| Sarah Chen | Chief Executive Officer | Growth, reputation, operational efficiency and accountability. |
| Marcus Thorne | Chief Financial Officer | Return on investment, compliance cost and enterprise risk. |
| Elena Rodriguez | Chief Technology Officer | Developer productivity, technical debt and innovation. |
| David Miller | Board Member | Accountability, meaningful metrics and regulatory compliance. |

# Task 1 Governance Blueprint

**Executive request:** The CEO requires a formal security governance structure with clear roles, reporting relationships and accountability following the recent near-miss.

## Current Organizational Context

| Employee / Role | Department | Relevant Context |
|-----------------|------------|------------------|
| John Smith – IT Manager | IT Operations | Manages infrastructure and performs some security activities. |
| Jane Doe – Senior Developer | Development | Leads a key product development team. |
| Mark Johnson – Compliance Officer | Legal & Compliance | Focuses on healthcare regulatory obligations. |
| Emily White – Data Analyst | Finance | Handles sensitive financial information. |
| Robert Green – HR Manager | Human Resources | Owns onboarding and offboarding processes. |

## Required Evidence Task 1

### 1. A current-state governance gap assessment identifying the most important weaknesses in GHC's ad-hoc model.

| Governance Domain | Current-State Governance Weakness | Business Impact / Risk | Priority |
|-------------------|-----------------------------------|------------------------|----------|
| Roles & Responsibilities | No dedicated governance function or accountable executive. Security activity sits informally with the IT Manager (John Smith) alongside his infrastructure duties, with no role holding formal authority over security strategy, risk acceptance or policy. | Decisions default to whoever is available rather than whoever is accountable. This is the exact condition that let the near-miss occur without a clear escalation owner. | Critical |
| Risk Management | GHC identifies risk reactively including the recent near-miss rather than through a scheduled, proactive risk-assessment cycle. | GHC cannot demonstrate a defensible, evidence-based security posture to regulators, acquirers, clients, or insurers, and will keep discovering risk only after incidents. | Critical |
| Policy & Documentation | Inherited, inconsistent policy base from two acquisitions: GHC is effectively operating under multiple overlapping or absent policy sets, with no harmonization performed and no consistent review cycle. | Uneven control coverage across the merged entity, complicated compliance evidence for healthcare regulators, and a real chance that a legacy weakness from an acquired system was the source of the near-miss. | High |
| Cross-Functional Governance Structure | No forum exists where IT Operations, Development, Compliance, Finance, and HR jointly weigh security trade-offs; decisions are made unilaterally within silos (illustrated by the CTO/IT Manager password-policy dispute). | Cross-functional risks e.g., a control that helps compliance but harms developer productivity are not resolved at the right level, producing unmanaged friction or unmanaged risk. | High |
| Board Oversight & Reporting | The Board has no structured, standing channel for security information; it became aware of the issue's severity only reactively, after the near-miss, with no consolidated view of performance or risk appetite. | The Board cannot discharge its oversight duty or make informed risk-appetite and investment decisions as GHC scales toward its 2026 growth goals. | High |
| Data Ownership & Classification | Patient data (core to GHC's product), financial data (Finance), and employee data (HR) each have de facto working owners 

### 2. A proposed security governance organizational chart showing the Board, CEO, governance function and relevant business/technology relationships.

The structure below creates a single accountable governance owner. The Director of Information Security Governance (DISG) who reports directly to the CEO for operational sponsorship and resourcing, with a functional accountability to the Board Risk & Audit Committee to preserve independence when reporting on risk exposure, including risks arising from the CEO's own business units. A cross-functional Security Steering Committee gives business units a formal voice in security decisions, and Compliance and IT Operations retain their existing reporting lines while coordinating closely with the DISG.

```text
Board of Directors
│
├── Board Risk & Audit Committee
│
└── Chief Executive Officer (CEO)
    │
    ├── Chief Financial Officer (CFO)
    ├── Chief Technology Officer (CTO)
    │
    └── Director of Information Security Governance (DISG)
        │
        ├── IT Manager (John Smith)
        ├── Compliance Officer (Mark Johnson)
        │
        └── Security Steering Committee (SSC)
            │
            ├── Development Representative (Jane Doe)
            ├── Finance Representative (Emily White)
            ├── HR Representative (Robert Green)
            └── Other Business Stakeholders
```

