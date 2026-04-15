# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared

## Release Role Matrix

The table below shows each role's responsibilities during the release process:

| Role                  | Pre-Release Responsibility                                          | During Release                     | Post-Release                          |
|-----------------------|---------------------------------------------------------------------|------------------------------------|---------------------------------------|
| Release Manager       | Owns release plan, schedule, and go/no-go decision                 | Coordinates deployment activities  | Sends release summary to stakeholders |
| Developers            | Complete all PRs, resolve review feedback, support release testing  | On-call for hotfixes               | Monitor for release-related defects   |
| QA/Testing            | Execute final test pass; sign off on acceptance criteria            | Run smoke tests post-deploy        | Validate critical flows in production |
| Site Reliability Eng. | Confirm monitoring, alerting, and rollback procedures are in place  | Monitor deployment health          | Own post-deploy system health review  |
| Customer Support Lead | Review release notes; prepare support team for new features        | Available for urgent escalations   | Gather initial customer feedback      |
| Product Manager       | Approve release scope and feature readiness                         | Informed of deployment status      | Review success metrics post-launch    |
| Project Manager       | Confirm all release gates are met; communicate timeline            | Stakeholder communication          | Coordinate post-release retrospective |

## Pre-Release Readiness Checklist (All Personas)

- [ ] **Release Manager:** Release plan confirmed, deployment window scheduled, stakeholders notified
- [ ] **Developers:** All PRs merged, no blocking defects, on-call schedule confirmed
- [ ] **QA/Testing:** All acceptance criteria signed off, smoke test scripts ready
- [ ] **SRE:** Monitoring dashboards active, alerting thresholds set, rollback procedure documented
- [ ] **Customer Support Lead:** Support team briefed on new features, FAQs and known issues documented
- [ ] **Product Manager:** Feature scope confirmed, release notes reviewed and approved
- [ ] **Project Manager:** All go/no-go criteria confirmed, final release communication drafted

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
