# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

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

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register reviewed and updated weekly with team
- [ ] Stakeholder reviews scheduled at key milestones
- [ ] Cross-functional dependencies tracked and updated
- [ ] Test coverage monitored and maintained
- [ ] Security scans reviewed and vulnerabilities addressed

## New Contributor Onboarding Checklist

Use this checklist to help new team members get up to speed quickly:

### Access & Setup
- [ ] Repository access granted (read/write permissions)
- [ ] CI/CD access and credentials configured
- [ ] Development environment set up and verified
- [ ] Communication channels added (Slack, Teams, email lists)
- [ ] Project board and tracking tool access granted

### Artifact Review
- [ ] Review project one-pager and goals
- [ ] Read through current sprint/iteration backlog
- [ ] Review risk register and active dependencies
- [ ] Familiarize with Definition of Done (DoD)
- [ ] Review recent retrospective notes and action items
- [ ] Read through release notes from last 2-3 releases

### Communication & Integration
- [ ] Attend team standup and introduction
- [ ] Schedule 1:1s with PM, Product Lead, and key team members
- [ ] Review communication cadence (standups, syncs, demos)
- [ ] Understand escalation paths and who to contact for questions
- [ ] Join relevant meetings and accept recurring invites

### First Contributions
- [ ] Complete a small, well-defined task to familiarize with workflows
- [ ] Submit first PR following team conventions
- [ ] Participate in code review (review someone else's PR)
- [ ] Ask questions and request clarifications as needed
