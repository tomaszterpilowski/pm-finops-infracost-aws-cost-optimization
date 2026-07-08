# Project Charter

## Project Name

Run FinOps Practice: Infracost in Every Terraform PR + AWS Cost Optimization

## Project Type

DevOps / FinOps / AWS Cost Optimization / Cloud Governance

## Duration

9 months

## Problem Statement

The organization operated a growing AWS-based platform. Platform usage and traffic were increasing, but AWS spend was growing faster than expected. Engineering teams used Terraform and GitHub Pull Requests to manage infrastructure changes, but cost impact was not visible during infrastructure review.

This created a gap between engineering decisions and financial accountability. Cost was typically reviewed after deployment, when optimization was harder and ownership was less clear.

## Objective

Introduce cost visibility into the Terraform delivery lifecycle and establish a repeatable FinOps operating model for AWS spend governance.

## Goals

- Add estimated monthly cost impact to relevant Terraform Pull Requests.
- Build a shared cost governance model across Engineering, Finance and Product.
- Improve Savings Plans and Reserved Instances coverage.
- Reduce avoidable AWS spend while supporting platform growth.
- Establish monthly FinOps reviews and actionable dashboards.
- Create an optimization backlog with owners and measurable outcomes.

## Scope

### In Scope

- Terraform PR cost visibility
- Infracost integration
- GitHub / Atlantis review process alignment
- AWS Cost Explorer and Kubecost reporting inputs
- Savings Plans and RI review process
- KPI dashboard design
- monthly FinOps governance cadence
- optimization backlog and action tracking
- stakeholder communication and onboarding

### Out of Scope

- rewriting production Terraform modules
- redesigning the entire AWS landing zone
- migrating workloads between cloud providers
- exposing raw billing or sensitive account-level data
- implementing chargeback as a full finance operating model

## Success Criteria

| Success measure | Target / outcome |
|---|---:|
| relevant Terraform PRs include cost visibility | implemented |
| engineering teams onboarded | 6 teams |
| Terraform repositories covered | 14 repositories |
| Savings Plans + RI coverage | 82% |
| AWS spend reduction | $38K/month |
| monthly governance review | established |
| optimization backlog | active and owner-driven |

## Business Value

The project reduced monthly AWS spend from approximately **$173K/month** to **$135K/month**, delivering a run-rate improvement of approximately **$38K/month** while supporting continuous platform growth.

Beyond the savings, the project improved decision quality by making cost visible before merge and creating shared ownership between Engineering, Finance and Product.
