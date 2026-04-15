# OctoAcme Project Management Overview

## Purpose
Provide a concise, shareable introduction to how OctoAcme runs projects so new teammates can quickly understand our approach, roles, and key artifacts.

## Scope
Applies to all cross-functional projects that deliver product features, services, or integrations.

## Principles
- Customer-first: prioritize customer value and usability.
- Iterative delivery: deliver small, testable increments.
- Clear ownership: each project has a named Project Manager (PM) and Product Lead.
- Data-informed decisions: measure impact and iterate based on evidence.
- Psychological safety: encourage feedback and learning.

## Core Roles

All OctoAcme projects are staffed with some or all of the following roles depending on project complexity and type. See [Roles & Personas](octoacme-roles-and-personas.md) for full descriptions.

- **Project Manager (PM):** coordinates delivery, schedules, risk, communications.
- **Product Manager (PdM):** defines outcomes, prioritizes backlog, and measures success.
- **Developers:** implement features, collaborate on design and testability.
- **QA/Testing:** validate quality and acceptance criteria.
- **UX Designer:** designs user-centric interfaces and advocates for user needs throughout the lifecycle.
- **Release Manager:** plans, schedules, and coordinates production releases.
- **Data Analyst:** defines and monitors project metrics and KPIs; supports data-informed decisions.
- **Site Reliability Engineer (SRE):** ensures system reliability, scalability, and rapid incident response.
- **Customer Support Lead:** brings customer feedback into planning and ensures support readiness for releases.
- **Stakeholders:** provide inputs and approvals.

## When to Engage Each Role

Different project types require different role involvement. Use the guidance below to ensure the right personas are engaged at the right time.

| Project Type                | Always Engage                                | Also Consider                                      |
|-----------------------------|----------------------------------------------|----------------------------------------------------|
| New customer-facing feature | PM, PdM, Developers, QA, UX Designer        | Data Analyst (metrics), Support Lead (readiness)   |
| Infrastructure / reliability | PM, Developers, SRE                         | Release Manager (deploy coordination)              |
| Data / analytics initiative | PM, PdM, Data Analyst, Developers           | QA (data validation), SRE (pipeline reliability)  |
| Hotfix / incident response  | PM, Developers, SRE, Release Manager        | Support Lead (customer comms), QA (smoke tests)    |
| Major release               | All roles                                    | —                                                  |

## Key Artifacts
- Project Charter / One-pager
- Roadmap and Release Plan
- Sprint/Iteration Backlog
- Acceptance Criteria & Definition of Done
- Risk Register
- Retrospective notes and action items

## Lifecycle (high-level)
1. Initiation: problem statement, stakeholders, high-level timeline.
2. Planning: scope, resources, milestones, dependencies.
3. Execution: build, test, review, iterate.
4. Release: deploy, verify, announce.
5. Close & Retrospective: capture learnings and next steps.

## Communication Cadence
- Weekly sync between PM + PdM
- Twice-weekly standups for delivery team (or as agreed)
- Monthly stakeholder updates
- Ad-hoc escalations as needed

## How to use these docs
- Keep the Project Charter updated in the project repo.
- Add process-specific docs into `.copilot/` if you want Copilot Spaces to use them as context.
