# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner
- Mitigation plan
- Status

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status

## Role-Based Communication Templates

Each role has specific communication responsibilities. Use the templates below to ensure consistent and complete information sharing.

### Project Manager — Weekly Status Update
- Progress this week:
- Next steps:
- Risks & blockers:
- Ask / decisions needed:

### Product Manager — Roadmap & Backlog Update
- Features delivered this sprint:
- Upcoming priorities:
- Trade-off decisions made:
- Stakeholder asks or feedback needed:

### Release Manager — Release Readiness Update
- Release target date:
- Go/no-go status:
- Open release risks:
- Stakeholder actions required:

### SRE — System Health Update
- Current system status (uptime, error rates, latency):
- Active or recent incidents:
- Reliability risks for upcoming release:
- Recommended actions:

### Customer Support Lead — Customer Feedback Summary
- Top support tickets or trends this week:
- Customer-impacting issues flagged for the backlog:
- Support readiness for upcoming releases:
- Customer satisfaction indicators:

### Data Analyst — Metrics Update
- Key metrics this sprint (vs. targets):
- Data anomalies or gaps identified:
- Insights to inform backlog prioritization:

---

## Cross-Functional Dependency Mapping

When starting a new project or sprint, map cross-functional dependencies to reduce surprises:

1. **Identify dependencies:** For each backlog item, note which roles must deliver or review before work can progress (e.g., UX design before development begins; SRE sign-off before release).
2. **Document in the Risk Register:** Flag any dependency where another team's timeline is uncertain.
3. **Review at weekly sync:** Confirm dependency status and unblock or escalate as needed.
4. **Escalation path for dependency blockers:** Developer/role owner → Project Manager → affected team's lead → Sponsor (if blocking critical path).

Common cross-functional dependencies to watch:

| Dependency                            | Blocking Role          | Unblocked Role           |
|---------------------------------------|------------------------|--------------------------|
| UX designs for user-facing feature    | UX Designer            | Developers               |
| Metric/instrumentation requirements   | Data Analyst           | Developers               |
| Reliability sign-off for new services | SRE                    | Release Manager          |
| Support readiness for new features    | Customer Support Lead  | Release Manager / PM     |
| QA sign-off                           | QA/Testing             | Release Manager          |

---

## Communication Templates
Weekly Status Template:
- Progress this week:
- Next steps:
- Risks & blockers:
- Ask / decisions needed:

Incident Communication
- Triage summary
- Actions being taken
- Expected timeline
- Post-incident blameless retrospective scheduled

## Escalation Paths
- Team-level -> PM -> Product Lead -> Sponsor
- For security incidents, follow the security incident runbook and notify Security on-call
