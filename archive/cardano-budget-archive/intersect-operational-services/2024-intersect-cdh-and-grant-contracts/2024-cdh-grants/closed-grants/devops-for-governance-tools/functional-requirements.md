# Functional Requirements

{% include "../../../../../../../.gitbook/includes/this-page-has-been-archived.md" %}

## Context

### High-Level Description Of Services

To ensure the effective development, deployment, and maintenance of these governance tools, we need to handle:

* Cloud service
* Infrastructure
* Pipeline Configuration
* Orchestration and containerization
* Domain management
* Monitoring technology
* Networking configuration
* Security measures

### DevOps Strategy Highlights

DevOps Strategy focuses on optimizing development and deployment processes for a small team without a dedicated DevOps engineer. It emphasizes selecting well-tested, developer-friendly components to streamline operations, reduce operational costs, and enhance system flexibility. The strategy further defines adopting Docker containers for packaging, utilizing Docker Compose on the Hetzner cloud for small projects, and Kubernetes for more complex requirements in larger projects.

Furthermore, GitHub for code repository and GitHub Actions for CI/CD pipelines, coupled with GitHub Secrets for secret management, handling monitoring by an open-source stack of Grafana, Prometheus, and Loki for cost-effective and efficient observability.

The strategy also highlights the importance of documentation using GitHub Markdown pages and outlines an implementation plan that includes infrastructure setup, pipeline configuration, deployment strategies, and continuous monitoring and optimization.

## Description of required services

All services provided by the chosen supplier must be accompanied by testing results confirming that the requirements were fully implemented.\
The supplier will support two key streams of work:

