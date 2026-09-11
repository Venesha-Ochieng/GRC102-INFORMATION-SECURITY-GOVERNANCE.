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
### 3. A RACI matrix covering at least six governance activities, including policy approval, risk review and incident response planning.

**R = Responsible** - performs the work  
**A = Accountable** - ultimately owns the decision/outcome  
**C = Consulted** - provides input  
**I = Informed** - kept aware of the decision/activity  
**AR = Accountable & Responsible combined**

| Governance Activity | BD | CEO | CFO | CTO | DISG | ITM | CO | SSC | BU |
|---------------------|----|-----|-----|-----|------|-----|----|-----|----|
| Security strategy development | A | C | I | C | R | I | C | C | I |
| Security policy development (drafting) | I | I | I | C | R | C | C | C | I |
| Security policy approval | A | C | I | C | R | I | C | C | I |
| Information Security Charter approval | A | R | C | I | C | I | I | I | I |
| Risk assessment & treatment (register review) | I | A | C | C | R | C | C | C | C |
| Incident response planning | I | I | I | C | A | R | C | C | I |
| Incident response execution (live event) | I* | I* | I | C | A | R | C | I | I |
| Security compliance monitoring | I | I | I | C | A | C | R | C | I |
| Security awareness & training | I | I | I | I | A | C | C | C | R |
| Security budget approval | A | C | R | I | C | I | I | I | I |
| Third-party / vendor risk review | I | I | C | C | A | C | R | C | C |
| Security metrics & Board reporting | I | C | I | I | AR | I | C | I | I |
| Resolve cross-functional disputes (e.g., password policy) | I | C | I | C | R | C | C | A | I |

**Legend:** BD = Board · CFO = Chief Financial Officer · CTO = Chief Technology Officer · DISG = Director, Information Security Governance · ITM = IT Manager · CO = Compliance Officer · SSC = Security Steering Committee · BU = Business Unit Managers · *Board/CEO informed only for material incidents.

### 4. A short explanation of how the proposed structure supports accountability, transparency, business alignment and risk management.

#### i. Accountability

Assigning a single Accountable role per activity directly closes the ownership gap identified in the current-state assessment. By separating security governance from general IT infrastructure management, GHC ensures clear boundaries, authority, and answerability across all operational activities.

#### ii. Transparency

Regular reporting from the DISG to executive leadership and the Board provides full visibility into the enterprise risk posture. The functional line to the Board Risk & Audit Committee guarantees that critical risk information reaches directors undiluted, even when balancing competing budget or delivery constraints.

#### iii. Business Alignment

Security decisions are evaluated within full business context through the cross-functional Security Steering Committee. This structure allows leadership to balance security requirements against innovation, customer trust, and operational speed.

#### iv. Risk Management

Establishing named risk owners and a formal assessment lifecycle replaces reactive decision-making with an evidence-based, audit-ready risk management process. Risks are systematically evaluated, assigned treatment plans, and escalated before resulting in operational disruption or regulatory non-compliance.

# Task 2 Information Security Charter

The CFO and Board require a formal mandate for the information security programme. Draft a concise but complete Information Security Charter that can be approved by executive management and referenced across the organisation.

## GHC Strategic Goals for 2026

| Strategic Goal | Business Intent |
|----------------|-----------------|
| Expand Market Share | Increase the client base by 25% through new features and entry into two regional markets. |
| Enhance Operational Efficiency | Reduce overhead by 10% and improve system uptime to 99.99%. |
| Maintain Customer Trust | Protect patient information and aim for zero major data breaches. |
| Foster Innovation | Invest in AI-driven diagnostics and secure data-exchange capabilities. |
| Achieve Regulatory Excellence | Meet applicable healthcare and data-protection obligations proactively. |

## Charter Sections

### Purpose - why the Information Security Programme exists and how it supports GHC.

