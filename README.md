# awesome-opa

A curated list of Open Policy Agent (OPA) related tools, frameworks and articles.

**WORK IN PROGRESS**

## Contents

- [Official Projects](#official-projects)
  - [Repositories](#repositories)
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

## Official projects

### Repositories

- [OPA](https://github.com/open-policy-agent/opa) - Open Policy Agent Github repository
- [Gatekeeper](https://github.com/open-policy-agent/gatekeeper) - Kubernetes admission controller using OPA
- [Conftest](https://github.com/open-policy-agent/conftest) - Write tests against structured configuration data

## Language & platform integrations

### Java

- [Java](https://github.com/Bisnode/opa-java-client) - Generic Java client to query OPA's REST API
- [Spring Security](https://github.com/Bisnode/opa-spring-security) - OPA Spring Security Library
- [Gradle](https://github.com/Bisnode/opa-gradle-plugin) - OPA plugin for Gradle

### Python

- [OPA Python client](https://github.com/Turall/OPA-python-client) - Python client for OPA's REST API
- [Rego Python](https://github.com/open-policy-agent/rego-python) - Python package for interacting with Rego

### PHP

- [OPA Library for PHP](https://github.com/segrax/openpolicyagent) - OPA client, a PSR-15 authorization middleware and a PSR-15 bundle distributor middleware.

### Docker

- [OPA Docker authorization](https://github.com/open-policy-agent/opa-docker-authz) - OPA to help policy-enable an existing services

## Kubernetes

### Blogs and articles

- [Policy Enabled Kubernetes with OPA](https://www.capitalone.com/tech/software-engineering/policy-enabled-kubernetes-with-open-policy-agent/) - Guide on setting up OPA for kubernetes admission control
- [Using OPA on EKS](https://aws.amazon.com/blogs/opensource/using-open-policy-agent-on-amazon-eks/) - Using Open Policy Agent on Amazon EKS

## Datasource integrations

- [Kafka authorizer](https://github.com/Bisnode/opa-kafka-plugin) - Kafka authorizer plugin with example policies
- [Data Filtering on Spring Data](https://github.com/jferrater/opa-data-filter-spring-boot-starter) - Data filtering for MongoDB and JPA using OPA
- [Elasticsearch](https://github.com/open-policy-agent/contrib/tree/master/data_filter_elasticsearch) - OPA-Elasticsearch Data Filtering Example

## IDE and editor integrations

- [VS Code plugin](https://marketplace.visualstudio.com/items?itemName=tsandall.opa) - Develop, test, debug, and analyze policies for OPA in VS Code
- [IntelliJ plugin](https://github.com/vgramer/opa-idea-plugin) - OPA plugin for the IntelliJ IDE
- [CodeMirror](https://github.com/StyraInc/codemirror-rego) - Rego mode and minimal key map for [CodeMirror](https://codemirror.net/)

## Infrastructure as code

- [Regula](https://github.com/fugue/regula) - Evaluates Terraform code for potential security misconfigurations and compliance violations.
- [Example Terraform policies](https://github.com/Scalr/sample-tf-opa-policies) - Example Terraform policies

### Blogs and articles

- [Using OPA with Pulumi CrossGuard](https://www.pulumi.com/blog/opa-support-for-crossguard/) - Authoring Pulumi CrossGuard Policy with OPA
- [AWS CDK with OPA](https://aws.amazon.com/blogs/opensource/realize-policy-as-code-with-aws-cloud-development-kit-through-open-policy-agent/) - Realize Policy-as-Code with AWS Cloud Development Kit through Open Policy Agent

## Tools and utilities

- [OPA pre-commit hooks](https://github.com/anderseknert/pre-commit-opa) - Pre-commit hooks for OPA/Rego/Conftest development

## Support and community

- [Styra](https://www.styra.com/) - Commercial support, and tools for managing OPA at scale, by the creators of OPA
- [Stack Overflow](https://stackoverflow.com/questions/tagged/open-policy-agent) - Stack Overflow OPA section
- [OPA Slack](https://openpolicyagent.slack.com) - Opem Policy Agent Slack workspace

