# awesome-opa

<img src="assets/awesome-opa.png" width="150"><br/><br/>

A curated list of [awesome](https://github.com/sindresorhus/awesome) Open Policy Agent (OPA) related tools, frameworks and articles.

## Contents

- [Official Projects](#official-projects)
  - [Repositories](#repositories)
  - [Docs](#docs)
  - [Blogs and Articles](#blogs-and-articles)
- [Policy Packages](#policy-packages)
- [Language and Platform Integrations](#language-and-platform-integrations)
  - [Java](#java)
  - [Python](#python)
  - [PHP](#php)
  - [.NET](#net)
  - [Node.js](#nodejs)
  - [Clojure](#clojure)
  - [Docker](#docker)
- [WebAssembly (WASM)](#webassembly-wasm)
- [Kubernetes](#kubernetes)
  - [Blogs and Articles](#blogs-and-articles)
- [Datasource Integrations](#datasource-integrations)
- [IDE and Editor Integrations](#ide-and-editor-integrations)
- [Infrastructure as Code](#infrastructure-as-code)
  - [Blogs and Articles](#infrastructure-as-code-blogs-and-articles)
- [Tools and Utilities](#tools-and-utilities)
- [Support and Community](#support-and-community)
- [Recommended Reading](#recommended-reading)

## Official projects

### Repositories

- [OPA](https://github.com/open-policy-agent/opa) - Open Policy Agent Github repository
- [Gatekeeper](https://github.com/open-policy-agent/gatekeeper) - Kubernetes admission controller using OPA
- [Conftest](https://github.com/open-policy-agent/conftest) - Write tests against structured configuration data

### Docs

- [OPA](https://www.openpolicyagent.org/docs/) - Official OPA documentation
- [Styra Academy](https://academy.styra.com/) - Excellent OPA training courses
- [Conftest](https://www.conftest.dev/) - Conftest documentation

### Blogs and Articles

- [OPA](https://blog.openpolicyagent.org/) - Official blog for the OPA project

## Policy Packages

- [Library](https://github.com/open-policy-agent/library) - Community-owned policy library for OPA
- [Policy Hub CLI](https://github.com/policy-hub/policy-hub-cli) - CLI tool that makes Rego policies searchable
- [Rego policies](https://github.com/redhat-cop/rego-policies) - Rego policies from the the Red Hat community of practice

## Language and Platform Integrations

### Java

- [Java](https://github.com/Bisnode/opa-java-client) - Generic Java client to query OPA's REST API
- [Spring Security](https://github.com/Bisnode/opa-spring-security) - OPA Spring Security Library
- [Gradle](https://github.com/Bisnode/opa-gradle-plugin) - OPA plugin for Gradle

### Python

- [OPA Python client](https://github.com/Turall/OPA-python-client) - Python client for OPA's REST API
- [Rego Python](https://github.com/open-policy-agent/rego-python) - Python package for interacting with Rego

### PHP

- [OPA Library for PHP](https://github.com/segrax/openpolicyagent) - OPA client, a PSR-15 authorization middleware and a PSR-15 bundle distributor middleware

### .NET

- [ASP.NET Core](https://github.com/build-security/OPA-AspDotNetCore-Middleware) - ASP.NET Core authorization middleware

### Node.js

- [OPA Express](https://github.com/build-security/opa-express-middleware) - OPA client for the Express framework

### Clojure

- [Clojure](https://github.com/anderseknert/clj-opa) - Middleware and utilities for app authorization with OPA in Clojure

### Docker

- [OPA Docker authorization](https://github.com/open-policy-agent/opa-docker-authz) - OPA to help policy-enable an existing services
- [Docker Security Checker](https://github.com/madhuakula/docker-security-checker) - OPA Rego policies for Dockerfile Security checks using Conftest ([blog](https://blog.madhuakula.com/dockerfile-security-checks-using-opa-rego-policies-with-conftest-32ab2316172f))
- [Dockerfile security](https://github.com/gbrindisi/dockerfile-security) - A collection of OPA rules to statically analyze Dockerfiles to improve security

## WebAssembly (WASM)

- [NPM module](https://github.com/open-policy-agent/npm-opa-wasm/) - a small SDK for using WebAssembly (wasm) compiled Open Policy Agent Rego policies
- [Go SDK](https://github.com/open-policy-agent/golang-opa-wasm) - a small Go library for using WebAssembly (wasm) compiled Open Policy Agent Rego policies
- [.NET Core Library](https://github.com/christophwille/csharp-opa-wasm) - .NET SDK for calling WASM-compiled OPA policies from .NET Core

### Docs

- [WASM](https://www.openpolicyagent.org/docs/latest/wasm/) - Official docs on WebAssembly for OPA

## Kubernetes

- [Konstraint](https://github.com/plexsystems/konstraint) - CLI tool for working with templates and constraints when using Gatekeeper
- [Deprek8ion](https://github.com/swade1987/deprek8ion) - A set of rego policies to monitor Kubernetes APIs deprecations
- [Rego Policies](https://github.com/redhat-cop/rego-policies) - Gatekeeper policies collection
- [Gatekeeper Policy Manager](https://github.com/sighupio/gatekeeper-policy-manager) - Web UI for Gatekeeper policies
- [Validating and Mutating Admission Control Example](https://github.com/tsandall/validating-and-mutating-example) - Example validating and mutation admission controller
- [Admission policy development](https://github.com/k8spin/opa-k8s-development) - OPA Kubernetes validation and mutation testing environment

### Blogs and Articles

- [Policy Enabled Kubernetes with OPA](https://www.capitalone.com/tech/software-engineering/policy-enabled-kubernetes-with-open-policy-agent/) - Guide on setting up OPA for kubernetes admission control
- [Using OPA on EKS](https://aws.amazon.com/blogs/opensource/using-open-policy-agent-on-amazon-eks/) - Using Open Policy Agent on Amazon EKS
- [OPA and Gatekeeper](https://www.infracloud.io/blogs/opa-and-gatekeeper/) - Comparison between OPA and Gatekeeper with lots of useful information
- [Kubernetes Authorization](https://itnext.io/kubernetes-authorization-via-open-policy-agent-a9455d9d5ceb) - Guide on using OPA for Kubernetes authorization

## Datasource Integrations

- [Kafka Authorizer](https://github.com/Bisnode/opa-kafka-plugin) - Kafka authorizer plugin with example policies
- [Data Filtering on Spring Data](https://github.com/jferrater/opa-data-filter-spring-boot-starter) - Data filtering for MongoDB and JPA using OPA
- [Elasticsearch](https://github.com/open-policy-agent/contrib/tree/master/data_filter_elasticsearch) - OPA-Elasticsearch Data Filtering Example
- [Strimzi](https://strimzi.io/) - Kafka in kubernetes, with built-in support for OPA as authorizer

## IDE and Editor Integrations

- [VS Code plugin](https://marketplace.visualstudio.com/items?itemName=tsandall.opa) - Develop, test, debug, and analyze policies for OPA in VS Code
- [IntelliJ plugin](https://github.com/open-policy-agent/opa-idea-plugin) - OPA plugin for the IntelliJ IDE
- [Emacs](https://github.com/psibi/rego-mode) - Emacs Major mode for working with Rego
- [Vim](https://github.com/tsandall/vim-rego) - Vim plugin for the Rego language, with support for syntax highlighting
- [Atom](https://github.com/open-policy-agent/opa/tree/master/misc/syntax/atom) - Syntax highlighting for the Atom editor
- [CodeMirror](https://github.com/StyraInc/codemirror-rego) - Rego mode and minimal key map for [CodeMirror](https://codemirror.net/)
- [TextMate](https://github.com/open-policy-agent/opa/tree/master/misc/syntax/textmate) - Syntax highlighting for TextMate
- [Sublime](https://github.com/open-policy-agent/opa/tree/master/misc/syntax/sublime) - Syntax highlighting for Sublime
- [Nano](https://github.com/scopatz/nanorc) - Syntax highlighting for Nano

## Infrastructure as Code

- [Regula](https://github.com/fugue/regula) - Evaluates Terraform code for potential security misconfigurations and compliance violations.
- [Example Terraform policies](https://github.com/Scalr/sample-tf-opa-policies) - Example Terraform policies
- [Terrascan](https://github.com/accurics/terrascan) - [500+ Policies](https://github.com/accurics/terrascan/tree/master/pkg/policies/opa/rego) written in OPA for security best practices.
- [KICS](https://github.com/Checkmarx/kics) - Keeping Infrastructure as Code Secure or KICS scans IaC projects for security vulnerabilities, compliance issues, and infrastructure misconfiguration. Currently working with Terraform projects, Kubernetes manifests, Dockerfiles, AWS CloudFormation Templates, and Ansible playbooks.

### Infrastructure as Code Blogs and Articles

- [Using OPA with Pulumi CrossGuard](https://www.pulumi.com/blog/opa-support-for-crossguard/) - Authoring Pulumi CrossGuard Policy with OPA
- [AWS CDK with OPA](https://aws.amazon.com/blogs/opensource/realize-policy-as-code-with-aws-cloud-development-kit-through-open-policy-agent/) - Realize Policy-as-Code with AWS Cloud Development Kit through Open Policy Agent
- [Kubernetes Authorization](https://itnext.io/kubernetes-authorization-via-open-policy-agent-a9455d9d5ceb) - Kubernetes Authorization via Open Policy Agent

## Tools and Utilities

- [Fregot](https://github.com/fugue/fregot) - Alternative REPL implementation for Rego
- [OPA pre-commit](https://github.com/anderseknert/pre-commit-opa) - Pre-commit hooks for OPA/Rego/Conftest development
- [Monitor OPA Gatekeeper](https://github.com/developer-guy/monitor-opa-gatekeeper) - Monitoring implementation guide for OPA Gatekeeper ([blog](https://sysdig.com/blog/monitor-gatekeeper-prometheus/))

## Support and Community

- [Styra](https://www.styra.com/) - Commercial support, and tools for managing OPA at scale, by the creators of OPA
- [Stack Overflow](https://stackoverflow.com/questions/tagged/open-policy-agent) - Stack Overflow OPA section
- [OPA Slack](https://openpolicyagent.slack.com) - Opem Policy Agent Slack workspace

## Recommended Reading

- [Microservices Security in Action](https://www.manning.com/books/microservices-security-in-action) - Book on micorservices security, with dedicated section covering OPA. Freely available online.
- [Fugue](https://www.fugue.co/blog/5-tips-for-using-the-rego-language-for-open-policy-agent-opa) - 5 tips for using the Rego language for Open Policy Agent
