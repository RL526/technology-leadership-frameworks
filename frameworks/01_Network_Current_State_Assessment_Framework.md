# Network Current State Assessment Framework
**City of Philadelphia – Office of Innovation and Technology**
*Technology Leadership Frameworks | [Candidate Name]*

---

## Purpose

This framework provides a structured methodology for conducting a comprehensive assessment of the current network environment. It is designed to establish a documented baseline of infrastructure, operations, performance, and risk posture before any strategic transformation effort begins.

A current state assessment is the foundational input to all resiliency, availability, recovery, and buildout planning.

---

## Scope

| Domain | Included |
|---|---|
| Physical infrastructure | LAN, WAN, data centers, cabling, hardware inventory |
| Logical architecture | VLANs, routing, switching, DNS, DHCP, firewall zones |
| Cloud and hybrid connectivity | Cloud gateways, SD-WAN, VPN tunnels |
| Network security posture | Firewall rules, IDS/IPS, access controls, segmentation |
| Performance and capacity | Bandwidth utilization, latency, packet loss, throughput |
| Vendor and contract landscape | ISPs, hardware vendors, support contracts, EOL dates |

---

## Assessment Phases

### Phase 1 — Discovery and Inventory
- Collect all network diagrams (current and historical)
- Inventory all active hardware: routers, switches, firewalls, load balancers, wireless controllers
- Document all circuits: provider, bandwidth, contract expiration, SLA terms
- Identify all data center and closet locations with physical access controls
- Capture all IP address schemes, VLAN assignments, and subnet documentation

### Phase 2 — Architecture Review
- Map logical topology end-to-end
- Identify single points of failure
- Assess redundancy: core, distribution, and access layers
- Review WAN architecture: MPLS, SD-WAN, direct internet, hybrid
- Document DNS and DHCP infrastructure and management model
- Assess cloud connectivity: direct connect, VPN, peering

### Phase 3 — Security Posture Review
- Review firewall rule sets for bloat, conflicts, and shadow rules
- Assess network segmentation: flat network vs. tiered zones
- Identify unmanaged or rogue devices
- Review IDS/IPS coverage and alert tuning status
- Assess wireless security: encryption standards, guest isolation, rogue AP detection
- Document privileged access to network infrastructure

### Phase 4 — Performance and Capacity Baseline
- Pull 90-day utilization reports for all WAN circuits
- Identify top bandwidth consumers by application and user segment
- Document recurring outage or degradation incidents (prior 12 months)
- Review QoS policies and traffic prioritization
- Assess capacity headroom against projected growth

### Phase 5 — Vendor and Contract Landscape
- Compile all active network vendor relationships
- Document contract terms, renewal dates, and escalation paths
- Identify hardware at or near end-of-life (EOL) or end-of-support (EOS)
- Assess vendor concentration risk
- Review SLA compliance history

---

## Key Deliverables

| Deliverable | Description |
|---|---|
| Network Inventory Register | All hardware, circuits, and logical assets documented |
| Current State Architecture Diagram | Validated logical and physical topology |
| Risk and Gap Summary | Identified vulnerabilities, gaps, and single points of failure |
| Capacity Baseline Report | Utilization, headroom, and growth projections |
| Vendor Landscape Summary | Contracts, EOL exposure, and concentration risk |
| Executive Summary | 1–2 page leadership-facing summary of findings |

---

## Decision Criteria — When to Escalate

Escalate findings immediately when any of the following are identified:

- Active hardware with no vendor support path
- Flat network architecture with no segmentation between critical systems
- No redundancy on core or WAN connectivity
- Firewall rule sets not reviewed in more than 12 months
- Missing or outdated network diagrams for production environments
- Unmanaged devices on production segments

---

## Framework Owner

**[Candidate Name]**
Deputy Chief Networking Officer (Candidate)
City of Philadelphia – Office of Innovation and Technology
