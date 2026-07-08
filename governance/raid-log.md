# RAID Log

## Risks

| ID | Risk | Impact | Probability | Mitigation | Owner | Status |
|---|---|---:|---:|---|---|---|
| R-01 | Engineering teams treat cost review as bureaucracy | High | Medium | lightweight PR-native process and onboarding | Project Lead | Managed |
| R-02 | Infracost output misunderstood as exact billing | Medium | Medium | training and documentation | DevOps / FinOps | Managed |
| R-03 | Missing tags reduce cost attribution quality | High | High | tagging standard and backlog items | Cloud Engineering | Managed |
| R-04 | Savings Plans overcommitment | High | Medium | monthly coverage and forecast review | FinOps / Cloud | Managed |
| R-05 | Workflow failures slow PR throughput | Medium | Medium | phased rollout and support process | DevOps | Managed |

## Assumptions

| ID | Assumption | Validation approach | Status |
|---|---|---|---|
| A-01 | Terraform PRs are the correct decision point | confirmed through workflow review | Validated |
| A-02 | majority of meaningful infra cost changes are represented in Terraform | repo inventory and team review | Validated |
| A-03 | stable workloads can support commitment optimization | spend and utilization analysis | Validated |
| A-04 | teams will adopt cost comments if low friction | pilot rollout | Validated |

## Issues

| ID | Issue | Impact | Action | Owner | Status |
|---|---|---:|---|---|---|
| I-01 | inconsistent resource tagging | High | define standard and remediation backlog | Cloud / DevOps | In progress |
| I-02 | unclear service ownership in some workloads | Medium | map application owners | Project Lead | Managed |
| I-03 | finance needed savings validation method | Medium | agree baseline and reporting method | FinOps | Closed |

## Dependencies

| ID | Dependency | Needed for | Owner | Status |
|---|---|---|---|---|
| D-01 | GitHub / Atlantis workflow access | PR cost integration | DevOps | Complete |
| D-02 | AWS billing visibility | baseline and reporting | FinOps | Complete |
| D-03 | Kubecost data | EKS cost visibility | Cloud Engineering | Complete |
| D-04 | engineering team availability | adoption and rollout | Engineering Manager | Complete |
