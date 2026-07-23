<p>
  <a href="https://avisi.cloud/">
    <img src="./img/ame-robot.svg" alt="Avisi Managed Environments robot" width="150">
  </a>
</p>

<h1>Avisi Managed Environments</h1>

<p>
  <strong>Managed Kubernetes with automated operations and built-in observability.</strong>
</p>

<p>
  Run mission-critical applications on supported public, private and hybrid
  infrastructure while Avisi Cloud manages the Kubernetes platform.
</p>

<p>
  <a href="https://avisi.cloud/features"><strong>Explore Features</strong></a> ·
  <a href="https://docs.avisi.cloud/docs/product/overview/introduction"><strong>Read the Documentation</strong></a> ·
  <a href="https://console.avisi.cloud/"><strong>Start a Trial</strong></a> ·
  <a href="https://status.avisi.cloud/"><strong>Platform Status</strong></a>
</p>

---

## What is AME?

**Avisi Managed Environments (AME)** is a managed Kubernetes platform. It provides the infrastructure,
Kubernetes control plane, managed components and support needed to run
production workloads safely and reliably.

AME maintains a consistent Kubernetes experience across supported cloud
providers. Your teams keep Kubernetes access and application portability while
Avisi Cloud operates platform components, validates upgrades and maintains
managed add-ons.

## Platform capabilities

| Area                       | Capabilities                                                                                                     |
| -------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| **Cluster lifecycle**      | Automated provisioning, defined Kubernetes release channels, maintenance windows and flexible upgrade strategies |
| **Compute**                | Multiple node pools, node auto-healing, autoscaling and workload-specific configuration                          |
| **Access and audit**       | Organisations, environments, OIDC-based SSO, role-based access and audit logs                                    |
| **Networking and storage** | Managed networking, load balancers, ingress, persistent storage and volume snapshots where supported             |
| **Day-2 operations**       | Managed add-ons, events, alerts, runbooks, backup workflows and operational automation                           |
| **Developer interfaces**   | Web console, `acloud` CLI, Go client, REST API and Terraform provider                                            |

The [AME feature overview](https://avisi.cloud/features) describes the current
platform capabilities. Stability and provider-specific support can change, so
the [product documentation](https://docs.avisi.cloud/docs/product/overview/features-quickview)
remains the source of truth.

## Managed Observability

Observability is included within AME. Clusters receive an integrated stack for
collecting, retaining and acting on operational signals without requiring
individual teams to build and maintain the platform themselves.

| Component        | Role in AME                                                                     |
| ---------------- | ------------------------------------------------------------------------------- |
| **Prometheus**   | Collects Kubernetes and application metrics using standard Prometheus resources |
| **Cortex**       | Provides scalable, highly available long-term metrics storage                   |
| **Loki**         | Collects and stores cluster log events                                          |
| **Grafana**      | Visualizes metrics and logs using familiar open tooling                         |
| **Alertmanager** | Routes alerts to services such as Slack, Opsgenie and custom webhooks           |

Metrics, logs, alerts and relevant cluster activity are available through the
AME Console. Long-term data remains accessible independently of an individual
cluster's availability.

<details>
<summary><strong>Observability integration details</strong></summary>

- Prometheus Operator support enables standard `ServiceMonitor` and
  `PodMonitor` resources.
- Baseline node and pod metrics are collected automatically.
- Prometheus alerts can be viewed and silenced through supported AME
  interfaces.
- Loki forwards cluster log events to the managed logging stack.
- Alertmanager configuration can route actionable alerts to external systems.
- Audit information provides additional visibility into cluster and platform
  activity.

</details>

[Read the Observability documentation](https://docs.avisi.cloud/docs/product/overview/observability)

## One operating model across clouds

AME supports public-cloud and private-infrastructure deployments through a
consistent API and Kubernetes experience.

| Provider or infrastructure | Documented availability |
| -------------------------- | ----------------------- |
| Amazon Web Services (AWS)  | Supported               |
| Azure                      | Beta                    |
| Hetzner                    | Supported               |
| Leafcloud                  | Supported               |
| OpenStack                  | Supported               |
| VMware vSphere             | Supported               |

Provider features and regional availability differ. Check the
[current product overview](https://docs.avisi.cloud/docs/product/overview/introduction)
before selecting an infrastructure target.

## Automation for platform engineers

<details open>
<summary><strong>Console, CLI and API</strong></summary>
- Use the **AME Console** to organise environments, create clusters, inspect
  activity and manage lifecycle operations.
- Use the **`acloud` CLI** to manage clusters and open authenticated cluster
  shells from a terminal.
- Use the **REST API** and **Go client** to integrate AME into internal
  platforms and automation.
</details>

<details>
<summary><strong>Terraform and operational tooling</strong></summary>

- [`terraform-provider-acloud`](https://github.com/avisi-cloud/terraform-provider-acloud)
  manages AME resources through infrastructure as code.
- [`acloud-toolkit`](https://github.com/avisi-cloud/acloud-toolkit) automates
  recurring Kubernetes tasks such as snapshots and operational workflows.
- [`go-client`](https://github.com/avisi-cloud/go-client) provides typed access
  to the Avisi Cloud API for Go applications.

</details>

## Kubernetes lifecycle and releases

AME uses release channels to separate early validation from production
adoption. Releases track Kubernetes, the AME controllers, operating-system
images and managed platform components together.

Do not rely on a static README for current component versions:

- [Release notes](https://docs.avisi.cloud/docs/product/overview/release-notes)
  document current channels, versions, fixes and required actions.
- [Engineering Blog](https://docs.avisi.cloud/blog) covers notable platform
  changes, Kubernetes support and engineering guidance.
- [Platform Status](https://status.avisi.cloud/) reports service health.

## Get started

1. [Open the AME Console](https://console.avisi.cloud/) and create a trial
   organisation.
2. Connect a supported cloud account or discuss private-infrastructure
   integration with Avisi Cloud.
3. Create an environment and deploy a Kubernetes cluster.
4. Manage the platform through the Console, CLI, API or Terraform.

| Need                       | Resource                                                                          |
| -------------------------- | --------------------------------------------------------------------------------- |
| Learn the platform         | [AME Documentation](https://docs.avisi.cloud/)                                    |
| Compare capabilities       | [AME Features](https://avisi.cloud/features)                                      |
| Track product changes      | [Engineering Blog](https://docs.avisi.cloud/blog)                                 |
| Review current releases    | [AME Release Notes](https://docs.avisi.cloud/docs/product/overview/release-notes) |
| Resolve operational alerts | [Kubernetes and cloud-native runbooks](https://docs.avisi.cloud/docs/runbooks)    |
| Check service health       | [Avisi Cloud Status](https://status.avisi.cloud/)                                 |
| Contact support            | [support@avisi.cloud](mailto:support@avisi.cloud)                                 |

## Kubernetes certified

Avisi Cloud provides CNCF-conformant Kubernetes and is a Kubernetes Certified
Service Provider, combining a portable upstream Kubernetes foundation with
managed lifecycle operations and engineering support.

<p>
  <img src="./img/certified-kubernetes.webp" alt="Certified Kubernetes">
</p>

---

<p>
  <a href="https://avisi.cloud/">Avisi Cloud</a> ·
  Part of <a href="https://www.avisi.nl/cloud">Avisi Group B.V.</a><br>
  © 2026 Avisi Cloud
</p>
