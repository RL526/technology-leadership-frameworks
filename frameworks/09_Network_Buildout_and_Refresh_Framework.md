# Network Buildout and Refresh Framework
**City of Philadelphia – Office of Innovation and Technology**
*Technology Leadership Frameworks | [Candidate Name]*

---

## Purpose

This framework defines the standards and processes for planning, executing, and documenting network infrastructure buildouts and technology refresh projects. Buildout and refresh work represents the highest-risk, highest-impact category of network change — requiring disciplined project governance, architectural standards enforcement, and post-deployment validation.

This framework applies to new site buildouts, major infrastructure upgrades, data center network refreshes, and end-of-life hardware replacement programs.

---

## Scope

| Project Type | Included |
|---|---|
| New site buildouts | Branch offices, community centers, public safety facilities |
| Data center network refresh | Core switching, spine-leaf upgrades, interconnect redesign |
| Campus network refresh | Distribution and access layer hardware replacement |
| Wireless refresh | Controller replacement, AP hardware refresh, design updates |
| WAN modernization | MPLS to SD-WAN migration, circuit upgrades, provider transitions |
| End-of-life replacement | Systematic replacement of EOL/EOS hardware by asset class |

---

## Project Phases

### Phase 1 — Planning and Design
- Define project scope, objectives, and success criteria
- Conduct current state assessment of impacted infrastructure
- Develop target state architecture aligned to OIT standards
- Identify all dependencies: power, cabling, space, licensing, and circuit orders
- Produce bill of materials (BOM) with vendor quotes
- Develop project schedule with milestones and resource assignments
- Obtain DCNO design approval before procurement

### Phase 2 — Procurement and Staging
- Submit procurement request aligned to City procurement policy
- Confirm delivery timeline against project schedule
- Stage and image all hardware before site deployment
- Validate firmware versions against approved baseline
- Complete factory acceptance testing (FAT) for major deployments
- Document staged configuration for each device before shipping

### Phase 3 — Deployment
- Deploy during approved maintenance window
- Follow site-specific deployment runbook developed in Phase 1
- Two-person rule for all core infrastructure deployment
- Document as-built configuration for every device installed
- Test all connections and services before declaring deployment complete
- Obtain site sign-off from agency technology liaison before closing deployment window

### Phase 4 — Validation and Cutover
- Execute post-deployment test plan: connectivity, performance, security controls
- Validate monitoring coverage: confirm all new devices appear in NOC dashboard
- Confirm backup of all as-built configurations to configuration management system
- Conduct user acceptance testing for business-critical applications at site
- Document any deviations from design and obtain DCNO approval for exceptions

### Phase 5 — Project Closure
- Update CMDB with all new assets, configurations, and circuit information
- Archive all project documentation: design, BOM, as-built, test results
- Conduct lessons learned review for all projects over 90 days in duration
- Submit final project report to DCNO and CIO office
- Schedule 30-day and 90-day post-deployment health checks

---

## Architecture Standards

All buildout and refresh projects must comply with:

- Approved hardware vendor list — no unapproved hardware in production
- Standard VLAN and IP addressing schema
- Redundancy requirements by site tier (reference Framework 02)
- Security segmentation standards (reference Framework 04)
- Monitoring integration requirements (reference Framework 08)
- Configuration backup requirements before and after every deployment

---

## Key Deliverables

| Deliverable | Description |
|---|---|
| Design Document | Target state architecture with diagrams, BOM, and technical specifications |
| Deployment Runbook | Step-by-step deployment procedures for each site or project phase |
| As-Built Documentation | Final documented configuration for every device deployed |
| Post-Deployment Test Results | Documented validation of connectivity, performance, and security |
| Project Closure Report | Final summary of scope, schedule, budget, and lessons learned |

---

## Decision Criteria — When to Escalate

Escalate immediately when any of the following occur:

- Deployment causes unplanned outage to Tier 1 services
- Hardware delivered does not match approved BOM or fails staging validation
- Design deviation identified during deployment that cannot be resolved within maintenance window
- Project schedule slips more than 30 days without approved change to project plan
- Vendor unable to deliver hardware within 60 days of procurement for a critical path item

---

## Framework Owner

**[Candidate Name]**
Deputy Chief Networking Officer (Candidate)
City of Philadelphia – Office of Innovation and Technology
