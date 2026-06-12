# Network Change Management Framework
**City of Philadelphia – Office of Innovation and Technology**
*Technology Leadership Frameworks | [Candidate Name]*

---

## Purpose

This framework establishes the standards and processes for managing changes to network infrastructure in a controlled, documented, and risk-aware manner. Uncontrolled change is one of the leading causes of network outages and security incidents in enterprise environments.

Every change to production network infrastructure — regardless of perceived size — carries risk. This framework ensures that risk is assessed, communicated, and managed before any change is executed.

---

## Scope

| Domain | Included |
|---|---|
| Network hardware | Router, switch, firewall, wireless, and load balancer configuration changes |
| Circuit and connectivity | ISP circuit orders, BGP changes, SD-WAN policy changes |
| Access controls | Firewall rule additions, modifications, and deletions |
| IP and DNS | Subnet changes, VLAN additions, DNS record modifications |
| Software and firmware | Network device OS upgrades, patch application |
| Cloud and hybrid | Cloud gateway changes, VPN tunnel modifications |

---

## Change Classification

| Change Type | Definition | Approval Required |
|---|---|---|
| Standard | Pre-approved, low-risk, repeatable change with documented procedure | No CAB — follow standard procedure |
| Normal | Planned change requiring risk assessment and scheduled maintenance window | CAB approval required |
| Emergency | Unplanned change required to restore service or address critical security risk | DCNO approval; CAB review within 48 hours |

---

## Change Management Process

### Step 1 — Request and Documentation
- Submit change request with: description, business justification, scope, risk assessment, rollback plan, and proposed maintenance window
- Identify all systems and users potentially affected
- Confirm backup of current configuration before change window
- Attach test plan: how success will be verified after change

### Step 2 — Risk Assessment
- Assess change risk: Low / Medium / High based on scope, complexity, and potential impact
- High-risk changes require peer review by second network engineer before CAB submission
- All firewall rule changes require security team review regardless of risk level
- Changes affecting Tier 1 systems require DCNO review regardless of change type

### Step 3 — Change Advisory Board (CAB) Review
- CAB meets weekly for Normal changes
- Change request submitted minimum 48 hours before CAB meeting
- CAB membership: DCNO (chair), network engineering lead, security representative, operations representative
- CAB approves, defers, or rejects with documented rationale
- Emergency changes bypass CAB but require DCNO approval and post-change CAB review

### Step 4 — Execution
- Changes executed only during approved maintenance window
- Two-person rule for all P1-affecting changes: engineer executing + engineer monitoring
- Real-time documentation of all steps executed during change window
- Rollback executed immediately if change causes unintended impact
- Change owner responsible for monitoring for minimum 30 minutes post-change

### Step 5 — Post-Change Review
- Update configuration management database (CMDB) within 24 hours of successful change
- Close change ticket with: actual steps taken, outcome, and any deviations from plan
- Failed or rolled-back changes require root cause documentation before resubmission
- Monthly change success rate reported to technology leadership

---

## Maintenance Windows

| Window Type | Schedule | Applicable Changes |
|---|---|---|
| Standard maintenance window | Weekly — Sunday 10:00 PM to 2:00 AM | Normal changes |
| Extended maintenance window | Monthly — Saturday 8:00 PM to 4:00 AM | High-risk or major changes |
| Emergency window | As needed — DCNO authorization required | Emergency changes only |

---

## Rollback Standards

Every change request must include a documented rollback plan before approval. Rollback plans must include:

- Specific steps to restore previous configuration
- Estimated time to complete rollback
- Trigger criteria: what conditions require rollback execution
- Confirmation that rollback has been tested or validated in non-production environment where possible

---

## Key Deliverables

| Deliverable | Description |
|---|---|
| Change Request Record | Documented request, approval, execution, and outcome for every change |
| CAB Meeting Minutes | Weekly record of changes reviewed, approved, deferred, or rejected |
| Change Success Rate Report | Monthly metric: percentage of changes completed without incident |
| Failed Change Analysis | Root cause documentation for every failed or rolled-back change |
| Configuration Backup Log | Evidence of pre-change backups for all production device changes |

---

## Decision Criteria — When to Escalate

Escalate immediately when any of the following occur:

- Change causes P1 or P2 incident and rollback is not successful
- Emergency change implemented without DCNO authorization
- Configuration backup not available before a high-risk change is executed
- Change executed outside approved maintenance window without authorization
- Three or more failed changes from the same engineer or team within 30 days

---

## Framework Owner

**[Candidate Name]**
Deputy Chief Networking Officer (Candidate)
City of Philadelphia – Office of Innovation and Technology