The GlobalHealth Connect (GHC) Information Security Programme exists to protect the confidentiality, integrity, and availability of patient, financial, corporate, and third-party data. The Programme establishes a formal governance mandate to transform security into a predictable, well-governed enterprise capability that sustains customer trust, fulfills regulatory requirements, and directly enables GHC’s 2026 strategic objectives:

- Expand Market Share: Increase the client base by 25% through new features and entry into two regional markets.
- Enhance Operational Efficiency: Reduce overhead by 10% and improve system uptime to 99.99%.
- Maintain Customer Trust: Protect patient information and aim for zero major data breaches.
- Foster Innovation: Invest in AI-driven diagnostics and secure data-exchange capabilities.
- Achieve Regulatory Excellence: Meet applicable healthcare and data-protection obligations proactively.

### Scope — assets, systems, data, people and third parties covered by the programme.

The Programme covers all information assets owned, processed or stored by GHC or on GHC's behalf, including:

- All production, staging and development systems supporting GHC's cloud-based patient management platform;
- Patient health information and other regulated personal data, wherever it is processed, including systems inherited through acquisition;
- Corporate systems (finance, HR, collaboration tools) and the people, contractors and third parties who access them;
- Third-party and vendor relationships, including cloud infrastructure providers, software suppliers and outsourced service providers with access to GHC data or systems;
- Newly acquired entities, which are brought into scope from the effective date of acquisition and subject to a defined security integration plan.

### Authority — source of authority, decision rights and escalation powers.

This Charter is authorised by the Board of Directors and approved by the CEO. The Information Security Governance Lead is authorised to:

Coordinate the information security governance programme.

- Develop and maintain security policies and governance procedures.
- Request information needed for risk and compliance reviews.
- Escalate significant security risks to the CEO and Security Steering Committee.
- Recommend security controls and corrective actions.
- Monitor progress against agreed security objectives.
- Require departments to assign owners for identified risks and actions.
- Coordinate security reporting to executive management and the Board.

Department managers remain responsible for implementing approved security requirements within their areas. Significant exceptions, unresolved risks and issues affecting patient information, service availability, regulatory obligations or customer trust must be escalated through the Security Steering Committee to the CEO.

### Roles and Responsibilities — high-level governance accountabilities linked to Task 1.

| Role | Key Accountabilities & Responsibilities |
|------|-----------------------------------------|
| Board of Directors / Audit Committee | Provides ultimate oversight, approves enterprise risk appetite, approves this Charter, and reviews quarterly governance metrics. |
| Chief Executive Officer (Sarah Chen) | Executive sponsor; retains ultimate operational accountability, allocates resources, and resolves enterprise-level risk tradeoffs. |
| Director of InfoSec Governance (DISG) | Owns security strategy, policy framework, Enterprise Risk Register, and Board/SSC reporting; chairs the Security Steering Committee. |
| Chief Financial Officer (Marcus Thorne) | Evaluates security investments against risk exposure and ROI; approves capital allocation for GRC programs. |
| Chief Technology Officer (Elena Rodriguez) | Ensures "Security by Design" in engineering, secures product development pipelines, and balances developer speed with control standards. |
| IT Manager (John Smith) | Implements and operates infrastructure controls, executes patching SLAs, and provides operational support for incident response. |
| Compliance Officer (Mark Johnson) | Maintains the regulatory obligations register, monitors healthcare compliance (e.g., HIPAA/privacy), and coordinates audit evidence. |
| HR Manager (Robert Green) | Manages workforce security controls, including background checks, access onboarding/offboarding, and awareness training enforcement. |
| Data Analyst (Emily White) | Fosters data classification standards and ensures appropriate protection for sensitive patient and financial data sets. |
| All Staff & Contractors | Fulfill policy requirements, complete security awareness training, and immediately report suspected security incidents. |

### Key Principles — risk-based, business-aligned, proportionate and continuously improving security.

All security decisions, policies, and control implementations at GHC shall align with eight core principles:

