# OctoAcme Project Management Docs

This README centralizes OctoAcme's project management process documents and provides a short summary of the processes used across projects. Use this as the primary entry point for onboarding and day-to-day reference for project delivery practices.

Overview

OctoAcme organizes work around a clear lifecycle: initiation, planning, execution, release, and continuous improvement. Initiation captures the problem, stakeholders, success metrics, and a lightweight one-pager to authorize planning. Planning turns that authorization into a prioritized backlog, estimates, a Definition of Done, and a release/milestone roadmap. Execution emphasizes small, testable increments delivered through timeboxed iterations with clear acceptance criteria and a project board to track work from Backlog → Ready → In Progress → In Review → QA → Done.

Key workflows and quality practices

Day-to-day workflows focus on predictable reviews and automation. The team uses small pull requests (<= 400 lines when possible), links PRs to their issues and acceptance criteria, runs automated tests and security scans in CI before review, and requires at least one approval before merging. Releases are categorized (patch/minor/major) and require pre-release checks, smoke tests on staging, and documented rollback plans for safe production changes. Unit, integration, and end-to-end smoke tests are part of the quality strategy, alongside manual QA for feature acceptance when required.

Personas and communication

Roles are explicit: Product Managers define outcomes and success metrics, Project Managers coordinate delivery and risks, Developers implement and test, QA validates acceptance, and Stakeholders provide approvals and guidance. The core communication cadence includes daily standups, weekly delivery syncs, a PM–PdM weekly alignment, and regular stakeholder updates. Risks are tracked in a Risk Register and escalated via defined paths (team → PM → Product Lead → Sponsor) when needed.

Continuous improvement

Retrospectives are held after sprints, releases, or incidents and focus on a few actionable items that are added back into the backlog or risk register. The team tracks the impact of improvements and iterates on processes to reduce single-person dependencies and improve delivery predictability.

Links to process documents

- docs/octoacme-project-management-overview.md
- docs/octoacme-project-initiation.md
- docs/octoacme-project-planning.md
- docs/octoacme-execution-and-tracking.md
- docs/octoacme-risks-and-communication.md
- docs/octoacme-release-and-deployment.md
- docs/octoacme-retrospective-and-continuous-improvement.md
- docs/octoacme-roles-and-personas.md
