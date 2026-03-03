# Awesome Everything-as-Code (EaC) [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of tools, patterns, and methodologies for a text-based, versionable, and automated world.

**Everything as Code (EaC)** is the philosophy of treating all aspects of the software development lifecycle and business operations—infrastructure, diagrams, presentations, policies, and even finance—as code. If it's in Git, it exists.

## Contents

- [Foundations](#foundations)
- [Infrastructure &amp; Cloud](#infrastructure--cloud)
- [Visuals &amp; Media](#visuals--media)
- [Data &amp; Analytics](#data--analytics)
- [Business &amp; Productivity](#business--productivity)
- [Patterns &amp; Methodologies](#patterns--methodologies)
- [Resources](#resources)
- [Related Awesome Lists](#related-awesome-lists)

## Foundations

*The languages and specifications that power the EaC world.*

- [YAML](https://yaml.org/) - Human-friendly data serialization standard.
- [HCL](https://github.com/hashicorp/hcl) - HashiCorp Configuration Language built for infrastructure.
- [JSON](https://www.json.org/) - Lightweight data-interchange format.
- [TOML](https://toml.io/) - Tom's Obvious Minimal Language for configuration files.
- [CUE](https://cuelang.org/) - Data validation language that makes it easy to define and use data schemas.
- [Jsonnet](https://jsonnet.org/) - Data templating language for generating JSON/YAML.
- [OpenAPI](https://www.openapis.org/) - Standard for defining RESTful APIs in YAML/JSON.
- [Markdown](https://daringfireball.net/projects/markdown/) - The ubiquitous markup language for documentation.

## Infrastructure & Cloud

### Infrastructure as Code

*Define and provision infrastructure using declarative configuration files.*

- [Terraform](https://www.terraform.io/) - Infrastructure as Code tool for building, changing, and versioning infrastructure.
- [OpenTofu](https://opentofu.org/) - Open source fork of Terraform.
- [Pulumi](https://www.pulumi.com/) - Infrastructure as Code using familiar programming languages.
- [CDK](https://aws.amazon.com/cdk/) - Define AWS cloud infrastructure using familiar programming languages.
- [CDKTF](https://developer.hashicorp.com/terraform/cdktf) - Use familiar programming languages to define Terraform infrastructure.

### Configuration as Code

*Manage system and application configuration through version-controlled files.*

- [Ansible](https://www.ansible.com/) - Agentless automation and configuration management in YAML.
- [Helm](https://helm.sh/) - The package manager for Kubernetes with templated YAML.
- [Kustomize](https://kustomize.io/) - Kubernetes native configuration management without templates.

### Policy as Code

*Define security, compliance, and governance rules as versionable code.*

- [Open Policy Agent](https://www.openpolicyagent.org/) - Policy-based control for cloud native environments.
- [Sentinel](https://www.hashicorp.com/sentinel) - Policy as code framework by HashiCorp.
- [Conftest](https://www.conftest.dev/) - Write tests against structured configuration data.
- [Checkov](https://www.checkov.io/) - Static analysis tool for infrastructure as code security.
- [Trivy](https://trivy.dev/) - Comprehensive security scanner for containers and IaC.
- [Falco](https://falco.org/) - Cloud native runtime security using declarative rules.

## Visuals & Media

### Diagrams as Code

*Create diagrams and visualizations from text-based definitions.*

- [D2](https://d2lang.com/) - A modern declarative language that turns text into professional diagrams.
- [Mermaid](https://mermaid.js.org/) - JavaScript-based diagramming tool that renders Markdown-inspired text.
- [PlantUML](https://plantuml.com/) - Create UML diagrams from plain text descriptions.
- [Graphviz](https://graphviz.org/) - Open source graph visualization software using DOT language.
- [Diagrams](https://diagrams.mingrammer.com/) - Draw cloud system architecture in Python code.
- [Markmap](https://markmap.js.org/) - Visualize Markdown documents as interactive mindmaps.
- [Structurizr](https://structurizr.com/) - Architecture diagrams as code using the C4 model.
- [Infographic](https://infographic.antv.vision/) - Declarative infographic rendering.

### Presentations as Code

*Build slide decks using text files and version control.*

- [Slidev](https://sli.dev/) - Markdown-based presentation slides with Vue components for developers.
- [Marp](https://marp.app/) - Markdown presentation ecosystem with CLI and VS Code support.
- [reveal.js](https://revealjs.com/) - HTML presentation framework with Markdown support.
- [Spectacle](https://formidable.com/open-source/spectacle/) - React-based presentation library.

### Documents as Code

*Create professional documents from markup and code.*

- [Typst](https://typst.app/) - Modern markup-based typesetting system for documents.
- [LaTeX](https://www.latex-project.org/) - Document preparation system for high-quality typesetting.
- [Pandoc](https://pandoc.org/) - Universal document converter between markup formats.
- [Asciidoctor](https://asciidoctor.org/) - Text processor for converting AsciiDoc to various formats.

### Video as Code

*Generate video content programmatically.*

- [Remotion](https://www.remotion.dev/) - Create real videos programmatically using React.
- [Manim](https://www.manim.community/) - Create mathematical animations programmatically in Python.
- [Satori](https://github.com/vercel/satori) - Convert HTML and CSS into SVG images.
- [Motion Canvas](https://motioncanvas.io/) - TypeScript library for creating animated videos.

## Data & Analytics

### Data Transformation as Code

*Define data pipelines and transformations in version-controlled code.*

- [dbt](https://www.getdbt.com/) - The industry standard for data transformation as code.
- [SQLMesh](https://sqlmesh.com/) - Next-generation data transformation framework.
- [Malloy](https://www.malloydata.dev/) - Experimental language for describing data relationships.
- [Dagster](https://dagster.io/) - Data orchestration platform with declarative pipelines.

### BI as Code

*Build reports and dashboards using SQL and Markdown.*

- [Evidence.dev](https://evidence.dev/) - Build high-quality data products using SQL and Markdown.
- [Rill](https://www.rilldata.com/) - Fast operational dashboards from SQL and YAML.

### Data Quality as Code

*Define data validation and expectations as code.*

- [Great Expectations](https://greatexpectations.io/) - Data validation and documentation as code.
- [Soda](https://www.soda.io/) - Data quality testing using YAML configuration.
- [dbt tests](https://docs.getdbt.com/docs/build/tests) - Built-in testing framework for dbt models.

### Visualization Libraries

*Programmatic charting and plotting tools for data analysis.*

- [Matplotlib](https://matplotlib.org/) - Comprehensive 2D plotting library for Python.
- [Seaborn](https://seaborn.pydata.org/) - High-level statistical data visualization built on Matplotlib.
- [Altair](https://altair-viz.github.io/) - Declarative statistical visualization library for Python built on Vega-Lite.
- [Plotly](https://plotly.com/) - Interactive plotting library for Python, R, and JavaScript.
- [Bokeh](https://bokeh.org/) - Interactive visualization library for modern web browsers.
- [ggplot (plotnine)](https://plotnine.readthedocs.io/) - Grammar of graphics for Python inspired by R's ggplot2.
- [Vega/Vega-Lite](https://vega.github.io/vega-lite/) - Declarative language for creating, saving, and sharing interactive visualization designs.
- [D3.js](https://d3js.org/) - JavaScript library for manipulating documents based on data.
- [Chart.js](https://www.chartjs.org/) - Simple yet flexible JavaScript charting for designers & developers.
- [Holoviews](https://holoviews.org/) - Declarative data analysis and visualization library for Python.
## Business & Productivity

### Resume as Code

*Create and maintain your resume in structured data formats.*

- [JSON Resume](https://jsonresume.org/) - An open source standard for resumes in JSON format.
- [Standard Resume](https://standardresume.co/) - Build a professional resume from a text-based workflow.
- [HackMyResume](https://github.com/hacksalot/HackMyResume) - Generate resumes from JSON/YAML.
- [RenderCV](https://docs.rendercv.com/) - Write your CV as YAML.

### Finance as Code

*Track personal and business finances in plain text.*

- [Beancount](https://github.com/beancount/beancount/) - Double-entry bookkeeping in plain text.
- [Ledger](https://ledger-cli.org/) - Command-line accounting with plain text files.
- [hledger](https://hledger.org/) - Plain text accounting software inspired by Ledger.

### Notes as Code

*Manage knowledge and notes in plain text format.*

- [Org Mode](https://orgmode.org/) - Notes, planning, and authoring in plain text for Emacs.
- [Obsidian](https://obsidian.md/) - Knowledge base that works on local Markdown files.

## Patterns & Methodologies

*Approaches for scaling the EaC philosophy across organizations.*

- [GitOps](https://opengitops.dev/) - Using Git as the single source of truth for declarative infrastructure.
- [Architecture Decision Records](https://adr.github.io/) - Capture important architectural decisions in text files.
- [Docs as Code](https://www.writethedocs.org/guide/docs-as-code/) - Apply software development practices to documentation.
- [Literate Programming](https://en.wikipedia.org/wiki/Literate_programming) - Writing code as a narrative for humans.
- [API Design First](https://swagger.io/resources/articles/adopting-an-api-first-approach/) - Define APIs before implementing them.
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

- [Infrastructure as Code](https://martinfowler.com/bliki/InfrastructureAsCode.html) - Fowler's original definition of IaC.
- [Everything as Code](https://youtu.be/HcmPi7-IVQo?si=RZxxr3m7f6Q7xbgO) - Seth Vargo's talk on codification and automation in cloud environments.

## Related Awesome Lists

*Other curated lists covering related topics.*

### Infrastructure & Cloud

- [Awesome Terraform](https://github.com/shuaibiyy/awesome-terraform) - Curated list of Terraform resources and modules.
- [Awesome Pulumi](https://github.com/pulumiverse/awesome-pulumi) - Resources for Pulumi infrastructure as code.
- [Awesome Ansible](https://github.com/ansible-community/awesome-ansible) - Ansible roles, playbooks, and resources.
- [Awesome Kubernetes](https://github.com/ramitsurana/awesome-kubernetes) - Curated list for Kubernetes.
- [Awesome GitOps](https://github.com/weaveworks/awesome-gitops) - Resources for GitOps practices.
- [Awesome Policy as Code](https://github.com/hysnsec/awesome-policy-as-code) - Curated list of Policy as Code resources.

### Diagrams & Documentation

- [Awesome README](https://github.com/matiassingers/awesome-readme) - Curated list of awesome READMEs.
- [Awesome Technical Writing](https://github.com/BolajiAyodeji/awesome-technical-writing) - Technical writing resources.

### Data

- [Awesome dbt](https://github.com/Hiflylabs/awesome-dbt) - Curated list of dbt resources.
- [Awesome Data Engineering](https://github.com/igorbarinov/awesome-data-engineering) - Data engineering resources.

### Security & Policy

- [Awesome Open Policy Agent](https://github.com/StyraInc/awesome-opa) - Resources for OPA and Rego.
- [Awesome DevSecOps](https://github.com/TaptuIT/awesome-devsecops) - Security as code practices.

### Productivity

- [Awesome Markdown](https://github.com/BubuAnabelas/awesome-markdown) - Markdown tools and resources.

## Contributing

Contributions are welcome! Please read the [contribution guidelines](contributing.md) first.
