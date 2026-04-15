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

## UX Designer

### Role Summary
Designs user interfaces and user experiences, ensuring solutions are user-centric, accessible, and aligned with product goals.

### Responsibilities
- Collaborate with Product Managers and Developers on UI/UX design
- Advocate for user needs in design decisions and trade-offs
- Review prototypes and gather user feedback iteratively
- Ensure design consistency and accessibility across projects
- Participate in design reviews and acceptance criteria validation

### Goals
- Improve usability and accessibility of products
- Integrate user feedback into iterative improvements
- Reduce design-related rework through early collaboration

### Typical Communication
- Design review sessions with PM, PdM, and Dev
- User feedback discussions in planning and retrospectives
- Share design prototypes, wireframes, and rationale
- Participate in sprint planning and demo sessions

---

## Release Manager

### Role Summary
Plans, schedules, coordinates, and communicates production releases to all stakeholders, reducing risk and ensuring predictable delivery.

### Responsibilities
- Prepare release plans and coordination schedules
- Coordinate with QA, Developers, and PMs for release readiness
- Monitor release activities and manage rollback procedures
- Document release notes and communicate with stakeholders
- Capture lessons learned post-release and drive continuous improvement

### Goals
- Deliver predictable, low-risk releases
- Ensure post-release stability and user communication
- Reduce release-related incidents and rollbacks

### Typical Communication
- Pre- and post-release syncs with PM, QA, Dev
- Stakeholder updates (timing, scope, risks)
- Release summary emails and incident post-mortems
- Coordination via project boards and release checklists

---

## Data Analyst

### Role Summary
Defines and analyzes quantitative project metrics and KPIs, enabling data-informed prioritization and continuous improvement.

### Responsibilities
- Develop and report on usage, impact, and performance metrics
- Support PM/PdM with analytics for decision making and backlog prioritization
- Automate collection and visualization of periodic data
- Partner with Product Managers to validate success criteria

### Goals
- Increase transparency into value delivery and product performance
- Support evidence-based prioritization and improvements
- Enable rapid iteration through data visibility

### Typical Communication
- Share regular dashboard updates and metric reviews
- Join metric review meetings and planning sessions
- Present findings to support product decisions
- Collaborate with Developers on telemetry and instrumentation

---

## Site Reliability Engineer (SRE)

### Role Summary
Monitors system reliability, scalability, and performance, collaborating with the broader technical team to ensure robust delivery and rapid incident response.

### Responsibilities
- Monitor key system indicators, uptime, and performance metrics
- Lead on-call incident response and drive root-cause analysis
- Collaborate with Developers on reliability improvements and automation
- Contribute to release readiness and post-deployment verification
- Document incident playbooks and runbooks

### Goals
- Achieve targeted uptime and reliability metrics
- Reduce MTTR (Mean Time to Repair) for incidents
- Improve system observability and prevent future incidents

### Typical Communication
- Post-incident reviews with Dev and PM teams
- System health reporting and metrics sharing
- Joint planning with Dev team for reliability improvements
- Participate in release and deployment coordination

---

## Customer Support Lead

### Role Summary
Champions feedback from users and support staff in backlog prioritization and release planning, ensuring customer success.

### Responsibilities
- Surface critical support issues and trends for prioritization
- Maintain close communication with PM and Product Manager pre-release
- Ensure support readiness and training for new features and releases
- Gather and synthesize customer feedback for product decisions
- Participate in planning and retrospectives to capture customer perspective

### Goals
- Reduce recurring support incidents and improve issue resolution
- Improve customer satisfaction and reduce support overhead
- Ensure customer success with new features through proactive support

### Typical Communication
- Weekly sync with product and project managers
- Summary reports of top user issues and trends
- Participate in sprint planning and release planning sessions
- Customer feedback presentation to PM and Developers

---

## Role Interaction Guide

The following roles interact in key ways throughout the project lifecycle:

### Core Cross-Functional Loop
- **PM/PdM + Developers + Testers:** define requirements, implement, and validate quality
- **Release Manager + QA + Developers:** coordinate pre-release readiness and deploy
- **SRE + Developers:** monitor post-release health and respond to incidents

### Support & Feedback Loop
- **Customer Support Lead + PM/PdM:** surface customer issues for prioritization
- **Data Analyst + PM/PdM:** provide metrics to support decision making
- **UX Designer + PM/PdM + Developers:** iterate on user experience based on feedback

### Planning & Execution
- **Project Manager:** coordinates all roles through planning, execution, and retrospectives
- **All roles:** participate in standups, planning, demos, and retrospectives

---

## Role Collaboration Matrix by Project Phase

The table below shows which roles are actively engaged at each phase of the project lifecycle. **R** = Responsible, **C** = Consulted, **I** = Informed.

| Role                  | Initiation | Planning | Execution | Release | Close & Retro |
|-----------------------|:----------:|:--------:|:---------:|:-------:|:-------------:|
| Project Manager       | R          | R        | R         | R       | R             |
| Product Manager       | R          | R        | C         | C       | C             |
| Developers            | C          | R        | R         | R       | C             |
| QA/Testing            | I          | C        | R         | R       | C             |
| UX Designer           | C          | R        | R         | I       | C             |
| Release Manager       | I          | C        | C         | R       | C             |
| Data Analyst          | C          | R        | C         | I       | R             |
| Site Reliability Eng. | I          | C        | C         | R       | C             |
| Customer Support Lead | C          | C        | I         | C       | R             |

---

## Role Collaboration Checklist

Use this checklist at each critical project gate to ensure all key personas are involved at the right time.

### Initiation Gate
- [ ] Project Manager has been assigned and has reviewed the project charter
- [ ] Product Manager has defined the problem statement and success metrics
- [ ] Data Analyst has been consulted on metric definition and measurement approach
- [ ] UX Designer has been informed of scope and user experience considerations
- [ ] Customer Support Lead has been consulted on known customer pain points

### Planning Gate
- [ ] All relevant roles have attended the kickoff meeting
- [ ] UX Designer has provided wireframes or design input for user-facing work
- [ ] Data Analyst has confirmed instrumentation and tracking requirements
- [ ] Release Manager has reviewed the release plan and timeline
- [ ] SRE has been consulted on reliability, scalability, and observability requirements

### Execution Gate (mid-sprint check)
- [ ] Developers have flagged any technical blockers to the Project Manager
- [ ] QA has a clear test plan aligned with acceptance criteria
- [ ] UX Designer has reviewed in-progress UI changes
- [ ] Data Analyst has confirmed telemetry is being implemented correctly

### Release Gate
- [ ] Release Manager has confirmed the deployment window and release plan
- [ ] SRE has verified monitoring and alerting are in place
- [ ] Customer Support Lead has been briefed on new features and potential support needs
- [ ] QA has signed off on all acceptance criteria

### Close & Retrospective Gate
- [ ] Data Analyst has presented post-release metrics
- [ ] Customer Support Lead has shared initial customer feedback
- [ ] All roles have contributed retrospective input
- [ ] Action items have been assigned to owners across roles

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- Reference the Role Interaction Guide and Role Collaboration Matrix to understand how personas collaborate across project phases.