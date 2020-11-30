# awesome-opa

<img src="assets/awesome-opa.png" width="150"><br/><br/>

A curated list of [awesome](https://github.com/sindresorhus/awesome) Open Policy Agent (OPA) related tools, frameworks and articles.

**WORK IN PROGRESS**

## Contents

- [Official Projects](#official-projects)
  - [Repositories](#repositories)
  - [Docs](#docs)
  - [Blogs and articles](#official-articles)
- [Language integrations](#language-integrations)
  - [Java](#java)
  - [Python](#python)
  - [PHP](#php)
  - [Docker](#docker)
- [Kubernetes](#kubernetes)
  - [Blogs and articles](#kubernetes-articles)
- [Datasource integrations](#datasource-integrations)
- [IDE and editor integrations](#ide-and-editor-integrations)
- [Infrastructure as code](#iac)
  - [Blogs and articles](#iac-articles)
- [Tools and utilities](#tools-and-utilities)
- [Support and community](#support-and-community)
- [Recommended reading](#recommended-reading)

## Official projects

### Repositories

- [OPA](https://github.com/open-policy-agent/opa) - Open Policy Agent Github repository
- [Gatekeeper](https://github.com/open-policy-agent/gatekeeper) - Kubernetes admission controller using OPA
- [Conftest](https://github.com/open-policy-agent/conftest) - Write tests against structured configuration data
- [Library](https://github.com/open-policy-agent/library) - Community-owned policy library for the OPA

### Docs

- [OPA](https://www.openpolicyagent.org/docs/) - Official OPA documentation
- [Styra Academy](https://academy.styra.com/) - Excellent OPA training courses
- [Conftest](https://www.conftest.dev/) - Conftest documentation

### Blogs and articles

- [OPA](https://blog.openpolicyagent.org/) - Official blog for the OPA project

## Language & platform integrations

### Java

- [Java](https://github.com/Bisnode/opa-java-client) - Generic Java client to query OPA's REST API
- [Spring Security](https://github.com/Bisnode/opa-spring-security) - OPA Spring Security Library
- [Gradle](https://github.com/Bisnode/opa-gradle-plugin) - OPA plugin for Gradle

### Python

- [OPA Python client](https://github.com/Turall/OPA-python-client) - Python client for OPA's REST API
- [Rego Python](https://github.com/open-policy-agent/rego-python) - Python package for interacting with Rego

### PHP

- [OPA Library for PHP](https://github.com/segrax/openpolicyagent) - OPA client, a PSR-15 authorization middleware and a PSR-15 bundle distributor middleware

### Docker

- [OPA Docker authorization](https://github.com/open-policy-agent/opa-docker-authz) - OPA to help policy-enable an existing services
- [Docker Security Checker](https://github.com/madhuakula/docker-security-checker) - OPA Rego policies for Dockerfile Security checks using Conftest ([blog](https://blog.madhuakula.com/dockerfile-security-checks-using-opa-rego-policies-with-conftest-32ab2316172f))
- [Dockerfile security](https://github.com/gbrindisi/dockerfile-security) - A collection of OPA rules to statically analyze Dockerfiles to improve security

## Kubernetes

- [Konstraint](https://github.com/plexsystems/konstraint) - CLI tool for working with templates and constraints when using Gatekeeper
- [Deprek8ion](https://github.com/swade1987/deprek8ion) - A set of rego policies to monitor Kubernetes APIs deprecations
- [Rego Policies](https://github.com/redhat-cop/rego-policies) - Gatekeeper policies collection
- [Gatekeeper Policy Manager](https://github.com/sighupio/gatekeeper-policy-manager) - Web UI for Gatekeeper policies
- [Validating and Mutating Admission Control Example](https://github.com/tsandall/validating-and-mutating-example) - Example validating and mutation admission controller
- [Admission policy development](https://github.com/k8spin/opa-k8s-development) - OPA Kubernetes validation and mutation testing environment

### Blogs and articles

- [Policy Enabled Kubernetes with OPA](https://www.capitalone.com/tech/software-engineering/policy-enabled-kubernetes-with-open-policy-agent/) - Guide on setting up OPA for kubernetes admission control
- [Using OPA on EKS](https://aws.amazon.com/blogs/opensource/using-open-policy-agent-on-amazon-eks/) - Using Open Policy Agent on Amazon EKS
- [OPA and Gatekeeper](https://www.infracloud.io/blogs/opa-and-gatekeeper/) - Comparison between OPA and Gatekeeper with lots of useful information

## Datasource integrations

- [Kafka Authorizer](https://github.com/Bisnode/opa-kafka-plugin) - Kafka authorizer plugin with example policies
- [Data Filtering on Spring Data](https://github.com/jferrater/opa-data-filter-spring-boot-starter) - Data filtering for MongoDB and JPA using OPA
- [Elasticsearch](https://github.com/open-policy-agent/contrib/tree/master/data_filter_elasticsearch) - OPA-Elasticsearch Data Filtering Example
- [Strimzi](https://strimzi.io/) - Kafka in kubernetes, with built-in support for OPA as authorizer

## IDE and editor integrations

- [VS Code plugin](https://marketplace.visualstudio.com/items?itemName=tsandall.opa) - Develop, test, debug, and analyze policies for OPA in VS Code
- [IntelliJ plugin](https://github.com/vgramer/opa-idea-plugin) - OPA plugin for the IntelliJ IDE
- [Emacs](https://github.com/psibi/rego-mode) - Emacs Major mode for working with Rego
- [Vim](https://github.com/tsandall/vim-rego) - Vim plugin for the Rego language, with support for syntax highlighting
- [Atom](https://github.com/open-policy-agent/opa/tree/master/misc/syntax/atom) - Syntax highlighting for the Atom editor
- [CodeMirror](https://github.com/StyraInc/codemirror-rego) - Rego mode and minimal key map for [CodeMirror](https://codemirror.net/)
- [TextMate](https://github.com/open-policy-agent/opa/tree/master/misc/syntax/textmate) - Syntax highlighting for TextMate
- [Sublime](https://github.com/open-policy-agent/opa/tree/master/misc/syntax/sublime) - Syntax highlighting for Sublime

## Infrastructure as code

- [Regula](https://github.com/fugue/regula) - Evaluates Terraform code for potential security misconfigurations and compliance violations.
- [Example Terraform policies](https://github.com/Scalr/sample-tf-opa-policies) - Example Terraform policies
- [Terrascan](https://github.com/accurics/terrascan) - [500+ Policies](https://github.com/accurics/terrascan/tree/master/pkg/policies/opa/rego) written in OPA for security best practices. 

### Blogs and articles

- [Using OPA with Pulumi CrossGuard](https://www.pulumi.com/blog/opa-support-for-crossguard/) - Authoring Pulumi CrossGuard Policy with OPA
- [AWS CDK with OPA](https://aws.amazon.com/blogs/opensource/realize-policy-as-code-with-aws-cloud-development-kit-through-open-policy-agent/) - Realize Policy-as-Code with AWS Cloud Development Kit through Open Policy Agent
- [Kubernetes Authorization](https://itnext.io/kubernetes-authorization-via-open-policy-agent-a9455d9d5ceb) - Kubernetes Authorization via Open Policy Agent

## Tools and utilities

- [Fregot](https://github.com/fugue/fregot) - Alternative REPL implementation for Rego
- [OPA pre-commit](https://github.com/anderseknert/pre-commit-opa) - Pre-commit hooks for OPA/Rego/Conftest development

## Support and community

- [Styra](https://www.styra.com/) - Commercial support, and tools for managing OPA at scale, by the creators of OPA
- [Stack Overflow](https://stackoverflow.com/questions/tagged/open-policy-agent) - Stack Overflow OPA section
- [OPA Slack](https://openpolicyagent.slack.com) - Opem Policy Agent Slack workspace

## Recommended reading

- [Fugue](https://www.fugue.co/blog/5-tips-for-using-the-rego-language-for-open-policy-agent-opa) - 5 tips for using the Rego language for Open Policy Agent
