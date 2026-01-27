## OpenFGA

[![CNCF Incubation](https://img.shields.io/badge/CNCF-Incubating-blue?logo=cncf)](https://www.cncf.io/projects/openfga/)
[![Join our community](https://img.shields.io/badge/slack-cncf_%23openfga-40abb8.svg?logo=slack)](https://openfga.dev/community)
[![Twitter](https://img.shields.io/twitter/follow/openfga?color=%23179CF0&logo=twitter&style=flat-square "@openfga on Twitter")](https://twitter.com/openfga)
[![OpenFGA YouTube Channel](https://img.shields.io/badge/YouTube-Subscribe-red?style=flat&logo=youtube)](https://www.youtube.com/@OpenFGA)
[![CLOMonitor](https://img.shields.io/endpoint?url=https://clomonitor.io/api/projects/cncf/openfga/badge)](https://clomonitor.io/projects/cncf/openfga)
[![LFX Health Score](https://img.shields.io/static/v1?label=Health%20Score&message=Excellent&color=10B981&logo=linuxfoundation&logoColor=white&style=flat)](https://insights.linuxfoundation.org/project/openfga)

OpenFGA is a high-performance, flexible authorization/permission engine built for developers and inspired by [Google Zanzibar](https://research.google/pubs/pub48190/). It combines [Relationship-Based Access Control (ReBAC)](https://en.wikipedia.org/wiki/Relationship-based_access_control) and [Attribute-Based Access Control (ABAC)](https://en.wikipedia.org/wiki/Attribute-based_access_control) with a domain-specific language that makes it easy to craft authorization solutions that grow and evolve to any use case, at any scale.

Originally developed by Auth0/Okta and [donated to the Cloud Native Computing Foundation](https://www.cncf.io/projects/openfga/) in September 2022, OpenFGA is currently at the Incubation level and maintained by [Okta and Grafana employees](https://github.com/openfga/community/blob/main/MAINTAINERS.md).

**Adopted by:** [Auth0](https://fga.dev) | [Grafana Labs](https://grafana.com/) | [Canonical](https://canonical.com/) | [Docker](https://docker.com) | [Agicap](https://agicap.com) | [Read.AI](https://read.ai) | [Headspace](https://headspace.com) | [and more...](https://github.com/openfga/community/blob/main/ADOPTERS.md)

---

### 🚀 Quick Start

```bash
# Run OpenFGA locally with Docker
docker pull openfga/openfga
docker run -p 8080:8080 -p 3000:3000 openfga/openfga run
```

Then explore the [playground](http://localhost:3000/playground), read the [documentation](https://openfga.dev/docs/getting-started), or watch the [OpenFGA Modeling Guide](https://www.youtube.com/playlist?list=PLUR5l-oTFZqWaDdhEOVt_IfPOIbKo1Ypt) for tutorials.

---

### 🙋‍♀️ Why Fine-Grained Authorization?

OpenFGA is designed to solve authorization for everyone, regardless of scale or complexity. Fine-grained authorization is becoming critical for modern software:

* **Agentic AI requires authorization**. You can't expose your API to agents without proper authorization. You also need authorization for Retrieval-Augmented Generation (RAG) and restricting Agent access to APIs or MCP servers.

* **Users expect collaboration features**. From 'Share' buttons to 'Request Access' workflows—for documents, project boards, photo albums, and IoT devices—OpenFGA makes these easy to build and govern.

* **Traditional RBAC doesn't scale**. Fine-grained approaches like OpenFGA create authorization models that remain easy to understand and visualize, even for complex patterns.

* **Security and compliance are mandatory**. The top risk in the [OWASP Top 10](https://owasp.org/Top10/) is [Broken Access Control](https://owasp.org/Top10/A01_2021-Broken_Access_Control/). Authorization is a critical part of any security solution.

---

### 💡 Why Centralize Authorization?

Centralizing authorization into a single, flexible service provides distinct advantages:

* **Ship faster** — Easily extensible to new requirements across all your products
* **Simplify auditing** — Explicit rules are easier to audit; built-in logs for all operations
* **Lower operational costs** — One authorization system is simpler to manage
* **Improve developer experience** — Same concepts and APIs regardless of team

---

### 🛠️ Developer Tooling

OpenFGA provides high-quality developer tooling:

- **AI Agent Skills** — [Skills](https://github.com/openfga/agent-skills) for AI Agents
- **SDKs** — [Go](https://github.com/openfga/go-sdk) | [JavaScript](https://github.com/openfga/js-sdk) | [.NET](https://github.com/openfga/dotnet-sdk) | [Python](https://github.com/openfga/python-sdk) | [Java](https://github.com/openfga/java-sdk)
- **CLI** — [Operate servers](https://github.com/openfga/cli), import/export models and tuples, run tests
- **IDE Extensions** — [VS Code](https://marketplace.visualstudio.com/items?itemName=openfga.openfga-vscode) and [JetBrains](https://plugins.jetbrains.com/plugin/24394-openfga) with syntax highlighting and validation
- **Kubernetes** — [Helm Chart](https://github.com/openfga/helm-charts) for easy deployment
- **CI/CD** — GitHub Actions for [testing](https://github.com/marketplace/actions/openfga-model-testing-action) and [deploying](https://github.com/marketplace/actions/openfga-model-deploy-action) models
- **Modular Models** — [Multi-team support](https://openfga.dev/docs/modeling/modular-models) for a single authorization system
- **Infrastructure as Code** — [Terraform Provider](https://github.com/openfga/terraform-provider-openfga)

---

### 👩‍💻 Useful Resources

| Resource | Description |
|----------|-------------|
| [Documentation](https://openfga.dev) | Guides, tutorials, and API reference |
| [Community](https://openfga.dev/community) | Join us on CNCF Slack or [GitHub Discussions](https://github.com/orgs/openfga/discussions) |
| [Contributing](https://github.com/openfga/.github/blob/main/CONTRIBUTING.md) | How to contribute code, docs, and more |
| [Adopters](https://github.com/openfga/community/blob/main/ADOPTERS.md) | Companies using OpenFGA in production |
| [Community Projects](https://github.com/openfga/community#community-projects) | Integrations and tools built by the community |

---

**Ready to get started?** Check out the [documentation](https://openfga.dev/docs/getting-started) or join us on [Slack](https://openfga.dev/community).
