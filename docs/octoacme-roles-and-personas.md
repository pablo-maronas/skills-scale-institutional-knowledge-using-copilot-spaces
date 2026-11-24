# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## Release Manager

### Role Summary
The Release Manager owns release readiness and coordinates deployment execution, communications, rollback readiness, and post-release verification.

### Responsibilities
- Confirm that scope, acceptance criteria, CI/security gates, and rollback plans are complete
- Coordinate deployment windows and release communications
- Facilitate go/no-go decisions with accountable delivery and product leads
- Confirm deployment health and post-release verification
- Maintain release notes and handoff records

### Goals
- Reduce release risk and deployment surprises
- Complete consistent, observable, reversible releases
- Ensure stakeholders and support teams receive timely information

### Decision and Accountability Boundaries
The Release Manager owns release coordination and readiness evidence, but does not independently change approved product scope. Product Managers decide scope and trade-offs; Security or SRE Leads decide whether release safety requirements are met.

### Typical Communication
- Pre-release readiness review
- Deployment coordination and status announcements
- Post-release verification report

### Collaboration
- **Project Manager:** Aligns schedules, dependencies, and escalation actions.
- **Product Manager:** Confirms scope, release value, and stakeholder expectations.
- **Developers and QA/Testing:** Verify implementation, test evidence, rollback steps, and smoke-test readiness.
- **Support Lead and Stakeholders:** Coordinate announcements, known issues, support readiness, and customer impact.

---

## QA/Quality Lead

### Role Summary
The QA/Quality Lead defines test strategy and quality gates, coordinates acceptance evidence, and helps the team identify and address quality risks.

### Responsibilities
- Define test strategy, coverage, quality gates, and acceptance evidence
- Coordinate manual, integration, end-to-end, regression, and exploratory testing
- Facilitate defect triage and communicate quality trends or release risks
- Advise on testability and validate that acceptance criteria are measurable

### Goals
- Prevent defects from reaching production
- Make quality status and remaining risks visible
- Deliver consistent acceptance evidence

### Decision and Accountability Boundaries
The QA/Quality Lead owns quality planning and defect-risk reporting but may not waive a project-approved quality gate alone. Quality exceptions require documented agreement from the Product Manager and relevant technical or release owners.

### Typical Communication
- Test planning and quality-risk reviews
- Defect triage and QA status updates
- Acceptance and release evidence summaries

### Collaboration
- **Developers:** Collaborate on testability, automation, reproduction, and fixes.
- **Product Manager:** Clarify acceptance criteria, priority, and acceptable product trade-offs.
- **Project Manager:** Report QA status, dependencies, and schedule impacts.
- **UX/Design, Security, and SRE Leads:** Validate usability, security, and operational requirements.
- **Stakeholders:** Communicate acceptance status and unresolved risks when approval is required.

---

## UX/Design Lead

### Role Summary
The UX/Design Lead represents customer needs through research, interaction design, usability validation, and clear product workflows.

### Responsibilities
- Research customer and user needs
- Define information architecture, workflows, prototypes, and interaction patterns
- Validate usability and accessibility requirements
- Document design decisions and maintain reusable design guidance

### Goals
- Improve usability and accessibility
- Ensure the delivered experience matches customer and product needs
- Resolve design ambiguity before costly implementation

### Decision and Accountability Boundaries
The UX/Design Lead owns experience quality and user-centered design recommendations. Final scope and prioritization remain with the Product Manager; implementation feasibility trade-offs are resolved with Developers.

### Typical Communication
- Design reviews and usability sessions
- Research readouts and prototypes
- Acceptance walkthroughs

### Collaboration
- **Product Manager:** Align research, outcomes, priorities, and success measures.
- **Developers:** Address feasibility and implementation details during design and delivery.
- **QA/Quality Lead:** Define usability and acceptance experience evidence.
- **Project Manager:** Surface design dependencies and review/approval schedule risks.
- **Stakeholders and Support:** Incorporate customer feedback and real-world usage context.

---

## Security Lead

### Role Summary
The Security Lead establishes security requirements and reviews significant changes, security testing, risk trade-offs, and incident follow-up.

### Responsibilities
- Define security requirements and threat-review needs
- Coordinate security testing and remediation
- Review high-impact and security-sensitive changes
- Support incident follow-up and post-incident actions
- Advise on security gates and escalations

### Goals
- Reduce security risk and exposure
- Make security requirements and exceptions explicit
- Improve secure implementation and incident learning

### Decision and Accountability Boundaries
The Security Lead owns security requirements and risk recommendations. The Product Manager approves relevant scope or risk trade-offs, and project release owners decide go/no-go based on documented security gates and escalation guidance.

### Typical Communication
- Threat or design reviews
- Security-scan and remediation updates
- Incident briefings and security gate decisions

### Collaboration
- **Developers:** Review secure implementation and remediation work.
- **QA/Quality Lead:** Coordinate security validation and evidence.
- **Product Manager:** Align risk treatment with customer and business priorities.
- **Project Manager:** Escalate unresolved risks and maintain release dependencies.
- **Release Manager, SRE Lead, and Support:** Coordinate incident response and customer-impact communications.

---

## Data/Analytics Lead

### Role Summary
The Data/Analytics Lead defines measurable outcomes, instrumentation needs, reporting approaches, and evidence used for project decisions.

### Responsibilities
- Translate goals into metrics and measurable hypotheses
- Define telemetry, event, and reporting requirements
- Build or maintain dashboards and analysis plans
- Interpret data and communicate decision recommendations

### Goals
- Make outcomes measurable and observable
- Prevent gaps in instrumentation and reporting
- Support evidence-based prioritization and iteration

