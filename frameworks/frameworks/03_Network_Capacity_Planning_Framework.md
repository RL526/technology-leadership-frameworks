# Network Capacity Planning Framework
**City of Philadelphia – Office of Innovation and Technology**
*Technology Leadership Frameworks | [Candidate Name]*

---

## Purpose

This framework establishes a repeatable methodology for assessing current network capacity, forecasting future demand, and making data-driven investment decisions to ensure infrastructure keeps pace with operational and strategic requirements.

Capacity planning is a proactive discipline. Reactive capacity management produces outages, degraded performance, and unplanned capital expenditures.

---

## Scope

| Domain | Included |
|---|---|
| WAN and internet circuits | Bandwidth utilization, peak demand, growth trending |
| LAN and campus switching | Port utilization, uplink saturation, VLAN growth |
| Wireless infrastructure | AP density, client load, channel utilization |
| Data center interconnects | East-west traffic, storage replication, backup windows |
| Cloud and hybrid links | Egress/ingress volumes, burst capacity, cost exposure |
| DNS, DHCP, and IP addressing | Subnet exhaustion, lease pool utilization, IPv6 readiness |

---

## Capacity Planning Cycle

### Step 1 — Establish Baseline
- Pull 90-day utilization reports for all WAN circuits, core uplinks, and wireless controllers
- Document peak utilization windows (time of day, day of week, seasonal patterns)
- Identify top 10 bandwidth consumers by application, user group, and site
- Capture current IP address utilization by subnet and VLAN
- Document current licensed capacity for all network management platforms

### Step 2 — Analyze Trends
- Calculate month-over-month growth rate for all measured domains
- Identify circuits or segments approaching 70% sustained utilization (warning threshold)
- Identify circuits or segments at or above 85% sustained utilization (action threshold)
- Flag any subnet pools below 20% available addresses
- Review cloud egress cost trends for anomalies or unexpected growth

### Step 3 — Model Future Demand
- Apply known planned changes: new sites, agency consolidations, application migrations, hybrid work policy shifts
- Apply historical growth rate to project 12-month and 36-month demand
- Model best case, base case, and worst case scenarios for each critical domain
- Identify capacity cliff dates — the projected date a segment will hit 100% at current growth rate

### Step 4 — Develop Recommendations
- Prioritize upgrades by risk: capacity cliff date, criticality tier, and cost of failure
- Identify quick wins: configuration changes, QoS tuning, traffic shaping that defer capital spend
- Develop capital recommendations with cost estimates for circuits, hardware, and licensing
- Align recommendations to budget cycle and procurement lead times

### Step 5 — Report and Review
- Produce quarterly capacity report for technology leadership
- Produce annual capacity plan aligned to budget submission
- Review and update model assumptions after any major infrastructure or operational change

---

## Utilization Thresholds

| Threshold | Level | Required Action |
|---|---|---|
| Below 50% | Healthy | No action required — monitor quarterly |
| 50%–69% | Watch | Include in next planning cycle |
| 70%–84% | Warning | Initiate upgrade planning within 90 days |
| 85%–94% | Action Required | Begin procurement process immediately |
| 95%+ | Critical | Escalate — emergency capacity action required |

---

## Key Deliverables

| Deliverable | Description |
|---|---|
| Capacity Baseline Report | Current utilization across all measured domains |
| Growth Trend Analysis | Month-over-month trending with capacity cliff projections |
| 12-Month Demand Forecast | Projected demand by domain with scenario modeling |
| Capital Recommendation Summary | Prioritized upgrade list with cost estimates |
| Quarterly Capacity Dashboard | Ongoing monitoring report for leadership review |

---

## Decision Criteria — When to Escalate

Escalate immediately when any of the following are identified:

- Any Tier 1 circuit at or above 85% sustained utilization
- Any subnet pool below 20% available addresses serving critical systems
- Capacity cliff date within 6 months for any critical segment
- Cloud egress costs exceeding budget by more than 20% in any quarter
- Wireless client density causing sustained packet loss or association failures

---

## Framework Owner

**[Candidate Name]**
Deputy Chief Networking Officer (Candidate)
City of Philadelphia – Office of Innovation and Technology