* [Implementation of DevOps Strategy](functional-requirements.md#implementation-of-devops-strategy-requirements)
* [Maintenance of the Implemented DevOps Strategy](functional-requirements.md#maintenance-of-the-implemented-devops-strategy)
* Stakeholder Alignment:\
  Ensure alignment and understanding of DevOps goals among key stakeholders, including development, operations, and leadership teams.

The supplier must be operational within 4 weeks of the award date.

### Implementation of DevOps Strategy requirements

The following table describes a list of requirements with Milestones and Deliverables:

<table><thead><tr><th width="206">Milestone</th><th width="311.3333333333333">Description</th><th>Deliverables</th></tr></thead><tbody><tr><td>Milestones 1 - Infrastructure setup and configuration</td><td><p>Configure and setup both infrastructure systems for governace tools.</p><p><br><br></p><p>The Supplier shall provide and carry out the following:</p><p><br></p><ul><li>Terraform Setup for Hetzner Cloud:<br>Use Terraform to define infrastructure as code for provisioning resources on Hetzner Cloud. This includes setting up virtual machines, networks, and storage that will host the Kubernetes clusters.</li><li>Kubernetes Cluster Configuration<br>Configure Kubernetes clusters on Hetzner Cloud, either by using Hetzner's managed Kubernetes service or by manually setting up the clusters through Terraform scripts. Ensure the clusters are optimized for scalability and reliability.</li></ul><p>Milestone 1 - Acceptance Criteria:<br>Terraform IaC scripts are fully documented, tested, and security-compliant. All cloud resources meet specifications.<br>Kubernetes Clusters are set up with secure communication, and optimized resources. Integrate team repository permissions where only certain team members are allowed to trigger github actions.</p></td><td><ul><li>IaC scripts for provisioning resources on Hetzner Cloud.<br><br></li><li>Scripts cover provisioning of virtual machines, networks, and storage that will host the Kubernetes clusters.</li></ul></td></tr><tr><td>Milestone 2 - Continuous Integration and Continuous Deployment (CI/CD) Pipeline Setup</td><td><p>Setup CI/CD for governance tools.</p><p>The Supplier shall provide and carry out the following:</p><ul><li>i6GitHub Actions for CI:<br>Set up GitHub Actions workflows for Continuous Integration. This should automate code linting, testing, building Docker images, and pushing them to a container registry upon every commit or pull request.</li><li>GitHub Actions for CD:<br>Configure GitHub Actions for Continuous Deployment. Automate the deployment process so that successful builds are automatically deployed to Kubernetes clusters. This includes updating deployments with new Docker images, managing Kubernetes configurations, and handling secrets.</li></ul><p>Milestone 2 - Acceptance Criteria:<br>CI with GitHub Actions: Builds and tests are automated for every commit or PR, with clear reporting on failures.<br>CD with GitHub Actions: Automated deployments to environments are successful, with rollback mechanisms tested.</p></td><td><ul><li>Github Actions pipeline scripts with defined steps: lint, test, build, push-to-registry, deploy, release</li></ul></td></tr><tr><td>Milestone 3 - Deployment Strategies and Operations</td><td><p>Ensure full deployment and operational strategies for governance tools.</p><p>The Supplier shall provide and carry out the following:</p><ul><li>Implement Kubernetes Deployment Strategies:<br>Implement advanced Kubernetes deployment strategies, to help maintain service availability and minimize risks during updates.</li><li>Monitoring and Rollback Mechanisms:<br>Integrate Prometheus for performance metrics, Grafana for visualization, and Loki for log aggregation, to monitor application and infrastructure performance in real-time.<br>Implement automated rollback processes in the deployment workflows to revert to previous versions if issues are detected post-deployment.</li></ul><p>Milestone 3 - Acceptance Criteria:<br>Deployment Strategies are implemented, documented, and cause zero downtime in staging tests.<br>Critical KPIs are monitored with real-time alerts; rollback procedures are tested for minimal downtime.</p></td><td><p>- Deployed showcase project using the system</p><p>- Monitoring demo of deployed showcase project</p></td></tr><tr><td>Milestone 4 - Security and Compliance Integration</td><td><p>Ensure full setup and configuration of the secrets management and compliance integration for governance tools.</p><p>The Supplier shall provide and carry out the following:</p><ul><li>Secrets Management:<br>Implement GitHub Secrets for secure storage and management of sensitive data and configurations. Integrate Kubernetes Secrets to securely deploy these configurations with the applications.</li><li>Security Scanning:<br>Incorporate security scanning tools into the CI pipeline to perform automated vulnerability scanning of Docker images and Kubernetes configurations, ensuring security issues are identified and resolved early in the development lifecycle.</li></ul><p>Milestone 4 - Acceptance Criteria:<br>Secrets are securely managed and integrated without exposure in code or to unauthorized personnel.<br>Security scans are part of the CI pipeline, with a process for addressing findings and documented compliance.</p></td><td>- Deployed showcase project using the added security features</td></tr></tbody></table>

### Maintenance of the Implemented DevOps Strategy

The Supplier shall ensure regular maintenance and support of the cloud infrastructure, orchestration tooling, domain management, monitoring systems, and CI/CD processes established under this document. The

Supplier will provide 2 dedicated DevOps engineers for ongoing support and maintenance activities.

<table><thead><tr><th width="188">On going activities</th><th width="411">Description</th><th>Deliverables</th></tr></thead><tbody><tr><td>Maintenance - Monitoring, Optimization, and Continuous Improvement</td><td><ul><li>Optimize CI/CD Pipelines and Kubernetes Configurations:<br>Continuously review and optimize the CI/CD pipelines and Kubernetes configurations to improve efficiency, reduce deployment times, and ensure the infrastructure scales effectively with the application needs.</li><li>Comprehensive Monitoring:<br>Monitor with Prometheus, Grafana, and Loki to ensure comprehensive visibility into both the application and the underlying infrastructure.</li><li>Feedback Loops and Iteration:<br>Establish feedback loops with development teams to gather insights and feedback on the DevOps processes and tooling. Use this feedback to make iterative improvements to the DevOps strategy and implementation.</li><li>Regular maintenance and support of the cloud infrastructure, orchestration tooling, domain management, monitoring systems, and CI/CD processes done in Workstream 1. The Supplier will provide 2 dedicated DevOps engineers for ongoing support and maintenance activities.</li></ul></td><td><p>Comprehensive monitoring covers all critical aspects with actionable alerts and accessible dashboards.<br>CI/CD and Kubernetes show efficiency improvements, with a process for regular performance review.<br>A process for feedback collection and implementation is active, with documented improvements.</p><p><br></p></td></tr></tbody></table>

## Requirements for Third-Party Software

The Supplier undertakes to provide Customer a complete list of all software libraries, compilers, and other Third Party Software which will be incorporated into the Deliverables and a copy of all license agreements to which Customer or any of its affiliates is bound to for the use of any Third Party Software and, if not licensed, the basis on which such Third Party Software may be lawfully used by Customer or any of its Affiliates.
