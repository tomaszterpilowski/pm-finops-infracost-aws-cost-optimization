# Operational FinOps Dashboard

## Purpose

This dashboard is for the operational FinOps review with Cloud Engineering, DevOps and Finance stakeholders.

## Dashboard Sections

### PR Cost Visibility

| Metric | Target | Status |
|---|---:|---|
| relevant Terraform PRs with cost estimate | 100% | implemented |
| repositories onboarded | 14 | complete |
| engineering teams onboarded | 6 | complete |

### Optimization Backlog

| Category | Example work items |
|---|---|
| EKS optimization | node mix, workload efficiency, namespace cost visibility |
| Commitment optimization | SP / RI coverage, expiry review, forecast alignment |
| Rightsizing | RDS classes, compute sizing, storage review |
| Waste reduction | idle resources, non-production schedules |
| Governance | tagging, owners, dashboard mapping |

### Commitment Coverage

```text
Covered       | ################################# | 82%
Uncovered     | #######                           | 18%
```

### Action Tracking

| Action | Owner | Status | Notes |
|---|---|---|---|
| Review upcoming commitment expiry | FinOps + Cloud | Open | monthly action |
| Validate large PR deltas | Cloud + Reviewers | Active | handled in PR workflow |
| Improve missing tags | DevOps + App Owners | In progress | backlog-driven |
| Review EKS cost allocation | Cloud | Active | Kubecost input |
