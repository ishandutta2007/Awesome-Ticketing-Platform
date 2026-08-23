# Awesome-Ticketing-Platform

## Top Terraform Automation Platforms Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Terraform / OpenTofu Orchestration, PR Automation, Policy-as-Code, Remote State, Drift Detection & IaC Collaboration (TACOs)*

**Last updated: August 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Terraform Automation** (often called TACOs – Terraform Automation and Collaboration Software). These tools orchestrate Terraform/OpenTofu runs, provide pull-request automation, policy enforcement, remote state management, drift detection, and team collaboration around infrastructure as code.



**Examples** include Terraform Cloud, Spacelift, Scalr, env0, Atlantis, Firefly, Brainboard, Massdriver, Digger, and OpsLevel (the category leaders and notable players).



**Open-source emphasis**: The open-source side is strong, led by **Atlantis** (the classic PR automation tool) and **Digger** (CI-native orchestration). This section is heavily expanded with these and related projects that let teams run Terraform automation without proprietary lock-in.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saashosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms

| Platform | Description | Starting Pricing | Free Tier Limits |
| :--- | :--- | :--- | :--- |
| **[Terraform Cloud / HCP Terraform](https://www.hashicorp.com/products/terraform)** | HashiCorp’s official managed platform for remote state, run orchestration, private registries, and team collaboration around Terraform. | Starts at **$0.10 / managed resource / month** (Essentials tier; Standard tier at $0.47 / resource / month) | **Free forever** for up to 500 managed resources, 1 concurrent run, unlimited users, and 1 policy set (up to 5 policies); includes $500 HCP trial credits for paid tiers. |
| **[Spacelift](https://spacelift.io/)** | Multi-IaC orchestration platform supporting Terraform, OpenTofu, Terragrunt, Pulumi, CloudFormation, Kubernetes, and Ansible with strong policy-as-code and stack dependencies. | Starts at **$20,000 / year** (Starter+ tier billed annually) | **Free forever** for up to 2 users and 1 public worker (1 concurrent run); 14-day free trial on paid features. |
| **[Scalr](https://scalr.com/)** | Pure-play Terraform/OpenTofu TACO focused on governance, OPA policies, remote operations, and predictable per-run pricing. | Starts at **$0.99 / run** (or **$99 / month** for 100 prepaid runs package) | **Free forever** for up to 50 runs/month, 5 concurrent runs, unlimited users, workspaces, and resources under management. |
| **[env0 (env zero)](https://www.env0.com/)** | Multi-IaC management platform with FinOps visibility, supporting Terraform, OpenTofu, Terragrunt, Pulumi, and more. | Starts at **$1,500 / month** (Cloud Compass tier) | **Free forever** for up to 250 runs/month and 30 active environments; 14-day free trial available for advanced features. |
| **[Atlantis](https://www.runatlantis.io/)** | Self-hosted Terraform pull-request automation that many teams run as a managed service pattern (primarily open-source — see Open-Source section). | **Free** (Open-Source / Self-Hosted) | **Free forever** (100% open-source under Apache 2.0; unlimited users, runs, and resources; self-hosted compute costs apply). |
| **[Firefly](https://www.firefly.ai/)** | Cloud asset management and IaC platform that helps discover, codify, and manage infrastructure with Terraform-related workflows. | Starts at **$2,499 / month** (Essential tier via AWS Marketplace, billed annually) | **Free forever** for up to 500 managed cloud resources / assets; 14-day free trial available for paid tiers. |
| **[Brainboard](https://www.brainboard.co/)** | Visual infrastructure-as-code design and automation platform that generates and manages Terraform. | Starts at **$99 / user / month** (Pro plan) | **Free forever** for individual use (unlimited cloud architectures and Terraform code generation); 21-day free trial for Pro features. |
| **[Massdriver](https://www.massdriver.cloud/)** | Platform engineering and infrastructure orchestration tool with Terraform support and developer self-service. | Starts at **$999 / month for 15 seats** (Business tier billed annually) | **14 to 30-day free trial** with full platform and POC access (no permanent free tier). |
| **[Digger](https://digger.dev/)** | IaC orchestration that runs Terraform/OpenTofu inside your existing CI (GitHub Actions, GitLab CI, etc.). | Starts at **$49 / user / month** (Digger Pro / OpenTaco, min. 5 seats; Enterprise from $3,000 / month) | **Free forever Community Edition** (100% open-source, runs in your CI with unlimited runs/resources); 14-day free trial for Pro. |
| **[OpsLevel](https://www.opslevel.com/)** | Service catalog and platform engineering tool that often integrates with Terraform workflows for ownership and maturity tracking. | Starts at **$10,000 / year** (~$833 / month for up to 20 users / ~$25–$45 / developer / month) | **14 to 30-day free trial** / POC with full catalog and check integration access (no permanent free tier). |



## Open-Source GitHub Projects

- **[Atlantis](https://github.com/runatlantis/atlantis)**  

  The classic open-source Terraform Pull Request Automation tool. Listens for VCS webhooks, runs plan/apply, and comments results back on PRs. Apache-2.0, widely adopted and self-hosted.



- **[Digger (OpenTaco)](https://github.com/diggerhq/digger)**  

  Open-source IaC orchestration that runs Terraform/OpenTofu natively inside your existing CI pipeline (GitHub Actions, GitLab CI, etc.). No extra compute or third-party secrets required; supports drift detection, policies, and more.



- **[Terrateam](https://github.com/)**  

  Open-source self-hosted Terraform/OpenTofu PR automation with strong Terragrunt support and additional IaC engines.



- **[OpenTofu](https://github.com/opentofu/opentofu)**  

  Community-driven open-source fork of Terraform that many automation platforms now support natively as a drop-in engine.



- **[Terragrunt](https://github.com/gruntwork-io/terragrunt)**  

  Thin wrapper for Terraform/OpenTofu that provides extra tools for keeping configurations DRY, often used with Atlantis or Digger.



- **[tf-controller / Flux Terraform Controller](https://github.com/)**  

  Kubernetes-native controllers for managing Terraform resources in a GitOps style.



- **[Infracost](https://github.com/infracost/infracost)**  

  Open-source tool that shows cloud cost estimates for Terraform plans directly in pull requests.



- **[Checkov / tfsec / Terrascan](https://github.com/)**  

  Open-source static analysis and policy-as-code scanners for Terraform that integrate into CI and automation platforms.



- **[OPA / Conftest](https://github.com/open-policy-agent)**  

  Open Policy Agent and related tools widely used for policy-as-code enforcement in Terraform workflows.



- **[Terraform modules and Atlantis deployment examples](https://github.com/terraform-aws-modules/terraform-aws-atlantis)**  

  Ready-to-use Terraform modules and community patterns for deploying Atlantis itself on cloud infrastructure.



### Additional Strong Open-Source Options

- Custom GitHub Actions / GitLab CI templates for plan/apply with locking and commenting.

- Drift detection scripts and scheduled pipelines.

- Private module registry implementations (e.g., using Git or Artifactory).

- State backend helpers and migration tools.

- Multi-account / multi-environment orchestration wrappers.



**Frameworks for building custom systems**: For most teams the combination of **Atlantis** or **Digger** + **OpenTofu/Terraform** + **OPA/Checkov** + your existing CI runners provides a complete, fully open-source automation stack. Run plans and applies from pull requests, enforce policies, detect drift on a schedule, and keep all secrets and state inside your own infrastructure. This approach eliminates per-run or per-resource SaaS fees while retaining full control and auditability.



## How to Contribute

1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.

- Terraform automation platforms execute infrastructure changes that can affect production systems and incur cloud costs. Open-source tools give excellent transparency and cost control but still require proper secret management, state locking, policy design, and operational safeguards.

- Always test workflows thoroughly and follow least-privilege principles for cloud credentials used by automation.



---

**Made for platform engineers, SREs, and DevOps teams who want flexible, auditable Infrastructure-as-Code automation.**

Let's make Terraform and OpenTofu workflows more open, secure, and under your control.