- Risk-Based Prioritization: Security effort and capital investment are scaled according to the probability and business impact of identified risks rather than applied uniformly.
- Business Alignment: Security serves as a business enabler, supporting growth, innovation, system availability, and customer trust.
- Proportionate Controls: Security mechanisms must provide effective protection without imposing unnecessary friction on operational workflows or developer productivity.
- Single-Point Accountability: Every significant security activity, asset, and risk must have a clearly named executive owner.
- Security & Privacy by Design: Defense controls, data classification, and privacy mechanisms are built into system architectures and product lifecycles from inception.
- Protection of Sensitive Data: Patient healthcare data, financial records, and employee information receive rigorous protection across all lifecycle stages.
- Continuous Improvement: Program controls and maturity are routinely benchmarked, audited, and optimized against evolving threat vectors and operational metrics.
- Shared Responsibility: Information security is an enterprise-wide responsibility spanning every operational business unit, not solely an IT function.

### Reporting Structure — management, committee and Board reporting expectations.

| Governance Level | Primary Audience | Key Content & Reporting Scope |
|------------------|------------------|-------------------------------|
| Management Operations | Director of InfoSec Governance (DISG) | Operational metrics, patch status, vulnerability logs, and departmental security updates from IT Operations, Development, Compliance, and HR. |
| Steering Committee | Security Steering Committee (SSC) | Cross-functional risk reviews, metric dashboards, policy conflict resolutions, project milestone tracking, and resource allocation. |
| Executive Leadership | Chief Executive Officer (CEO) | Strategic risk exposure, resource requirements, policy deadlocks, compliance gaps, and major security trends. |
| Board Oversight | Board of Directors / Risk & Audit Committee | Business-focused Executive Summaries covering overall risk posture, threat trends, control effectiveness, and risk-appetite alignment. |

### Review and Approval — approval authority, review frequency and change control.

#### 1. Review frequency

- Scheduled Annual Review: This Charter shall be reviewed every 12 months by the Director of Information Security Governance (DISG), in coordination with the Security Steering Committee (SSC), and re-approved by the Chief Executive Officer and the Board Risk & Audit Committee to ensure alignment with GHC’s strategic growth goals and security maturity.
- Out-of-Cycle Triggers: An immediate, out-of-cycle review will be initiated following any major security incident or near-miss, a business acquisition or restructuring, a material change in healthcare regulatory obligations, or major infrastructure/technology changes.

#### 2. Approval authority and change control.

- Operational Amendments: Minor updates, procedural adjustments, and operational policy changes are proposed by the DISG, reviewed by the SSC, and approved by the Chief Executive Officer.
- Material Governance Amendments: Structural changes affecting governance authority, risk appetite thresholds, or strategic direction require formal recommendation from the CEO and SSC, with final ratification by the Board of Directors.
- Communication & Version Control: All approved revisions will be formally documented, communicated across the organization, and published to relevant portals for all employees, contractors, and acquired operational teams.

## Required Evidence Task 2

### Completed GHC Information Security Charter.

### A 1–2 paragraph justification memo to Marcus Thorne, CFO, explaining how the Charter supports GHC's strategic goals, accountability and investment decisions.

## MEMORANDUM

**TO:** Marcus Thorne, Chief Financial Officer  
**FROM:** Director of Information Security Governance  
**DATE:** September 10, 2026

**SUBJECT:** Information Security Charter - Strategic and Investment Justification

Marcus, the attached Information Security Charter converts security from an uncoordinated IT expense into a governed, accountable enterprise program designed to protect GHC's valuation and strategic growth. By establishing a risk-prioritized investment framework, the Charter directly aligns capital allocation with our 2026 objectives expanding market share by 25%, achieving 99.99% platform uptime, entering regional markets, and scaling AI-driven diagnostics. In cloud healthcare infrastructure, unmitigated risks introduce catastrophic financial exposure from regulatory fines, client churn, and system downtime; enforcing "Security by Design" across acquisitions and product development eliminates post-deployment remediation costs and protects our operational margins.

