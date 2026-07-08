# Architecture

## Architecture Overview

The solution architecture embedded cost estimation into the infrastructure delivery workflow. The system did not replace Terraform, GitHub or Atlantis. It extended the existing workflow with cost visibility and governance.

## High-Level Architecture

```mermaid
flowchart LR
    subgraph Engineering[Engineering Delivery]
        DEV[Developer]
        TF[Terraform Change]
        PR[GitHub Pull Request]
        REVIEW[Engineering Review]
    end

    subgraph Automation[Automation Layer]
        ATL[Atlantis / Terraform Plan]
        IC[Infracost Estimate]
        COMMENT[PR Cost Comment]
    end

    subgraph AWS[AWS Platform]
        EKS[EKS Workloads]
        RDS[RDS]
        S3[S3]
        ALB[Load Balancer]
        CW[CloudWatch]
    end

    subgraph FinOps[FinOps Governance]
        CE[AWS Cost Explorer]
        KC[Kubecost]
        DASH[Dashboards]
        REVIEWMEET[Monthly FinOps Review]
        BACKLOG[Optimization Backlog]
    end

    DEV --> TF --> PR --> ATL --> IC --> COMMENT --> REVIEW
    REVIEW --> AWS
    AWS --> CE
    AWS --> KC
    CE --> DASH
    KC --> DASH
    DASH --> REVIEWMEET
    REVIEWMEET --> BACKLOG
    BACKLOG --> TF
```

## Terraform Pull Request Flow

```mermaid
sequenceDiagram
    participant Dev as Developer
    participant PR as GitHub Pull Request
    participant AT as Atlantis / Terraform
    participant IC as Infracost
    participant Rev as Reviewer

    Dev->>PR: Create infrastructure change
    PR->>AT: Trigger Terraform plan
    AT-->>PR: Return planned infrastructure delta
    PR->>IC: Generate cost estimate
    IC-->>PR: Publish monthly cost delta comment
    Rev->>PR: Review technical and cost impact
    Rev-->>PR: Approve or request changes
```

## Architecture Layers

### Engineering Delivery Layer

- developers
- cloud engineers
- Terraform changes
- GitHub Pull Requests
- code review and approvals

### Automation Layer

- Atlantis / Terraform plan
- Infracost estimate
- PR cost comment

### AWS Platform Layer

- EKS / ECS workloads
- RDS databases
- S3 storage
- Application Load Balancers
- CloudWatch metrics and logs
- IAM roles and policies

### FinOps Governance Layer

- AWS Cost Explorer
- Kubecost
- dashboards
- monthly FinOps review
- optimization backlog

## Why This Architecture Worked

The architecture worked because it did not create a detached governance system. Cost visibility was added to the existing engineering workflow, directly at the decision point.
