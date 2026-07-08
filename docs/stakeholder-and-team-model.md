# Stakeholder and Team Model

## Overview

The project required coordination across technical and business teams. It was not enough to integrate Infracost technically. The organization also needed agreement on ownership, review behavior, dashboards, decision thresholds and operating cadence.

## Core Team

| Role | Count | Main responsibilities |
|---|---:|---|
| IT Project / Infrastructure Coordinator | 1 | program coordination, timeline, risks, reporting, stakeholder alignment |
| Cloud Engineers | 2 | AWS cost drivers, architecture optimization, rightsizing, SP / RI analysis |
| DevOps Engineers | 2 | GitHub, Atlantis, Terraform workflow, Infracost integration |
| FinOps / Finance Analyst | 1 | spend baseline, savings validation, KPI tracking |
| Product Owner | 1 | business prioritization, roadmap alignment, adoption support |
| Platform / Engineering Manager | 1 | team adoption, review standards, resource prioritization |
| Security / Compliance Representative | 1 | access control, data handling, anonymization, governance alignment |

## Extended Stakeholders

| Stakeholder group | Involvement |
|---|---|
| Application Owners | review service-level cost and approve workload trade-offs |
| Developers | respond to PR cost deltas and justify infrastructure changes |
| Engineering Leadership | sponsor adoption and remove blockers |
| Finance | validate savings and reporting methodology |
| Platform Operations | support operationalization and dashboards |
| Security / Compliance | ensure safe handling of cost and account data |

## Communication Model

| Forum | Frequency | Participants | Purpose |
|---|---|---|---|
| Delivery sync | weekly | core team | blockers, progress, planning |
| Technical implementation review | weekly / bi-weekly | DevOps, Cloud, Project Lead | workflow, rollout, issues |
| Monthly FinOps Review | monthly | Engineering, Finance, Product, PM | spend, KPIs, backlog, decisions |
| Executive update | monthly / milestone-based | sponsor, PM, leadership | value, risks, decisions |
| Adoption sessions | during rollout | engineering teams | explain PR process and expectations |

## Project Lead Focus

The Project Lead had to keep three viewpoints aligned:

1. **Engineering:** make the process practical and low-friction.
2. **Finance:** make savings measurable and credible.
3. **Product / Leadership:** show that cloud spend supports growth efficiently.