From an investment and accountability perspective, the Charter establishes a single named governance lead (the DISG) for spend justification and introduces predictable cost controls through the Security Steering Committee, on which you sit. Instead of reactive, ad-hoc funding requests, you will receive risk-adjusted proposals evaluated against return on investment and business context before funds are committed. Furthermore, structured quarterly reporting to the CEO and Board Risk & Audit Committee delivers transparent oversight, allowing us to benchmark control performance directly against budget execution ahead of our planned 2026 market expansion.

# Task 3 Board Reporting and Security Metrics

The Board has requested a concise, business-focused security update. Select the most decision-useful metrics from the six-month dataset, interpret the trends and present the organisation's security posture without unnecessary technical jargon.

| Month | Phishing | Malware | Critical Vulns Patched | Patching % | Training % | High-Risk Incidents |
|---------|---------|---------|------------------------|------------|------------|--------------------|
| September | 150 | 25 | 10 of 15 | 67% | 45% | 2 |
| October | 180 | 30 | 12 of 20 | 60% | 50% | 3 |
| November | 210 | 35 | 15 of 25 | 60% | 55% | 4 |
| December | 250 | 40 | 18 of 30 | 60% | 60% | 5 |
| January | 280 | 45 | 20 of 35 | 57% | 65% | 6 |
| February | 320 | 50 | 22 of 40 | 55% | 70% | 7 |

## Required Evidence Task 3

### A one-page Board Executive Summary containing an overall Red/Amber/Green posture assessment and justification.

Over the six-month period from September to February, GlobalHealth Connect's (GHC) security posture has deteriorated significantly as external threat activity outpaces internal defensive capacity. High-risk security incidents have increased by 250% (rising from 2 to 7 per month), driven by a 113% surge in phishing attempts (150 to 320) and a 100% increase in malware detections (25 to 50).

Compounding this heightened threat volume, GHC's technical remediation throughput has declined. The critical vulnerability patching rate dropped from 67% to 55%, widening the exposure window for cloud-hosted patient data. While security awareness training completion showed consistent progress improving from 45% to 70% this single positive trend has not translated into a reduction in security events or high-risk incidents.

### Five selected security metrics showing current status, six-month trend and concise business commentary.

| Metric | Baseline (Sep) | Current Status (Feb) | 6-Month Trend & Rate | RAG Status | Business Commentary & Operational Impact |
|----------|----------------|----------------------|----------------------|------------|-------------------------------------------|
| High-Risk Security Incidents | 2 / mo | 7 / mo | ▲ +250% ((7-2)/2)*100 | RED | Direct Operational Harm: Incidents more than tripled over six months. Shows that attacks are bypassing defenses and consuming response bandwidth, directly threatening patient data, customer trust, and platform uptime. |
| Critical Vulnerabilities Patched (%) | 67% (10 of 15) | 55% (22 of 40) | ▼ -12% Rate ((55-67)/67)*100 | RED | Backlog Expansion: Unpatched critical vulnerabilities grew from 5 to 18 open issues. Engineering capacity is failing to keep pace with new vulnerability discoveries, extending system exposure windows. |
| Phishing Attempts Detected | 150 / mo | 320 / mo | ▲ +113% ((320-150)/320)*100 | RED | Escalating Threat Vector: Attempts more than doubled, reflecting increased market visibility post-acquisition. Email remains the primary intrusion vector for credential theft and account takeover. |
| Malware Detections | 25 / mo | 50 / mo | ▲ +100% ((50-25)/50)*100 | RED | Perimeter Pressure: Doubled in six months, tracking in proportion with rising phishing volume. Indicates endpoint defenses and email perimeters are under sustained, increasing strain. |
| Security Training Completion (%) | 45% | 70% | ▲ +25% ((70-45)/70)*100 | AMBER | Improving Culture: Participation improved steadily, showing governance focus yields results. However, 30% of staff remain untrained against a rising threat volume, leaving the human layer exposed. |

### At least two priority risks/issues and two actionable recommendations.

#### Priority Risk 1: Increase in High-Risk Security Incidents

