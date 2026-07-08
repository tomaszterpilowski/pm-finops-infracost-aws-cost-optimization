# Decision Log

## DEC-001 — Use PR-based FinOps control

**Decision:** Use the existing GitHub Pull Request process as the cost governance point.

**Reason:** Engineers already reviewed infrastructure changes in PRs. Adding cost visibility there minimized process friction.

**Impact:** Cost became visible before merge without introducing a separate approval workflow.

## DEC-002 — Integrate Infracost with Terraform workflow

**Decision:** Use Infracost to provide estimated monthly cost impact for Terraform changes.

**Reason:** The project needed a practical way to show cost delta before deployment.

**Impact:** Reviewers could see before / after cost estimates and monthly delta.

## DEC-003 — Keep estimates directional, not invoice-accurate

**Decision:** Treat PR cost estimates as decision support, not exact billing truth.

**Reason:** Early estimates are useful for review, but final billing depends on real usage, discounts and runtime behavior.

## DEC-004 — Manage Savings Plans and RI coverage monthly

**Decision:** Add recurring review of commitment coverage to the monthly FinOps cadence.

**Reason:** Commitment coverage changes as workloads grow, shrink or move.

**Impact:** Coverage reached 82% while keeping overcommitment risk visible.

## DEC-005 — Track optimization as backlog work

**Decision:** Convert FinOps recommendations into backlog items with owner, priority, impact and status.

**Reason:** Recommendations without owners often do not result in implementation.