### Decision and Accountability Boundaries
The Data/Analytics Lead owns metric definitions and analytical methods. The Product Manager defines outcome priorities and approves success targets; implementation details are delivered with Developers.

### Typical Communication
- Metrics planning and dashboard reviews
- Experiment or launch readouts
- Decision checkpoints and retrospectives

### Collaboration
- **Product Manager:** Define success metrics, hypotheses, and trade-off evidence.
- **Developers:** Specify and verify telemetry implementation and data quality.
- **Project Manager:** Schedule reporting checkpoints and decision reviews.
- **QA/Quality Lead:** Validate instrumentation and measurement acceptance evidence.
- **Stakeholders:** Provide concise outcome and adoption updates.

---

## Operations/Site Reliability Lead

### Role Summary
The Operations/Site Reliability Lead establishes operational readiness, observability, capacity, reliability, and incident-response expectations.

### Responsibilities
- Define service-level indicators, alerts, capacity, and support expectations
- Review architecture and operational readiness
- Coordinate reliability testing and incident preparedness
- Maintain operational risk and action tracking
- Participate in incident response and post-incident improvement

### Goals
- Keep services observable and resilient
- Make operational risk explicit before and after launch
- Improve incident detection, response, and recovery

### Decision and Accountability Boundaries
The SRE/Operations Lead owns operational readiness criteria and reliability recommendations. Service design trade-offs are resolved with Developers and Product Managers, while unresolved operational release risks are escalated through the Project Manager and Release Manager.

### Typical Communication
- Operational readiness reviews
- Capacity and reliability assessments
- Incident updates and blameless retrospectives

### Collaboration
- **Developers and QA/Quality Lead:** Validate reliability, failover, monitoring, and recovery behavior.
- **Release Manager:** Coordinate deployment safeguards and rollback readiness.
- **Project Manager:** Maintain operational risks, dependencies, and escalation paths.
- **Security Lead and Support Lead:** Coordinate incident handling and customer-impact assessment.

---

## Support Lead

### Role Summary
The Support Lead provides production feedback and customer-impact context, prepares support for releases, and coordinates operational and incident handoffs.

### Responsibilities
- Summarize customer issues and recurring support themes
- Assess support readiness and release communication needs
- Help diagnose production problems and organize customer updates
- Feed recurring issues and improvements into backlog prioritization

### Goals
- Improve customer understanding and issue resolution
- Reduce surprise support impacts from releases or incidents
- Ensure customer feedback informs product and operational decisions

### Decision and Accountability Boundaries
The Support Lead owns support readiness and customer-impact communication within approved messaging. Product Managers prioritize recurring issues; Developers own diagnosis and implementation; Project or incident leads coordinate delivery and escalation processes.

### Typical Communication
- Release support briefings and known-issue updates
- Customer-impact summaries
- Incident communications and follow-up reviews

### Collaboration
- **Product Manager:** Bring recurring issues and customer evidence into roadmap decisions.
- **Developers:** Provide reproduction context and validate fixes or workarounds.
- **Release and Project Managers:** Coordinate announcements, deployment timing, and escalations.
- **SRE/Security Leads:** Participate in incident triage and operational or security updates.
- **Stakeholders:** Communicate customer impact, resolution status, and support implications.

---

## Role Interaction and Handoff Matrix

| Persona | Primary handoff or contribution to other roles | Key artifacts | Primary escalation point |
|---|---|---|---|
| Developers | Implement and test approved work; escalate technical risks and feasibility constraints | Code, tests, PRs, technical designs | Project Manager for delivery risk; Product Manager for scope trade-offs; SRE or Security Lead for operational/security risk |
| Product Manager | Owns outcomes and prioritization; accepts scope trade-offs | One-pager, roadmap, acceptance criteria, success metrics | Project Manager for execution alignment; Sponsor or Stakeholders for priority decisions |
| Project Manager | Coordinates plans, risks, dependencies, status, and decisions | Project plan, risk register, status updates, decision log | Product Lead or Sponsor for material scope, priority, or resource decisions |
| QA/Quality Lead | Provides quality plan and acceptance evidence; reports residual quality risk | Test strategy, defect reports, acceptance evidence | Project Manager for schedule or resourcing; Product Manager for acceptance trade-offs |
| UX/Design Lead | Provides validated workflows and experience guidance | Research, prototypes, design specs, usability findings | Product Manager for outcome or priority decisions; Project Manager for approval dependencies |
| Security Lead | Defines security requirements and verifies risk treatment | Threat reviews, security results, exception records | Project Manager and Release Manager for unresolved release gates; Security incident process for incidents |
| Data/Analytics Lead | Defines and reports outcome evidence | Metric plan, telemetry specification, dashboards | Product Manager for target or prioritization decisions; Project Manager for reporting dependencies |
| Release Manager | Coordinates readiness and deployment handoffs; confirms verification | Release plan, notes, rollback plan, go/no-go record | Project Manager for cross-team coordination; Product Manager for scope; SRE or Security Lead for operational or security gates |
| SRE/Operations Lead | Defines operational readiness and incident expectations | Service indicators, alerts, capacity plans, readiness checks | Project Manager or Release Manager for operational release risk; incident lead for active incidents |
| Support Lead | Provides customer-impact and support readiness feedback | Known issues, support plans, customer-impact updates | Product Manager for recurring issue prioritization; incident lead or Project Manager for active customer impact |

Ownership means final accountability for the named deliverable or decision. Contributors provide expertise and may execute work, but a handoff is complete only when the receiving role confirms the required evidence and next action.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