**Evidence:**  
The number of high-risk security incidents increased significantly from 2 to 7 during the reporting period.

**Potential Impact:**

- Exposure of sensitive patient information.
- Loss of customer trust and confidence.
- Non-compliance with regulatory and legal requirements.
- Disruption to the availability of critical healthcare services.
- Increased incident response, remediation, and recovery costs.

**Priority:** High

#### Priority Risk 2: Declining Critical Vulnerability Remediation Performance

**Evidence:**  
Critical vulnerability remediation rates declined from 67% to 55%, while the number of identified critical vulnerabilities increased from 15 to 40.

**Potential Impact:**

- Critical security weaknesses may remain unaddressed for extended periods.
- Increased likelihood of cyberattacks and security incidents.
- Greater risk of compromise to critical GHC systems and data.
- Higher remediation and recovery costs if vulnerabilities are exploited.

**Priority:** High

### Recommendations

#### 1. Implement a Critical Vulnerability Remediation Programme

Management should establish a structured vulnerability remediation programme to ensure critical vulnerabilities are identified, prioritised, and resolved in a timely manner.

**Actions:**

- Identify and prioritise all outstanding critical vulnerabilities based on business impact and risk.
- Assign clear ownership and accountability for each vulnerability.
- Establish remediation deadlines aligned with risk severity.
- Report unresolved critical vulnerabilities to the Security Steering Committee.
- Escalate significant overdue vulnerabilities to executive management for action.

**Expected Outcome:**  
Improved critical vulnerability remediation performance above the current 55%, resulting in fewer outstanding critical vulnerabilities and a reduced overall risk exposure.

#### 2. Enhance Phishing Prevention and Security Awareness

GHC should strengthen its security awareness programme by aligning training initiatives with the evolving threat landscape and focusing on high-risk user groups.

**Actions:**

- Provide targeted phishing awareness training for employees most at risk.
- Conduct regular phishing simulation exercises to reinforce learning.
- Deliver additional support and training to employees who repeatedly fall victim to phishing attempts.
- Continue monitoring and reporting security awareness training completion rates.
- Regularly report phishing trends, malware activity, and related incidents to management.

**Expected Outcome:**  
Increased employee awareness and resilience against phishing attacks, leading to a reduction in successful phishing incidents, malware infections, and overall security incidents.

### A short rationale explaining why your five selected metrics are suitable for Board oversight.

The five selected metrics translate complex technical activity into clear, business-relevant signals for board-level oversight:

- High-Risk Incidents (Outcome Indicator): Tracks realized business impact and operational harm the primary metric for board accountability.
- Critical Vulnerability Patching Rate (Technical Health): Measures operational remediation efficiency percentage rather than raw counts, isolating whether GHC is closing exposure gaps faster than new flaws emerge.
- Security Training Completion (Human Control): Evaluates the direct impact of workforce investments and human-risk mitigation efforts.
- Phishing Volume & Malware Detections (Threat Context): Quantifies external attack pressure, providing essential context to determine whether rising incidents stem from weakening defenses or an intensifying threat landscape.

# 8. Task 4 Security Steering Committee

A dispute has emerged between the CTO and IT Manager regarding a proposed password policy. The CTO believes the policy will create excessive friction; the IT Manager argues that stronger controls are necessary. The CEO wants a formal Security Steering Committee (SSC) to resolve such cross-functional issues.

**Conflict context:** The proposed policy requires 16-character complex passwords changed every 30 days without password-manager integration. The CTO recommends a more balanced approach emphasizing multi-factor authentication and secure password-management.

## Required Evidence Task 4

### Security Steering Committee Terms of Reference covering purpose, scope, membership, responsibilities, meeting cadence, decision authority and reporting.

#### Purpose

The Security Steering Committee (SSC) provides a structured, cross-functional forum for overseeing information security at GlobalHealth Connect (GHC). The SSC ensures that security decisions are aligned with GHC’s business objectives, protect patient and organizational information, manage security risks, and consider operational and technology requirements.

