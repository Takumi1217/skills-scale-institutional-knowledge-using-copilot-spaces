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

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

---

## Additional Personas (proposed additions)

Below are proposed additional personas to improve clarity and accountability for cross-team and larger projects. For each persona we include responsibilities, primary artifacts they own, and typical interactions with existing roles.

### Technical Program Manager (TPM)
Role summary:
- Coordinates cross-team technical delivery, manages schedules, and tracks cross-repository dependencies.

Responsibilities:
- Maintain cross-team dependency tracker and milestone schedule
- Facilitate technical design trade-offs and cross-team planning
- Escalate and resolve cross-repo blockers

Primary artifacts:
- Dependency tracker, technical milestone plan, integration checklists

Interactions:
- PM/PdM: align on priorities and scope
- Developers/Engineering Leads: coordinate design and handoffs
- Project Manager: synchronize status and risks
- QA/Release Engineer: align integration and staging work

Reporting / touchpoints:
- Typically reports to an engineering manager or program lead; meets weekly with PM/PdM and leads.

---

### Delivery Lead
Role summary:
- Owns sprint-to-sprint delivery execution for a product area.

Responsibilities:
- Ensure backlog readiness and sprint plan execution
- Drive daily standups and removal of impediments
- Coordinate with QA to ensure acceptance criteria and test coverage

Primary artifacts:
- Sprint readiness checklist, release readiness checklist, burn-down reporting

Interactions:
- PM: coordinate scope and delivery timelines
- Developers: unblock and remove impediments
- QA Lead: ensure test coverage and release sign-off

Reporting / touchpoints:
- Operates closely with Project Manager; may be a senior engineer or team lead.

---

### QA Lead / Test Owner
Role summary:
- Defines test strategy and validates quality and acceptance criteria.

Responsibilities:
- Define test strategy (unit, integration, E2E, regression)
- Maintain test plans and automation priorities
- Sign off on release readiness from a QA perspective

Primary artifacts:
- Test plan, automation roadmap, release test checklist

Interactions:
- Developers: collaborate for testability and automation
- Release Engineer: coordinate staging and smoke tests
- PM/PdM: ensure acceptance criteria are met

Reporting / touchpoints:
- Works with Delivery Lead and Project Manager on release timelines.

---

### Release Engineer / SRE Release Owner
Role summary:
- Owns CI/CD, release automation, rollbacks, and post-deploy verifications.

Responsibilities:
- Maintain and evolve CI/CD pipelines and release tooling
- Define rollback and mitigation procedures
- Run or support production rollouts and post-deploy validations

Primary artifacts:
- Pipeline configurations, release playbooks, rollback runbooks

Interactions:
- Developers: build/release artifacts and deployment configuration
- QA Lead: staging validation and smoke tests
- Security Owner: ensure approvals and controls for releases

Reporting / touchpoints:
- Works with SRE/Platform teams; partners with Delivery Lead for scheduling releases.

---

### Security Owner / Security Reviewer
Role summary:
- Ensures security requirements are captured and reviewed.

Responsibilities:
- Perform security reviews, threat models, and coordinate scans
- Define security acceptance criteria and mitigation plans
- Approve releases when security posture meets requirements

Primary artifacts:
- Security review notes, checklists, mitigation backlog

Interactions:
- Developers: remediation guidance and secure design reviews
- CI/Release: integrate security scans into pipelines
- PM: inform risk decisions and release gating

Reporting / touchpoints:
- Part of security or platform organization; engaged during planning and before release.

---

### Observability / Monitoring Owner
Role summary:
- Defines metrics, alerting, and dashboards for features and platform health.

Responsibilities:
- Define success metrics and implement telemetry requirements
- Set alert thresholds and runbook references
- Validate post-release health and incident signals

Primary artifacts:
- Dashboards, alerts, runbooks, metric definitions

Interactions:
- Developers: implement telemetry and instrumentation
- Release Engineer: validate deploy-time checks and alerts
- Product: align metrics with success criteria

Reporting / touchpoints:
- Works with SRE/Platform and Data Analyst to ensure observability coverage.

---

### UX Researcher / Design Lead
Role summary:
- Owns user research and design consistency.

Responsibilities:
- Plan and run user research and usability testing
- Define accessibility guidance and design patterns
- Validate that implementation matches design intent

Primary artifacts:
- Research reports, design specs, accessibility checklist

Interactions:
- PdM: align research with product hypotheses
- Developers: handoff and QA on visual/interaction behavior
- PM: inform priorities based on user findings

Reporting / touchpoints:
- Part of Product/Design org; included early in planning and iteration cycles.

---

### Data Analyst / Instrumentation Owner
Role summary:
- Owns telemetry needs, experimentation metrics, and dashboards.

Responsibilities:
- Define required telemetry to measure success metrics
- Build dashboards and analyses to evaluate releases and experiments
- Validate instrumentation quality and data correctness

Primary artifacts:
- Event schema, dashboards, analysis reports

Interactions:
- PdM: define metric definitions and experiments
- Developers/Observability Owner: implement events and validate pipelines
- Product and Stakeholders: surface insights and KPIs

Reporting / touchpoints:
- Works with Product and Platform teams to ensure data-driven decisions.

---

### Customer Success Liaison
Role summary:
- Represents customer-facing perspectives and coordinates release communications.

Responsibilities:
- Bring customer insights and risk flags into planning
- Coordinate release enablement materials and communication
- Support customer-facing runbooks and escalation paths

Primary artifacts:
- Customer impact matrix, release communications plan, runbooks

Interactions:
- PM/PdM: align on customer priorities and readiness
- Support/Operations: prepare support runbooks and FAQs
- Product/Engineering: communicate major changes and workarounds

Reporting / touchpoints:
- Part of Customer Success or Support org; engaged ahead of major customer-impacting releases.

---

## Using these personas
- Add these personas into the project roles section of the Project Charter when relevant.
- For each project, indicate which personas are assigned or required and list the primary artifact owners (e.g., runbooks, dashboards, release playbooks).
- Capture primary touchpoints and reporting lines to reduce ambiguity and accelerate handoffs.
