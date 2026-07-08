# Operational FinOps Dashboard

## Purpose

Operational dashboard used during monthly FinOps reviews with Cloud Engineering, DevOps, Platform Engineering and Finance stakeholders.

The dashboard tracks AWS cost governance, Terraform cost visibility adoption, commitment coverage and optimization execution.

---

# Executive Dashboard

../images/aws-finops-executive-dashboard.png

---

# Key Operational KPIs

| KPI | Current Value | Status |
|------|------:|------|
| Key Terraform Repositories | 14 | Operational |
| Engineering Teams Onboarded | 6 | Complete |
| AWS Accounts Covered | 8 | Complete |
| PR Cost Visibility | 95% | Operational |
| Savings Plans + RI Coverage | 82% | Optimized |
| Monthly Savings Run-Rate | $38K | Achieved |
| AWS Monthly Spend (Current) | $135K | Stable |
| AWS Monthly Spend (Baseline) | $173K | Historical |

---

# Program Scope

## Delivery Overview

| Area | Value |
|------|------:|
| Project Duration | 9 Months |
| Core Team Size | 9 People |
| Extended Stakeholders | ~24 |
| AWS Accounts | 8 |
| Engineering Teams | 6 |
| Key Terraform Repositories | 14 |

---

# PR Cost Visibility

## Adoption Metrics

| Metric | Value |
|------|------:|
| Key Terraform Repositories | 14 |
| Engineering Teams | 6 |
| AWS Accounts | 8 |
| Cost Visibility Coverage | 95% |
| Repositories Fully Onboarded | 14 |
| Remaining Exceptions | 5% |

## Cost Review Workflow

```text
Developer
    ↓
Terraform Change
    ↓
Pull Request
    ↓
Atlantis Plan
    ↓
Infracost Estimate
    ↓
Engineering Review
    ↓
Approve / Rework
    ↓
Deployment
```

---

# Optimization Backlog

| Category | Example Work Items | Priority |
|---|---|---|
| EKS Optimization | Node mix, workload efficiency, namespace visibility | High |
| Commitment Optimization | Savings Plans, RI coverage, expiry review | High |
| Rightsizing | RDS sizing, EC2 sizing, storage optimization | Medium |
| Waste Reduction | Idle resources, non-production schedules | Medium |
| Governance | Tagging standards, ownership mapping, dashboards | Medium |

---

# Commitment Coverage

## Current Coverage

| Metric | Value |
|---|---:|
| Savings Plans + RI Coverage | 82% |
| On-Demand Exposure | 18% |
| Coverage Status | Healthy |
| Review Frequency | Monthly |

### Coverage Summary

82% commitment coverage provides a balance between:

- Cost Optimization
- Operational Flexibility
- Growth Readiness
- Commitment Risk Management

Maintaining 100% commitment coverage is generally not recommended because development, burst and temporary workloads typically require a percentage of on-demand capacity.

---

# Monthly Savings Drivers

| Optimization Area | Monthly Impact |
|---|---:|
| Savings Plans + RI Optimization | $24K |
| Rightsizing & Resource Cleanup | $9K |
| Governance & Cost Visibility | $5K |
| **Total Savings** | **$38K** |

---

# Cost Reduction Results

| Metric | Before | After |
|---|---:|---:|
| AWS Monthly Spend | $173K | $135K |
| Monthly Savings | - | $38K |
| Annualized Savings | - | $456K |
| 3-Year Value Projection | - | $1.37M |
| PR Cost Visibility | 0% | 95% |
| SP / RI Coverage | Not Managed | 82% |

---

# Action Tracking

| Action | Owner | Status | Notes |
|---|---|---|---|
| Review Upcoming Commitment Expiry | FinOps + Cloud | Open | Monthly Governance Activity |
| Validate High-Cost Terraform PRs | Cloud + Reviewers | Active | Cost Review Workflow |
| Improve Tagging Coverage | DevOps + Application Owners | In Progress | Governance Backlog |
| Review EKS Cost Allocation | Cloud Engineering | Active | Kubecost Review |
| Monthly Savings Validation | Finance + FinOps | Active | Executive Reporting |

---

# Business Outcomes

✅ AWS Cost Governance Operational

✅ 14 Key Terraform Repositories Onboarded

✅ 95% PR Cost Visibility

✅ 82% Savings Plans + RI Coverage

✅ 6 Engineering Teams Enabled

✅ 8 AWS Accounts Governed

✅ $38K Monthly Savings Run-Rate

✅ $456K Annualized Savings

✅ Monthly FinOps Review Process Established

---

# Operational Status

**Status:** Green

The FinOps program is fully operational and integrated into the AWS infrastructure delivery process.

Key infrastructure changes are reviewed for cost impact before deployment, commitment coverage is actively managed, and optimization activities are tracked through recurring monthly governance reviews.

The program currently delivers approximately **$38K monthly savings**, maintains **82% Savings Plans + Reserved Instance coverage**, and provides **95% Terraform Pull Request cost visibility** across **14 key Terraform repositories**.