The SSC also provides a formal mechanism for resolving disagreements between security, business, and technology functions, ensuring that security decisions are not made by one department in isolation.

#### Scope of Authority

The SSC oversees and adjudicates matters across the following core domains:

- Governance & Policy: Reviewing, approving, and recommending changes to information security policies, standards, and control frameworks.
- Risk & Exceptions: Evaluating major security risks, reviewing the Enterprise Risk Register, and approving policy exceptions/risk acceptances within Board-approved thresholds.
- Strategy & Roadmap: Prioritizing security investments, control enhancements, and roadmap initiatives prior to Board budget requests.
- Incident Review & Performance: Monitoring the security metrics dashboard, evaluating major incident post-mortems, and tracking key remediation SLAs.
- Cross-Functional Resolution: Settling operational security disputes between departments that exceed single-function authority.

#### Membership

| Member | Role | Committee Function |
|----------|------|-------------------|
| Sarah Chen | CEO | Executive sponsor and senior decision-maker; provides executive direction. |
| Director of Information Security Governance (DISG) | Information Security Governance | Chair and committee coordinator; sets the agenda, presents security risks and metrics, and maintains the decisions and actions log. |
| Elena Rodriguez | CTO | Technology, product, and development perspective. |
| Marcus Thorne | CFO | Financial, investment, and enterprise-risk perspective. |
| John Smith | IT Manager | IT operations and infrastructure perspective; participates in operational and technical matters. |
| Mark Johnson | Compliance Officer | Regulatory, compliance, and healthcare-security perspective. |
| Robert Green | HR Manager | Workforce policies, onboarding/offboarding, conduct, and security awareness. |
| Rotating Business Unit Representative | Business Unit Representative | Provides operational and business-unit input on matters affecting specific functions. |

#### Key Responsibilities

1. Dispute Resolution: Evaluate and resolve cross-functional conflicts between security requirements and business productivity.
2. Policy Approval & Recommendations: Approve operational guidelines and recommend formal enterprise security policies for Board ratification.
3. Risk Management & SLAs: Prioritize risk register items, track vulnerability remediation progress against defined SLAs, and approve bounded risk acceptances.
4. Metrics & Performance Oversight: Review monthly key performance indicators (KPIs) and key risk indicators (KRIs) between quarterly Board reporting cycles.
5. Investment Prioritization: Review business cases for security initiatives and evaluate expected business value and risk reduction.
6. Escalation: Escalate unresolved risks, major incidents, or policy exceptions exceeding committee threshold directly to the CEO and Board Risk & Audit Committee.

#### Meeting Cadence

- Regular meetings: Monthly.
- Ad-hoc meetings: The Chair may call additional meetings when a major security incident, high-risk issue, or urgent cross-functional dispute requires immediate attention.
- Annual review: The SSC will review its effectiveness and Terms of Reference at least once every year.

#### Decision Authority

The SSC may:

- Approve or reject security policy exceptions and risk acceptances that fall within the risk appetite and authority approved by the Board.
- Resolve security-related disagreements between departments within its delegated authority.
- Prioritise security initiatives, remediation activities, and corrective actions.
- Assign responsible owners and deadlines for agreed actions.
- Recommend security policies and significant control changes for approval through GHC’s established governance structure.
- Escalate matters that exceed its authority or cannot be resolved by the committee.

#### Reporting and Board Relationship

The SSC will maintain formal reporting relationships with executive management and the Board.

- Minutes, decisions, and action items will be circulated to SSC members within five working days.
- The SSC will provide monthly updates to the CEO covering key decisions, significant risks, incidents, and outstanding actions.
- Security metrics, risk-register updates, and major security issues will be reported to executive management periodically.
- Significant unresolved risks and major security incidents will be escalated to the CEO and Board as appropriate.
- A summary of SSC decisions, key risks, and outstanding strategic issues will be incorporated into the quarterly Board security report.

### A sample agenda for the first SSC meeting with the password-policy conflict as a key discussion item.

