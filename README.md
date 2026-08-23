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

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms

- **[Terraform Cloud / HCP Terraform](https://www.hashicorp.com/products/terraform)**  

  HashiCorp’s official managed platform for remote state, run orchestration, private registries, and team collaboration around Terraform.



- **[Spacelift](https://spacelift.io/)**  

  Multi-IaC orchestration platform supporting Terraform, OpenTofu, Terragrunt, Pulumi, CloudFormation, Kubernetes, and Ansible with strong policy-as-code and stack dependencies.



- **[Scalr](https://scalr.com/)**  

  Pure-play Terraform/OpenTofu TACO focused on governance, OPA policies, remote operations, and predictable per-run pricing.



- **[env0 (env zero)](https://www.env0.com/)**  

  Multi-IaC management platform with FinOps visibility, supporting Terraform, OpenTofu, Terragrunt, Pulumi, and more.



- **[Atlantis](https://www.runatlantis.io/)**  

  (Listed here for completeness; primarily open-source — see Open-Source section.) Self-hosted Terraform pull-request automation that many teams also run as a managed service pattern.



- **[Firefly](https://www.firefly.ai/)**  

  Cloud asset management and IaC platform that helps discover, codify, and manage infrastructure with Terraform-related workflows.



- **[Brainboard](https://www.brainboard.co/)**  

  Visual infrastructure-as-code design and automation platform that generates and manages Terraform.



- **[Massdriver](https://www.massdriver.cloud/)**  

  Platform engineering and infrastructure orchestration tool with Terraform support and developer self-service.



- **[Digger](https://digger.dev/)**  

  (Primarily open-source with optional cloud features — see Open-Source section.) IaC orchestration that runs Terraform/OpenTofu inside your existing CI.



- **[OpsLevel](https://www.opslevel.com/)**  

  Service catalog and platform engineering tool that often integrates with Terraform workflows for ownership and maturity tracking.



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
