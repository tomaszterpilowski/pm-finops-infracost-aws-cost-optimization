# Operational FinOps Dashboard

## Purpose

Operational dashboard used during monthly FinOps reviews with Cloud Engineering, DevOps, Platform and Finance stakeholders.

The dashboard tracks AWS spend governance, Terraform cost visibility adoption, commitment coverage and optimization execution.

---

## Key Operational KPIs

| KPI | Current Value | Status |
|------|------:|------|
| Key Terraform Repositories | 14 | Active |
| Engineering Teams Onboarded | 6 | Complete |
| AWS Accounts Covered | 8 | Complete |
| PR Cost Visibility | 95% | Operational |
| Savings Plans + RI Coverage | 82% | Optimized |
| Monthly Savings Run-Rate | $38K | Achieved |

---

## PR Cost Visibility

### Adoption Metrics

| Metric | Value |
|---|---:|
| Key Terraform Repositories | 14 |
| Engineering Teams | 6 |
| AWS Accounts | 8 |
| PR Cost Visibility | 95% |
| Repositories Fully Onboarded | 14 |
| Remaining Manual Exceptions | 5% |

### Process Flow

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
Approval / Rework
   ↓
Deployment