## GlobalHealth Connect (GHC)

### Security Steering Committee – First Meeting

**Date:** 10 September 2026  
**Time:** 10:00 AM – 11:30 AM  
**Location:** Boardroom / Virtual Meeting  
**Chair:** Sarah Chen, CEO

| Time | Agenda Item | Lead | Purpose |
|--------|-------------|------|---------|
| 10 min | Welcome, Introductions and Terms of Reference | Sarah Chen / DISG | Welcome members, confirm membership, and review the SSC's purpose, responsibilities, authority, and meeting arrangements. |
| 15 min | Current Security Governance Priorities | DISG | Review key security governance gaps, current risks, security metrics, and priority areas requiring SSC attention. |
| 10 min | Password Policy Conflict – Background | CTO / IT Manager | Present the disagreement regarding the proposed password policy and explain the concerns from the technology and IT operations perspectives. |
| 30 min | Password Policy Options and Decision | SSC / DISG | Evaluate the proposed options based on security strength, user impact, technical feasibility, compliance, cost, and business impact, and agree on a preferred approach. |
| 10 min | Risk and Action Ownership | DISG | Document the decision, assign responsible owners, establish deadlines, and identify any required risk acceptance or policy exception. |
| 5 min | Reporting and Escalation | Chair / DISG | Agree on matters that require reporting or escalation to the CEO and Board. |
| 10 min | Any Other Business and Next Meeting | Chair | Discuss any additional security matters and confirm the date and priority topics for the next SSC meeting. |

### Password Policy Conflict

The SSC will use the password-policy conflict as its main decision-making discussion. The current proposal includes:

- Minimum 16-character complex passwords.
- Mandatory password changes every 30 days.
- No password-manager integration.

The committee will consider the security benefits and risks of the proposal alongside user experience, password fatigue, technical feasibility, operational impact, compliance requirements, and business needs.

The objective is to reach a risk-based and business-aligned decision. If the matter exceeds the SSC's delegated authority or the Board-approved risk appetite, it will be escalated to the CEO and, where necessary, the Board Risk & Audit Committee.

### Expected Outcomes

At the end of the first meeting, the SSC should have:

- Confirmed its Terms of Reference and membership.
- Identified the key security governance priorities.
- Reached a decision or recommendation on the password-policy conflict.
- Assigned owners and deadlines for agreed actions.
- Identified matters requiring escalation to senior management or the Board.
- Confirmed the next SSC meeting date and priority agenda items.

### A 1–2 paragraph briefing note to the CEO explaining how the SSC will resolve cross-functional conflict and maintain strategic alignment.

**To:** Sarah Chen, Chief Executive Officer  
**From:** Director of Information Security Governance  
**Date:** 10 September 2026  
**Subject:** How the Security Steering Committee Will Resolve Cross-Functional Conflict and Maintain Strategic Alignment

Sarah,

The Security Steering Committee (SSC) will provide GHC with a structured forum for resolving disagreements that involve security, technology, IT operations, compliance, and business needs. The current disagreement between the CTO and IT Manager over the password policy demonstrates the need for decisions to be made collectively rather than by one department. The SSC will consider both positions objectively, assess the risks, operational impact, technical feasibility, compliance requirements, and business needs, and then agree on a practical risk-based approach. For the password policy, the Committee can consider a balanced solution that combines strong authentication, multi-factor authentication (MFA), and secure password management while avoiding unnecessary password changes that may create user frustration and security weaknesses.

The SSC will maintain strategic alignment by ensuring that security decisions support GHC's business objectives, risk appetite, and growth plans. Each decision will be documented, assigned to a responsible owner, given a clear implementation deadline, and monitored for effectiveness. Matters that exceed the SSC's authority, risk appetite, or have significant financial, regulatory, or reputational impact will be escalated to the CEO and, where necessary, the Board Risk & Audit Committee. This approach will improve accountability and transparency while ensuring that security supports GHC's operations, customer trust, innovation, and future growth.
