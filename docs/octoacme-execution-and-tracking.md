# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Role-Specific Standup Guidance

Each role should focus on the following during daily standups:

| Role                  | What to Report                                                                 |
|-----------------------|--------------------------------------------------------------------------------|
| Developers            | Completed work, current task, blockers, PRs awaiting review                    |
| QA/Testing            | Test status, open defects, acceptance criteria verification progress           |
| UX Designer           | Design reviews completed, open design questions, upcoming design deliverables  |
| Release Manager       | Release readiness status, upcoming deployment windows, open release risks      |
| Data Analyst          | Metric tracking status, data anomalies, instrumentation issues                 |
| Site Reliability Eng. | System health, active incidents, on-call updates, reliability concerns         |
| Customer Support Lead | Emerging support trends, customer-reported issues relevant to current work     |
| Project Manager       | Overall progress, risks, escalations, upcoming milestones                      |

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

### Role-Based Escalation Guidance

| Escalation Type              | Primary Owner          | Escalate To                          |
|------------------------------|------------------------|--------------------------------------|
| Technical blocker            | Developer / Tech Lead  | Project Manager                      |
| Design conflict              | UX Designer            | Product Manager, then PM             |
| Release risk                 | Release Manager        | Project Manager, then Sponsor        |
| Reliability / incident       | SRE                    | PM + on-call team; Sponsor if P1     |
| Customer-impacting issue     | Customer Support Lead  | Product Manager, then PM             |
| Data / metric gap            | Data Analyst           | Product Manager                      |

## SRE & Customer Support Lead — Progress Tracking Checklist

Use this checklist each week to ensure SRE and Customer Support Lead are appropriately involved in execution tracking:

- [ ] SRE has reviewed current system health dashboards and flagged any concerns
- [ ] SRE has confirmed monitoring and alerting are in place for in-progress features
- [ ] Customer Support Lead has reviewed open support tickets for trends related to current sprint work
- [ ] Customer Support Lead has shared any critical customer feedback with the Product Manager
- [ ] Any reliability risks identified by SRE have been added to the Risk Register
- [ ] Any customer-impacting issues identified by Support Lead have been added to the backlog for triage

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
