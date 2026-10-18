# Awesome Everything-as-Code (EaC) [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of tools, patterns, and methodologies for a text-based, versionable, and automated world.

**Everything as Code (EaC)** is the philosophy of treating all aspects of the software development lifecycle and business operations—infrastructure, diagrams, presentations, policies, and even finance—as code. If it's in Git, it exists.

## Contents

- [Foundations](#foundations)
- [Infrastructure &amp; Cloud](#infrastructure--cloud)
  - [Infrastructure as Code](#infrastructure-as-code)
  - [Configuration as Code](#configuration-as-code)
  - [Policy as Code](#policy-as-code)
  - [APIs as Code](#apis-as-code)
  - [GitOps](#gitops)
  - [Development Environments as Code](#development-environments-as-code)
  - [Monitoring as Code](#monitoring-as-code)
  - [Pipelines as Code](#pipelines-as-code)
  - [Backend as Code](#backend-as-code)
  - [Build as Code](#build-as-code)
- [Visuals &amp; Media](#visuals--media)
  - [Diagrams as Code](#diagrams-as-code)
  - [Presentations as Code](#presentations-as-code)
  - [Documents as Code](#documents-as-code)
  - [Documentation as Code](#documentation-as-code)
  - [Video as Code](#video-as-code)
  - [CAD as Code](#cad-as-code)
- [Data &amp; Analytics](#data--analytics)
  - [Data Transformation as Code](#data-transformation-as-code)
  - [BI as Code](#bi-as-code)
  - [Data Quality as Code](#data-quality-as-code)
  - [Visualization Libraries](#visualization-libraries)
  - [Database as Code](#database-as-code)
  - [Dashboards as Code](#dashboards-as-code)
  - [Workflows as Code](#workflows-as-code)
  - [AI Evaluations as Code](#ai-evaluations-as-code)
- [Business &amp; Productivity](#business--productivity)
  - [Resume as Code](#resume-as-code)
  - [Finance as Code](#finance-as-code)
  - [Notes as Code](#notes-as-code)
  - [Email as Code](#email-as-code)
  - [Forms as Code](#forms-as-code)
- [Patterns &amp; Methodologies](#patterns--methodologies)
- [Resources](#resources)
  - [Books](#books)
  - [Articles](#articles)
  - [Talks](#talks)
- [Related Awesome Lists](#related-awesome-lists)
  - [Infrastructure &amp; Cloud](#infrastructure--cloud-1)
  - [Diagrams &amp; Documentation](#diagrams--documentation)
  - [Data](#data)
  - [Security &amp; Policy](#security--policy)
  - [Productivity](#productivity)
- [Contributing](#contributing)

## Foundations

*The languages and specifications that power the EaC world.*

- [CUE](https://cuelang.org/) - Data validation language that makes it easy to define and use data schemas.
- [HCL](https://github.com/hashicorp/hcl) - HashiCorp Configuration Language built for infrastructure.
- [JSON](https://www.json.org/) - Lightweight data-interchange format.
- [Jsonnet](https://jsonnet.org/) - Data templating language for generating JSON/YAML.
- [Markdown](https://daringfireball.net/projects/markdown/) - The ubiquitous markup language for documentation.
- [Nickel](https://github.com/nickel-lang/nickel) - Compose, validate, and generate static configuration with a dedicated configuration language.
- [OpenAPI](https://www.openapis.org/) - Standard for defining RESTful APIs in YAML/JSON.
- [Pkl](https://github.com/apple/pkl) - Define typed configuration with validation and tooling for generating configuration files.
- [TOML](https://toml.io/) - Tom's Obvious Minimal Language for configuration files.
- [YAML](https://yaml.org/) - Human-friendly data serialization standard.

## Infrastructure & Cloud

### Infrastructure as Code

*Define and provision infrastructure using declarative configuration files.*

- [Alchemy](https://github.com/alchemy-run/alchemy) - Define cloud resources alongside application code in TypeScript (currently in beta).
- [CDK](https://aws.amazon.com/cdk/) - Define AWS cloud infrastructure using familiar programming languages.
- [CDKTF](https://developer.hashicorp.com/terraform/cdktf) - Use familiar programming languages to define Terraform infrastructure.
- [Crossplane](https://www.crossplane.io/) - Build cloud infrastructure and platform APIs with declarative Kubernetes resources.
- [OpenTofu](https://opentofu.org/) - Open source fork of Terraform.
- [Packer](https://www.packer.io/) - Build machine images for multiple platforms from HCL templates.
- [Pulumi](https://www.pulumi.com/) - Infrastructure as Code using familiar programming languages.
- [SST](https://github.com/anomalyco/sst) - Define and deploy full-stack applications and cloud infrastructure with TypeScript.
- [Terraform](https://www.terraform.io/) - Infrastructure as Code tool for building, changing, and versioning infrastructure.
- [Terramate](https://github.com/terramate-io/terramate) - Orchestrate infrastructure stacks and generate configuration to reduce duplication across environments.

### Configuration as Code

*Manage system and application configuration through version-controlled files.*

- [Ansible](https://www.ansible.com/) - Agentless automation and configuration management in YAML.
- [cloud-init](https://cloud-init.io/) - Initialize cloud instances with declarative configuration.
- [Docker Compose](https://docs.docker.com/compose/) - Define multi-container applications, networks, and volumes in YAML.
- [Helm](https://helm.sh/) - The package manager for Kubernetes with templated YAML.
- [Kustomize](https://kustomize.io/) - Kubernetes native configuration management without templates.
- [Nix / NixOS](https://nixos.org/) - Define reproducible packages, development environments, and operating systems declaratively.
- [Pulumi ESC](https://github.com/pulumi/esc) - Compose environment configuration and secret references with declarative definitions.
- [Timoni](https://github.com/stefanprodan/timoni) - Define Kubernetes applications with CUE and distribute reusable modules as OCI artifacts.

### Policy as Code

*Define security, compliance, and governance rules as versionable code.*

- [Checkov](https://www.checkov.io/) - Static analysis tool for infrastructure as code security.
- [Conftest](https://www.conftest.dev/) - Write tests against structured configuration data.
- [Falco](https://falco.org/) - Cloud native runtime security using declarative rules.
- [Kyverno](https://kyverno.io/) - Define Kubernetes validation, mutation, and resource generation policies in YAML.
- [Open Policy Agent](https://www.openpolicyagent.org/) - Policy-based control for cloud native environments.
- [Sentinel](https://www.hashicorp.com/sentinel) - Policy as code framework by HashiCorp.
- [Trivy](https://trivy.dev/) - Comprehensive security scanner for containers and IaC.

### APIs as Code

*Generate API implementations, clients, and documentation from version-controlled specifications.*

- [OpenAPI Generator](https://github.com/OpenAPITools/openapi-generator) - Generate API clients, server stubs, and documentation from OpenAPI specifications.
- [Smithy](https://smithy.io/) - Define language-independent service models and API contracts.
- [TypeSpec](https://typespec.io/) - Describe API contracts with a modeling language and generate OpenAPI specifications.

### GitOps

*Continuously reconcile deployed applications with desired state stored in Git.*

- [Argo CD](https://argo-cd.readthedocs.io/) - Synchronize Kubernetes applications with declarative configuration stored in Git.
- [Flux](https://fluxcd.io/) - Reconcile Kubernetes deployments with version-controlled manifests and Helm releases.

### Development Environments as Code

*Define reproducible development tools, services, and container environments.*

- [Dev Container Specification](https://containers.dev/) - Describe container-based development environments with devcontainer.json.
- [Devbox](https://github.com/jetify-com/devbox) - Declare development tools and packages in devbox.json for isolated Nix-based environments.
- [devenv](https://devenv.sh/) - Define reproducible development environments, services, and tasks with Nix.
- [mise](https://github.com/jdx/mise) - Define tool versions, environment variables, and tasks in mise.toml.
- [Pixi](https://github.com/prefix-dev/pixi) - Manage reproducible multi-language dependencies, tasks, and environments with manifests and lockfiles.

### Monitoring as Code

*Version monitoring configuration and alerting rules alongside application code.*

- [Prometheus](https://prometheus.io/) - Define alerting and recording rules with YAML configuration and PromQL expressions.

### Pipelines as Code

*Define reusable continuous integration and delivery pipelines declaratively.*

- [Dagger](https://github.com/dagger/dagger) - Build programmable pipelines with reusable components and container-based execution.
- [Tekton](https://tekton.dev/) - Define CI/CD tasks and pipelines with declarative Kubernetes resources.

### Backend as Code

*Define backend services and infrastructure requirements alongside application code.*

- [Encore](https://github.com/encoredev/encore) - Declare backend APIs and infrastructure resources in application code for local development and cloud provisioning.

### Build as Code

*Define project tasks, dependencies, and build workflows in version-controlled configuration.*

- [moon](https://github.com/moonrepo/moon) - Configure projects, tasks, and execution dependencies for repositories and monorepos.

## Visuals & Media

### Diagrams as Code

*Create diagrams and visualizations from text-based definitions.*

- [Beautiful Mermaid](https://github.com/lukilabs/beautiful-mermaid) - Render Mermaid definitions as SVG diagrams or ASCII art.
- [D2](https://d2lang.com/) - A modern declarative language that turns text into professional diagrams.
- [Diagrams](https://diagrams.mingrammer.com/) - Draw cloud system architecture in Python code.
- [Ditaa](https://ditaa.sourceforge.net/) - Render diagrams from ASCII art descriptions.
- [Graphviz](https://graphviz.org/) - Open source graph visualization software using DOT language.
- [Infographic](https://infographic.antv.vision/) - Declarative infographic rendering.
- [LikeC4](https://github.com/likec4/likec4) - Describe software architecture with a modeling language and generate diagrams from the model.
- [Markmap](https://markmap.js.org/) - Visualize Markdown documents as interactive mindmaps.
- [Mermaid](https://mermaid.js.org/) - JavaScript-based diagramming tool that renders Markdown-inspired text.
- [Penrose](https://github.com/penrose/penrose) - Generate diagrams from textual descriptions of concepts, relationships, and visual rules.
- [PlantUML](https://plantuml.com/) - Create UML diagrams from plain text descriptions.
- [Structurizr](https://structurizr.com/) - Architecture diagrams as code using the C4 model.
- [WaveDrom](https://wavedrom.com/) - Render digital timing diagrams from JSON-based textual descriptions.

### Presentations as Code

*Build slide decks using text files and version control.*

- [Marp](https://marp.app/) - Markdown presentation ecosystem with CLI and VS Code support.
- [Presenterm](https://github.com/mfontanini/presenterm) - Create and run terminal presentations from Markdown files.
- [reveal.js](https://revealjs.com/) - HTML presentation framework with Markdown support.
- [Slidev](https://sli.dev/) - Markdown-based presentation slides with Vue components for developers.
- [Spectacle](https://formidable.com/open-source/spectacle/) - React-based presentation library.

### Documents as Code

*Create professional documents from markup and code.*

- [Asciidoctor](https://asciidoctor.org/) - Text processor for converting AsciiDoc to various formats.
- [LaTeX](https://www.latex-project.org/) - Document preparation system for high-quality typesetting.
- [Pandoc](https://pandoc.org/) - Universal document converter between markup formats.
- [Quarkdown](https://github.com/iamgio/quarkdown) - Create books, documents, and presentations with an extended Markdown typesetting language.
- [Quarto](https://quarto.org/) - Publish reproducible reports, books, presentations, and websites combining text and executable code.
- [React-pdf](https://github.com/diegomura/react-pdf) - Create PDF documents with React components in the browser or on the server.
- [Typst](https://typst.app/) - Modern markup-based typesetting system for documents.

### Documentation as Code

*Build documentation sites from version-controlled Markdown and configuration files.*

- [docmd](https://github.com/docmd-io/docmd) - Compile Markdown documentation into static sites and machine-readable knowledge formats.
- [Docusaurus](https://docusaurus.io/) - Build documentation websites from Markdown, MDX, and version-controlled configuration.
- [Material for MkDocs](https://github.com/squidfunk/mkdocs-material) - Build searchable documentation sites from Markdown and YAML configuration.
- [Sphinx](https://www.sphinx-doc.org/) - Generate technical documentation from reStructuredText and extensible text sources.
- [VitePress](https://vitepress.dev/) - Build documentation websites from Markdown with Vue components.

### Video as Code

*Generate video content programmatically.*

- [HyperFrames](https://github.com/heygen-com/hyperframes) - Render HTML, CSS, media, and seekable animations into deterministic MP4 videos.
- [Manim](https://www.manim.community/) - Create mathematical animations programmatically in Python.
- [Motion Canvas](https://motioncanvas.io/) - TypeScript library for creating animated videos.
- [Remotion](https://www.remotion.dev/) - Create real videos programmatically using React.
- [Revideo](https://github.com/midrender/revideo) - Create video scenes and animations in TypeScript with programmatic rendering and a React player.
- [Satori](https://github.com/vercel/satori) - Convert HTML and CSS into SVG images.
- [Simple FFmpegJS](https://github.com/Fats403/simple-ffmpegjs) - Compose videos with declarative timelines of clips, audio, and transitions using FFmpeg in Node.js.

### CAD as Code

*Create parametric 3D models from version-controlled text definitions.*

- [CadQuery](https://cadquery.readthedocs.io/) - Create parametric CAD models with Python.
- [OpenSCAD](https://openscad.org/) - Create solid 3D models with a textual constructive geometry language.

## Data & Analytics

### Data Transformation as Code

*Define data pipelines and transformations in version-controlled code.*

- [Dagster](https://dagster.io/) - Data orchestration platform with declarative pipelines.
- [dbt](https://www.getdbt.com/) - The industry standard for data transformation as code.
- [Malloy](https://www.malloydata.dev/) - Experimental language for describing data relationships.
- [SQLMesh](https://sqlmesh.com/) - Next-generation data transformation framework.

### BI as Code

*Build reports and dashboards using SQL and Markdown.*

- [Evidence.dev](https://evidence.dev/) - Build high-quality data products using SQL and Markdown.
- [Rill](https://www.rilldata.com/) - Fast operational dashboards from SQL and YAML.

### Data Quality as Code

*Define data validation and expectations as code.*

- [dbt tests](https://docs.getdbt.com/docs/build/tests) - Built-in testing framework for dbt models.
- [Great Expectations](https://greatexpectations.io/) - Data validation and documentation as code.
- [Soda](https://www.soda.io/) - Data quality testing using YAML configuration.

### Visualization Libraries

*Programmatic charting and plotting tools for data analysis.*

- [Altair](https://altair-viz.github.io/) - Declarative statistical visualization library for Python built on Vega-Lite.
- [Bokeh](https://bokeh.org/) - Interactive visualization library for modern web browsers.
- [Chart.js](https://www.chartjs.org/) - Simple yet flexible JavaScript charting for designers & developers.
- [D3.js](https://d3js.org/) - JavaScript library for manipulating documents based on data.
- [ggplot (plotnine)](https://plotnine.readthedocs.io/) - Grammar of graphics for Python inspired by R's ggplot2.
- [Holoviews](https://holoviews.org/) - Declarative data analysis and visualization library for Python.
- [Matplotlib](https://matplotlib.org/) - Comprehensive 2D plotting library for Python.
- [Plotly](https://plotly.com/) - Interactive plotting library for Python, R, and JavaScript.
- [Seaborn](https://seaborn.pydata.org/) - High-level statistical data visualization built on Matplotlib.
- [Vega/Vega-Lite](https://vega.github.io/vega-lite/) - Declarative language for creating, saving, and sharing interactive visualization designs.

### Database as Code

*Describe database structures and relationships with version-controlled schemas.*

- [Atlas](https://github.com/ariga/atlas) - Manage database schemas declaratively and generate migration plans from desired schema definitions.
- [DBML](https://dbml.dbdiagram.io/) - Define database tables and relationships with a declarative modeling language.
- [Drizzle ORM + Kit](https://github.com/drizzle-team/drizzle-orm) - Declare SQL schemas in TypeScript and generate migrations from schema definitions.

### Dashboards as Code

*Generate dashboards from reusable, version-controlled definitions.*

- [Grafonnet](https://grafana.github.io/grafonnet/) - Generate Grafana dashboards with reusable Jsonnet definitions.

### Workflows as Code

*Define task dependencies, triggers, and orchestration in version-controlled files.*

- [Argo Workflows](https://argoproj.github.io/workflows/) - Define container workflows as steps and dependency graphs in YAML.
- [Kestra](https://kestra.io/) - Declare orchestration workflows, tasks, dependencies, and triggers in YAML.

### AI Evaluations as Code

*Version evaluation cases, model providers, and assertions for AI systems.*

- [Promptfoo](https://www.promptfoo.dev/) - Define and run AI evaluations with version-controlled test cases and assertions.

## Business & Productivity

### Resume as Code

*Create and maintain your resume in structured data formats.*

- [HackMyResume](https://github.com/hacksalot/HackMyResume) - Generate resumes from JSON/YAML.
- [JSON Resume](https://jsonresume.org/) - An open source standard for resumes in JSON format.
- [RenderCV](https://docs.rendercv.com/) - Write your CV as YAML.
- [Standard Resume](https://standardresume.co/) - Build a professional resume from a text-based workflow.

### Finance as Code

*Track personal and business finances in plain text.*

- [Beancount](https://github.com/beancount/beancount/) - Double-entry bookkeeping in plain text.
- [hledger](https://hledger.org/) - Plain text accounting software inspired by Ledger.
- [Ledger](https://ledger-cli.org/) - Command-line accounting with plain text files.

### Notes as Code

*Manage knowledge and notes in plain text format.*

- [Obsidian](https://obsidian.md/) - Knowledge base that works on local Markdown files.
- [Org Mode](https://orgmode.org/) - Notes, planning, and authoring in plain text for Emacs.

### Email as Code

*Create email content from version-controlled text sources.*

- [emailmd](https://github.com/anypost/emailmd) - Convert Markdown into responsive HTML emails.
- [Maizzle](https://github.com/maizzle/framework) - Build HTML emails with templates, Tailwind CSS, and version-controlled configuration.
- [MJML](https://mjml.io/) - Create responsive email templates with a dedicated markup language.
- [React Email](https://react.email/) - Build version-controlled email templates with React components.

### Forms as Code

*Generate user interfaces from declarative schemas.*

- [JSON Forms](https://jsonforms.io/) - Generate forms from JSON Schema and declarative UI schemas.

## Patterns & Methodologies

*Approaches for scaling the EaC philosophy across organizations.*

- [API Design First](https://swagger.io/resources/articles/adopting-an-api-first-approach/) - Define APIs before implementing them.
- [Architecture Decision Records](https://adr.github.io/) - Capture important architectural decisions in text files.
- [Docs as Code](https://www.writethedocs.org/guide/docs-as-code/) - Apply software development practices to documentation.
- [GitOps](https://opengitops.dev/) - Using Git as the single source of truth for declarative infrastructure.
- [Ivy Tendril](https://github.com/Ivy-Interactive/Ivy-Tendril) - AI coding orchestration as code. Plans, verification gates, and agent memory defined in YAML and versionable in Git.
- [Literate Programming](https://en.wikipedia.org/wiki/Literate_programming) - Writing code as a narrative for humans.
- [Schema First](https://graphql.org/learn/schema/) - Define data schemas before writing application code.

## Resources

### Books

*Essential reading for the Everything as Code practitioner.*

- [Infrastructure as Code](https://www.oreilly.com/library/view/infrastructure-as-code/9781098114664/) - Comprehensive guide to managing cloud infrastructure with automation by Kief Morris.
- [Terraform: Up &amp; Running](https://www.terraformupandrunning.com/) - Practical guide to writing, planning, and creating IaC with Terraform by Yevgeniy Brikman.

### Articles

*Key articles explaining EaC concepts and practices.*

- [Infrastructure as Code: A Primer](https://www.hashicorp.com/resources/what-is-infrastructure-as-code) - HashiCorp's introduction to IaC concepts.

### Talks

*Conference talks and presentations about EaC practices.*

- [Everything as Code](https://youtu.be/HcmPi7-IVQo?si=RZxxr3m7f6Q7xbgO) - Seth Vargo's talk on codification and automation in cloud environments.
- [Infrastructure as Code](https://martinfowler.com/bliki/InfrastructureAsCode.html) - Fowler's original definition of IaC.

## Related Awesome Lists

*Other curated lists covering related topics.*

### Infrastructure & Cloud

- [Awesome Ansible](https://github.com/ansible-community/awesome-ansible) - Ansible roles, playbooks, and resources.
- [Awesome GitOps](https://github.com/weaveworks/awesome-gitops) - Resources for GitOps practices.
- [Awesome Kubernetes](https://github.com/ramitsurana/awesome-kubernetes) - Curated list for Kubernetes.
- [Awesome Policy as Code](https://github.com/hysnsec/awesome-policy-as-code) - Curated list of Policy as Code resources.
- [Awesome Pulumi](https://github.com/pulumiverse/awesome-pulumi) - Resources for Pulumi infrastructure as code.
- [Awesome Terraform](https://github.com/shuaibiyy/awesome-terraform) - Curated list of Terraform resources and modules.

### Diagrams & Documentation

- [Awesome README](https://github.com/matiassingers/awesome-readme) - Curated list of awesome READMEs.
- [Awesome Technical Writing](https://github.com/BolajiAyodeji/awesome-technical-writing) - Technical writing resources.

### Data

- [Awesome Data Engineering](https://github.com/igorbarinov/awesome-data-engineering) - Data engineering resources.
- [Awesome dbt](https://github.com/Hiflylabs/awesome-dbt) - Curated list of dbt resources.

### Security & Policy

- [Awesome DevSecOps](https://github.com/TaptuIT/awesome-devsecops) - Security as code practices.
- [Awesome Open Policy Agent](https://github.com/StyraInc/awesome-opa) - Resources for OPA and Rego.

### Productivity

- [Awesome Markdown](https://github.com/BubuAnabelas/awesome-markdown) - Markdown tools and resources.

## Contributing

Contributions are welcome! Please read the [contribution guidelines](contributing.md) first.
