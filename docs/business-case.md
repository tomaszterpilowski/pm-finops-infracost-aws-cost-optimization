# Business Case

## Executive Summary

The AWS platform was growing, but cloud spend was increasing faster than the organization wanted. The technical delivery model was already based on Terraform and Pull Requests, but financial impact was not part of the normal infrastructure review process.

The business case for the project was to reduce avoidable AWS cost growth by moving cost visibility earlier in the delivery lifecycle.

## Baseline

| Metric | Baseline |
|---|---:|
| AWS monthly spend | $173K/month |
| Traffic growth | +35% YoY |
| Cost growth | +28% YoY |
| Cost visibility in PRs | not standardized |
| Commitment coverage | inconsistent / reactive |
| Monthly FinOps governance | not formalized |

## Business Drivers

### Cloud spend was attracting leadership attention

AWS costs were material enough to require clearer governance, especially because the platform was expected to continue growing.

### Engineering decisions lacked financial context

Infrastructure decisions were reviewed for correctness, reliability and security, but cost impact was not always visible at the point of approval.

### Finance and Engineering needed a shared operating model

Finance could report spend after the fact, but Engineering owned many of the design and deployment decisions that created that spend.

### Commitment optimization needed discipline

Savings Plans and Reserved Instances can reduce cost only when matched to stable usage and reviewed continuously.

## Expected Benefits

| Benefit | Description |
|---|---|
| Cost transparency | reviewers see cost impact before merge |
| Better governance | cloud cost becomes part of delivery control |
| Reduced waste | optimization opportunities are tracked and assigned |
| Improved commitments | SP / RI coverage managed through recurring review |
| Stronger ownership | Engineering, Product and Finance operate from the same data |
| Executive confidence | leadership receives clearer cost and value reporting |

## Realized Benefits

| Metric | Result |
|---|---:|
| AWS spend reduction | $38K/month |
| Monthly run-rate after optimization | $135K/month |
| Savings Plans + RI coverage | 82% |
| Time to first visible savings | 3 months |
| Time to full measured run-rate impact | 6 months |
| Engineering teams onboarded | 6 |
| Terraform repositories covered | 14 |

## Financial Statement

The program reduced AWS monthly spend from approximately **$173K/month** to approximately **$135K/month**. This represents a monthly run-rate improvement of approximately **$38K/month**.

The project also created a governance mechanism to reduce the probability of costs growing again without review.
