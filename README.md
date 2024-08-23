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
  - [Go](#go)
  - [PHP](#php)
  - [.NET](#net)
  - [Node.js](#nodejs)
  - [Clojure](#clojure)
  - [Docker](#docker)
  - [CPP](#cpp)
  - [Rust](#rust)
  - [Typescript]("#typescript")
- [WebAssembly (Wasm)](#webassembly-wasm)
  - [Blogs and Articles](#webassembly-blogs-and-articles)
- [Kubernetes](#kubernetes)
  - [Service Mesh Authorization](#service-mesh-authorization)
  - [Blogs and Articles](#blogs-and-articles)
- [Nomad](#nomad)
- [Datasource Integrations](#datasource-integrations)
  - [Blogs and Articles](#datasource-integrations-blogs-and-articles)
- [IDE and Editor Integrations](#ide-and-editor-integrations)
- [Infrastructure as Code](#infrastructure-as-code)
  - [Blogs and Articles](#infrastructure-as-code-blogs-and-articles)
- [Serverless](#serverless)
  - [Blogs and Articles](#serverless-blogs-and-articles)
- [Testing](#testing)
  - [Blogs and Articles](#testing-blogs-and-articles)
- [Tools and Utilities](#tools-and-utilities)
- [Other Usecases](#other-usecases)
- [Fun and Quirky](#fun-and-quirky)
- [Support and Community](#support-and-community)
- [Recommended Reading](#recommended-reading)
- [People](#people)
  - [Maintainers](#maintainers)
  - [Community Stars](#community-stars)
  - [Meetup Groups](#meetup-groups)
- [Commercial Tools](#commercial-tools)
- [Contributing](#contributing)

## Official projects

### Repositories

- [OPA](https://github.com/open-policy-agent/opa) - Open Policy Agent Github repository
- [Gatekeeper](https://github.com/open-policy-agent/gatekeeper) - Kubernetes admission controller using OPA
- [Conftest](https://github.com/open-policy-agent/conftest) - Write tests against structured configuration data

### Docs

- [OPA](https://www.openpolicyagent.org/docs/) - Official OPA documentation
- [Styra Academy](https://academy.styra.com/) - Excellent OPA training courses
- [Gatekeeper](https://open-policy-agent.github.io/gatekeeper/website/docs/) - OPA Gatekeeper docs
- [Conftest](https://www.conftest.dev/) - Conftest documentation
- [Rego Style Guide](https://github.com/StyraInc/rego-style-guide) - Style guide for Rego, providing pointers on best practices for policy authoring
- [Regal Docs](https://docs.styra.com/regal) - Documentation for 60+ linter rules, providing an excellent reference for learning Rego

### Blogs and Articles

- [OPA](https://blog.openpolicyagent.org/) - Official blog for the OPA project
- [Logo](https://cncf-branding.netlify.app/projects/opa/) - The OPA Logo in different versions

## Policy Packages

- [Library](https://github.com/open-policy-agent/library) - Community-owned policy library for OPA
- [Policy Hub CLI](https://github.com/policy-hub/policy-hub-cli) - CLI tool that makes Rego policies searchable
- [Rego policies](https://github.com/redhat-cop/rego-policies) - Rego policies from the the Red Hat community of practice
- [Appshield](https://github.com/aquasecurity/appshield) - Open Database of rego policies for common Infrastructure as Code files
- [Conftest policy packs](https://github.com/rallyhealth/conftest-policy-packs) - Collection of Conftest policies for "Compliance-as-Code" security policies and general engineering standards. Policies targeting Terraform, Dockerfiles, package.json (NodeJS) files, etc
- [Confectionary](https://github.com/Cigna/confectionery) - A library of rules for Conftest used to detect Terraform misconfigurations.
- [Kubescape Rego library](https://github.com/kubescape/regolibrary) - Comprehensive set of Kubernetes policies from Kubescape
- [Kubernetes Security Policies](https://github.com/raspbernetes/k8s-security-policies) - Raspernetes library for fortifying cluster configurations

## Language and Platform Integrations

### Java

- [Styra Java SDK](https://github.com/StyraInc/opa-java) - Java SDK for interacting with OPA ([documentation](https://docs.styra.com/sdk))
- [Jarl](https://github.com/johanfylling/jarl) - Native evaluation of Rego in the JVM, via OPA's IR format ([blog](https://blog.openpolicyagent.org/i-have-a-plan-exploring-the-opa-intermediate-representation-ir-format-7319cd94b37d))
- [OPA Java Client](https://github.com/Bisnode/opa-java-client) - Generic Java client to query OPA's REST API
- [Spring Security](https://github.com/Bisnode/opa-spring-security) - OPA Spring Security Library
- [Spring Security Reactive](https://github.com/massenz/jwt-opa) - OPA with Spring Security Reactive
- [Gradle](https://github.com/Bisnode/opa-gradle-plugin) - OPA plugin for Gradle
- [Thunx](https://github.com/xenit-eu/thunx) - Thunx is a pluggable ABAC system using OPA, Spring Cloud Gateway and Spring Data REST

### Python

- [OPA Python](https://github.com/heliconhq/opa-python) - Python client library for Open Policy Agent
- [OPA Python client](https://github.com/Turall/OPA-python-client) - Python client for OPA's REST API
- [Flask OPA](https://github.com/EliuX/flask-opa) - OPA client for the Flask microframework
- [Bottle Authorization](https://github.com/dolevf/bottle-acl-openpolicyagent) - Custom Bottle Application Authorization
- [Rego Python](https://github.com/open-policy-agent/rego-python) - Python package for interacting with Rego
- [Sphinx Rego](https://github.com/zenitysec/sphinx-rego) - Sphinx extension that automatically documents Rego policies
- [regopy](https://pypi.org/project/regopy/) - Python module which uses the C FFI for rego-cpp, allowing in-process Pythonic Rego policy evaluation
- [regorus](https://github.com/microsoft/regorus/tree/main/bindings/python) - Evaluate Rego policies in Python using Regorus, a fast, lightweight Rego interpreter written in Rust.

### Go

- [Go Example API Authorization](https://github.com/open-policy-agent/example-api-authz-go) - Example API authorization using OPA
- [Fiber OPA Integration](https://github.com/gofiber/contrib/tree/main/opafiber) - OPA integration for Fiber web framework. Enables to execute Rego policies in the middlewares.
- [HTTP API OPA middlewares](https://github.com/Joffref/opa-middleware) - Collection of OPA middlewares for your HTTP/Gin/Fiber API.
- [regorus](https://github.com/microsoft/regorus/tree/main/bindings/go) - Golang bindings to Regorus, a fast, lightweight Rego interpreter written in Rust.

### PHP

- [OPA Library for PHP](https://github.com/segrax/openpolicyagent) - OPA client, a PSR-15 authorization middleware and a PSR-15 bundle distributor middleware

### .NET

- [Styra C# SDK](https://github.com/StyraInc/opa-csharp) - C# SDK for interacting with OPA ([documentation](https://docs.styra.com/sdk))
- [ASP.NET Core](https://github.com/build-security/OPA-AspDotNetCore-Middleware) - ASP.NET Core authorization middleware
- [OpaDotNet.Extensions.AspNetCore](https://github.com/me-viper/OpaDotNet.Extensions) - ASP.NET Core authorization infrastructure
- [regorus](https://github.com/microsoft/regorus/tree/main/bindings/csharp) - C# bindings to Regorus, a fast, lightweight Rego interpreter written in Rust.

### Node.js

- [OPA Express](https://github.com/build-security/opa-express-middleware) - OPA client for the Express framework
- [regorus](https://github.com/microsoft/regorus/tree/main/bindings/wasm) - Evaluate Rego policies in WASM using Regorus. Try it out at [Regorus Playground](https://anakrish.github.io/regorus-playground/).

### Clojure


- [Jarl](https://github.com/johanfylling/jarl) - Native evaluation of Rego in the JVM (written in Clojure), via OPA's IR format ([blog](https://blog.openpolicyagent.org/i-have-a-plan-exploring-the-opa-intermediate-representation-ir-format-7319cd94b37d))
- [clj-opa](https://github.com/anderseknert/clj-opa) - Middleware and utilities for app authorization with OPA in Clojure

### Docker

- [OPA Docker authorization](https://github.com/open-policy-agent/opa-docker-authz) - OPA to help policy-enable an existing services
- [Docker Security Checker](https://github.com/madhuakula/docker-security-checker) - OPA Rego policies for Dockerfile Security checks using Conftest
- [Dockerfile security](https://github.com/gbrindisi/dockerfile-security) - A collection of OPA rules to statically analyze Dockerfiles to improve security

### Containers

 - [Konveyor Forklift Validation Service](https://github.com/konveyor/forklift-validation) - VM migration suitability assessment to avoid migrating VMs that are not fit for Kubevirt. Rules are applied on all the VMs of the source provider (VMware) during the initial inventory collection, then whenever a VM configuration changes.

### CPP

- [rego-cpp](https://microsoft.github.io/rego-cpp/) - Rego compiler and runtime implemented in C++. It provides a C FFI with Rust and Python bindings in addition to an extensible C++ implementation.
- [regorus](https://github.com/microsoft/regorus/tree/main/bindings/cpp) - C++ bindings to Regorus, a fast, lightweight Rego interpreter written in Rust.

### Rust

- [regorus](https://crates.io/crates/regorus) - A fast, lightweight Rego interpreter written in Rust. In addition to bringing the power of Rego to Rust-only environments, it is intended as a platform for developing Rego tools and exploring Rego language enhancements.
- [regorust](https://crates.io/crates/regorust) - Rust crate wrapping the C FFI for rego-cpp, allowing in-process Rego policy evaluation using idiomatic Rust.

### Typescript

- [Styra OPA Typescript SDK](https://github.com/StyraInc/opa-typescript) - Typescript SDK for interacting with OPA ([documentation](https://docs.styra.com/sdk))

## WebAssembly (Wasm)

- [NPM module](https://github.com/open-policy-agent/npm-opa-wasm/) - a small SDK for using WebAssembly compiled Open Policy Agent Rego policies
- [.NET Core Library](https://github.com/christophwille/csharp-opa-wasm) - .NET SDK for calling Wasm-compiled OPA policies from .NET Core
- [OpaDotNet](https://github.com/me-viper/OpaDotNet) - Open Policy Agent (OPA) WebAssembly dotnet core SDK
- [OpaDotNet.Compilation](https://github.com/me-viper/OpaDotNet.Compilation) - dotnet core backend for packaging Open Policy Agent Rego policies and data files into WASM policy bundles
- [Python Library](https://github.com/a2d24/python-opa-wasm) - Open Policy Agent WebAssembly SDK for Python
- [Go SDK](https://github.com/open-policy-agent/opa/tree/main/internal/wasm/sdk) - a small Go library for using WebAssembly compiled Open Policy Agent Rego policies
- [JVM](https://github.com/sangkeon/java-opa-wasm) - Java SDK for calling Wasm-compiled policies. Uses wasmtime.
- [Rust](https://github.com/matrix-org/rust-opa-wasm) - A crate to use OPA policies compiled to Wasm.
- [regorus](https://github.com/microsoft/regorus/tree/main/bindings/wasm) - Evaluate Rego policies in WASM using Regorus. Try it out at [Regorus Playground](https://anakrish.github.io/regorus-playground/).

### WebAssembly Blogs and Articles
- [Enforce policies in the browser with Open Policy Agent](https://medium.com/@robertgartman/enforce-policies-in-the-browser-with-open-policy-agent-22d8e32fbfb6?source=friends_link&sk=b7a58aecd84bf7367622347a91772947) - _first_ article in a series of three covering why and how to reuse backend Policy-as-Code in the browser.
- [Reuse Policy as Code — stay DRY](https://medium.com/@robertgartman/reuse-policy-as-code-stay-dry-7ad1229be160?source=friends_link&sk=196fd624a4027f5c33366f596dc75935) - _second_ article in a series of three covering why and how to reuse backend Policy-as-Code in the browser. This article focus on Rego and HOW
- [OPA & Angular: Policy-as-Code in the browser](https://medium.com/@robertgartman/opa-angular-policy-as-code-in-the-browser-7bb3e5a8f60c?source=friends_link&sk=69f87b120d716a4f4f7abe5d3e1680ec) - _third_ article in a series of three covering why and how to reuse backend Policy-as-Code in the browser. Angular Proof of Concept based on article 1 & 2.
- [Rego on WebAssembly](https://blog.openpolicyagent.org/opa-v0-15-1-rego-on-webassembly-81c226c51be4) - original OPA Wasm support blog post which summarizes how OPA's Wasm functionality works.

### Docs

- [Wasm](https://www.openpolicyagent.org/docs/latest/wasm/) - Official docs on WebAssembly for OPA

### Built with Wasm

- [OPA Wasm demo](https://opa-wasm.glitch.me/) - Demonstration of evaluating OPA's Wasm modules in the browser
- [Snyk CLI](https://github.com/snyk/snyk) - Test Infrastructure as Code source code for security misconfigurations and best practices in the local console. The npm-opa-wasm library is used to run WASM bundle of Rego policies to detect misconfiguration.
- [regorus](https://github.com/microsoft/regorus/tree/main/bindings/wasm) - Evaluate Rego policies in WASM using Regorus. Try it out at [Regorus Playground](https://anakrish.github.io/regorus-playground/).

## Kubernetes

- [Gatekeeper](https://github.com/open-policy-agent/gatekeeper) - A validating and mutating webhook that enforces CRD-based policies executed by OPA for Kubernetes
- [Gatekeeper Policy Library](https://www.github.com/open-policy-agent/gatekeeper-library) - A collection of constraint templates and sample constraints that you can use with Gatekeeper
- [Konstraint](https://github.com/plexsystems/konstraint) - CLI tool for working with templates and constraints when using Gatekeeper
- [Red Hat Rego Policies](https://github.com/redhat-cop/rego-policies) - Red Hat Rego policies collection
- [Gatekeeper Policy Manager](https://github.com/sighupio/gatekeeper-policy-manager) - Web UI for Gatekeeper policies
- [Validating and Mutating Admission Control Example](https://github.com/tsandall/validating-and-mutating-example) - Example validating and mutation admission controller
- [MagTape](https://github.com/tmobile/magtape) - OPA-based admission controller for policy enforcement
- [Meshery](https://meshery.io/) - Meshery leverages built-in relationships to enforce Kubernetes configuration best practices and enhances the development process through custom rules in OPA's Rego query language
- [Admission policy development](https://github.com/k8spin/opa-k8s-development) - OPA Kubernetes validation and mutation testing environment
- [Gatekeeper Conftest plugin](https://github.com/clover/gatekeeper-conftest) - A Conftest plugin that transforms input objects to be compatible with OPA Gatekeeper policies.
- [Cosign Gatekeeper Provider](https://github.com/developer-guy/cosign-gatekeeper-provider) - Cosign Provider a new provider of OPA Gatekeeper's ExternalData feature to verify container images
- [Kubescape](https://github.com/armosec/kubescape) - Kubescape is tool for scanning Kubernetes clusters for security issues. Kubescape tests (rules) are based completely on OPA. See the regos [here](https://github.com/armosec/regolibrary)
- [Kove](https://github.com/cmacrae/kove) - Watch your in-cluster Kubernetes manifests for OPA policy violations and export them as Prometheus metrics
- [GKE Policy Automation](https://github.com/google/gke-policy-automation) - Tool and policy library for reviewing GKE clusters against best practices

### Service Mesh Authorization

- [OPA Envoy Plugin](https://github.com/open-policy-agent/opa-envoy-plugin) - The OPA Envoy Plugin (compatible with Envoy, Istio, Gloo Edge, more)
- [Open Service Mesh](https://release-v0-11.docs.openservicemesh.io/docs/guides/integrations/external_auth_opa/#osm-with-opa-plugin-external-authorization-walkthrough) - Envoy based service mesh using OPA for external authorization
- [Kuma](https://konghq.com/videos/microservice-authorization-with-open-policy-agent-and-kuma/) - OPA for Kuma service mesh
- [Kong Mesh](https://konghq.com/blog/kong-service-mesh-and-opa-policy/) - OPA for Kong Mesh authorization ([docs](https://docs.konghq.com/mesh/1.5.x/features/opa/))

### Blogs and Articles

- [Policy Enabled Kubernetes with OPA](https://www.capitalone.com/tech/software-engineering/policy-enabled-kubernetes-with-open-policy-agent/) - Guide on setting up OPA for kubernetes admission control
- [Integrating OPA with Kubernetes](https://techblost.com/integrating-open-policy-agent-opa-with-kubernetes/) - Comprehensive introduction to OPA and Gatekeeper
- [Using OPA on EKS](https://aws.amazon.com/blogs/opensource/using-open-policy-agent-on-amazon-eks/) - Using Open Policy Agent on Amazon EKS
- [OPA and Gatekeeper](https://www.infracloud.io/blogs/opa-and-gatekeeper/) - Comparison between OPA and Gatekeeper with lots of useful information
- [Kubernetes Authorization](https://itnext.io/kubernetes-authorization-via-open-policy-agent-a9455d9d5ceb) - Guide on using OPA for Kubernetes authorization
- [Gatekeeper in a CI/CD pipeline](https://arapulido.github.io/blog/2021/08/02/testing-your-kubernetes-config-against-policy-ci/) - Guide on how to setup your CI environment to test your Kubernetes configuration against your policy in a CI environment as part of a GitOps strategy
- [Verifying container signatures on Kubernetes with Gatekeeper](https://medium.com/@LachlanEvenson/verifying-container-signatures-on-kubernetes-with-gatekeeper-19a4519c3016) - Verifying container signatures on Kubernetes with Gatekeeper
- [Gator CLI](https://medium.com/@LachlanEvenson/testing-gatekeeper-constraints-with-gator-cli-da31050a6564) - Testing Gatekeeper constraints with Gator CLI
- [Kubernetes: An Enterprise Guide, 2nd Ed Chapter 8 - Extending Security with OpenPolicyAgent](https://youtu.be/_GQZ8Qahu48) - Walk through labs that show you how to build, debug, and deploy GateKeeper policies and mutations in your cluster.
- [Kubernetes: An Enterprise Guide, 2nd Ed Chapter 9 - Node Security with GateKeeper](https://youtu.be/UrSvh74n24E) - Walk through labs that show the differences between VMs and containers with a breakout, creating `securityContext` defaults using mutations, replacing `PodSecurityPolicy` using GateKeeper, debuging audit violations, and policies for multi-tenant clusters.
- [OPA Gatekeeper: Policy and Governance for Kubernetes](https://kubernetes.io/blog/2019/08/06/opa-gatekeeper-policy-and-governance-for-kubernetes/) - Kubernetes blog post
- [Using OPA Gatekeeper on Azure](https://docs.microsoft.com/en-us/azure/governance/policy/concepts/policy-for-kubernetes) - Azure Policy for Kubernetes clusters

## Nomad

- [Nomad Admission Control Proxy](https://github.com/mxab/nacp) - An admission controller that can be used as a proxy to Nomad's API for mutation and validation with builtin OPA support.

## Datasource Integrations

- [Kafka Authorizer](https://github.com/StyraInc/opa-kafka-plugin) - Kafka authorizer plugin using OPA, with example policies
- [OPA Single Message Transformer](https://github.com/opencredo/opa-single-message-transformer) - Single Message Transformer for Kafka. Uses OPA to choose which records to filter out based on policy.
- [Data Filtering on Spring Data](https://github.com/jferrater/opa-data-filter-spring-boot-starter) - Data filtering for MongoDB and JPA using OPA
- [Elasticsearch](https://github.com/open-policy-agent/contrib/tree/master/data_filter_elasticsearch) - OPA-Elasticsearch Data Filtering Example
- [Strimzi](https://strimzi.io/) - Kafka in kubernetes, with built-in support for OPA as authorizer
- [Google Calendar](https://github.com/anderseknert/opa-google-calendar) - Integrating OPA with the Google Calendar API
- [Inspektor](https://github.com/poonai/inspektor) - Access Control as Code for databases using OPA to make its access decision
- [Alluxio](https://www.alluxio.io/) - Alluxio is a data orchestration tool which allows [delegating access control decisions to OPA](https://docs.alluxio.io/ee/user/2.10.0/en/security/OpenPolicyAgent-Integration.html)
- [Trino OPA Authorizer](https://github.com/stackabletech/trino-opa-authorizer/) - Plugin for Trino that allows using OPA for authorization

### Datasource Integrations Blogs and Articles

- [Google Calendar Integration](https://blog.styra.com/blog/the-power-of-data-calendar-based-policy-enforcement) - The Power of Data: Calendar-based Policy Enforcement
- [Apache Kafka](https://opencredo.com/blogs/controlling-kafka-data-flows-using-open-policy-agent/) - Controlling Kafka Data Flows using Open Policy Agent

## IDE and Editor Integrations

- [VS Code plugin](https://marketplace.visualstudio.com/items?itemName=tsandall.opa) - Develop, test, debug, and analyze policies for OPA in VS Code
- [IntelliJ plugin](https://github.com/open-policy-agent/opa-idea-plugin) - OPA plugin for the IntelliJ IDE
- [Zed Extension](https://github.com/StyraInc/zed-rego) - Zed extension for OPA and Rego leveraging [Regal](https://docs.styra.com/regal)
- [Emacs](https://github.com/psibi/rego-mode) - Emacs Major mode for working with Rego
- [Vim](https://github.com/tsandall/vim-rego) - Vim plugin for the Rego language, with support for syntax highlighting
- [Null-ls](https://github.com/jose-elias-alvarez/null-ls.nvim) - Use Neovim as a language server to inject LSP diagnostics, code actions, and more. Supports linting rego files.
- [Atom](https://github.com/open-policy-agent/opa/tree/master/misc/syntax/atom) - Syntax highlighting for the Atom editor
- [CodeMirror](https://github.com/StyraInc/codemirror-rego) - Rego mode and minimal key map for [CodeMirror](https://codemirror.net/)
- [TextMate](https://github.com/open-policy-agent/opa/tree/master/misc/syntax/textmate) - Syntax highlighting for TextMate
- [Sublime](https://github.com/open-policy-agent/opa/tree/master/misc/syntax/sublime) - Syntax highlighting for Sublime
- [Nano](https://github.com/scopatz/nanorc) - Syntax highlighting for Nano
- [Prism](https://prismjs.com/) - Prism is a lightweight, extensible syntax highlighter, built with modern web standards in mind (supports Rego)
- [tree-sitter-rego](https://github.com/FallenAngel97/tree-sitter-rego) - Tree-sitter grammar for Rego ([blog](https://decodeapps.pp.ua/blog/post/rego-treesitter))

## Infrastructure as Code

- [OPA AWS CloudFormation Hook](https://github.com/StyraInc/opa-aws-cloudformation-hook) - AWS CloudFormation Hook calling OPA for policy decisions. See also [tutorial](https://www.openpolicyagent.org/docs/latest/aws-cloudformation-hooks/).
- [TFLint OPA Ruleset](https://github.com/terraform-linters/tflint-ruleset-opa) - Write custom TFLint rules in Rego
- [Infracost](https://github.com/infracost/infracost/) - Infracost generates cloud cost estimates for Terraform and integrates with OPA, it can be used to write [cost policies](https://www.infracost.io/docs/features/cost_policies/)
- [Regula](https://github.com/fugue/regula) - Evaluates Terraform code for potential security misconfigurations and compliance violations.
- [Example Terraform policies](https://github.com/Scalr/sample-tf-opa-policies) - Example Terraform policies
- [Terrascan](https://github.com/accurics/terrascan) - [500+ Policies](https://github.com/accurics/terrascan/tree/master/pkg/policies/opa/rego) written in OPA for security best practices.
- [KICS](https://github.com/Checkmarx/kics) - Keeping Infrastructure as Code Secure or KICS scans IaC projects for security vulnerabilities, compliance issues, and infrastructure misconfiguration. Currently working with Terraform projects, Kubernetes manifests, Dockerfiles, AWS CloudFormation Templates, and Ansible playbooks.
- [Trivy](https://github.com/aquasecurity/trivy) - Scan your code and artifacts for known vulnerabilities and misconfiguration issues.
- [Terraform OPA IBM](https://github.com/IBM-Cloud/terraform-opa-ibm) - Terraform policy library for IBM Cloud
- [GCP policy guardrails for Terraform](https://github.com/GoogleCloudPlatform/policy-library/tree/main/validator) - Rego reference policy library for GCP controls (originally from forseti). Originally used by `terraform-validator` and now on `gcloud beta terraform vet`. More info at [Policy Validation](https://cloud.google.com/docs/terraform/policy-validation)
- [Pulumi OPA Bridge for CrossGuard](https://github.com/pulumi/pulumi-policy-opa) - This project allows OPA rules to be run in the context of Pulumi's policy system, CrossGuard

### Infrastructure as Code Blogs and Articles

- [Using OPA with Pulumi CrossGuard](https://www.pulumi.com/blog/opa-support-for-crossguard/) - Authoring Pulumi CrossGuard Policy with OPA
- [AWS CDK with OPA](https://aws.amazon.com/blogs/opensource/realize-policy-as-code-with-aws-cloud-development-kit-through-open-policy-agent/) - Realize Policy-as-Code with AWS Cloud Development Kit through Open Policy Agent
- [Kubernetes Authorization](https://itnext.io/kubernetes-authorization-via-open-policy-agent-a9455d9d5ceb) - Kubernetes Authorization via Open Policy Agent
- [Using OPA with Spacelift](https://spacelift.io/blog/what-is-open-policy-agent-and-how-it-works) - Open Policy Agent: What Is OPA and How It Works (Examples)

## Serverless

- [OPA Lambda Extension Plugin](https://github.com/godaddy/opa-lambda-extension-plugin) - A custom plugin for running OPA in AWS Lambda as a Lambda Extension

### Serverless Blogs and Articles

- [Serverless Policy Enforcement](https://blog.openpolicyagent.org/serverless-policy-enforcement-connecting-opa-and-aws-lambda-e624f7176a3) - Connecting Open Policy Agent and AWS Lambda
- [Lambda Authorizer](https://aws.amazon.com/blogs/opensource/creating-a-custom-lambda-authorizer-using-open-policy-agent/) - Creating a custom Lambda authorizer using Open Policy Agent

## Testing

- [rego-test-assertions](https://github.com/anderseknert/rego-test-assertions) - Helper library for working with assertions in Rego unit tests
- [kube-review](https://github.com/anderseknert/kube-review) - CLI tool to quickly create [AdmissionReview](https://kubernetes.io/docs/reference/access-authn-authz/extensible-admission-controllers/) requests from Kubernetes resources
- [gator CLI](https://open-policy-agent.github.io/gatekeeper/website/docs/gator/) - Command line unit test runner for OPA Gatekeeper
- [ocov](https://github.com/C5T/ocov) - Colors `opa test --coverage` reports in the terminal
- [opa-codecov](https://github.com/SVilgelm/opa-codecov) - Convert OPA test coverage report to a JSON format supported by Codecov

### Testing Blogs and Articles

- [Advanced Rego Testing Techniques](https://www.styra.com/blog/advanced-rego-testing-techniques/) - Great blog on testing patterns for Rego, by Nicholaos Mouzourakis

## Tools and Utilities

- [Regal](https://github.com/StyraInc/regal) - Regal is a linter for Rego, with the goal of making your Rego magnificent! ([blog](https://www.styra.com/blog/guarding-the-guardrails-introducing-regal-the-rego-linter/))
- [setup-opa](https://github.com/open-policy-agent/setup-opa) - GitHub action to configure the Open Policy Agent CLI in your GitHub Actions workflows
- [Fregot](https://github.com/fugue/fregot) - Alternative REPL implementation for Rego
- [OPA pre-commit](https://github.com/anderseknert/pre-commit-opa) - Pre-commit hooks for OPA/Rego/Conftest development
- [Monitor OPA Gatekeeper](https://github.com/developer-guy/monitor-opa-gatekeeper) - Monitoring implementation guide for OPA Gatekeeper ([blog](https://sysdig.com/blog/monitor-gatekeeper-prometheus/))
- [OpenAPI to Rego](https://github.com/ashutosh-narkar/openapi-to-rego) - Generate Rego code given an OpenAPI 3.0 Specification
- [Temporal reasoning with OPA](https://github.com/mhausenblas/temporal-opa) - Examples for working with time in Rego
- [OPAL](https://github.com/authorizon/opal) - Realtime policy and data updates for your OPA agents on top of websockets pub/sub
- [OPA Action](https://github.com/koozz/opa-action) - OPA Pull-Request Assessor is a GitHub Action that checks files against policies configured in the same repo
- [OPA Schema Examples](https://github.com/aavarghese/opa-schema-examples) - Examples of extending the OPA type checker with JSON [schemas](https://www.openpolicyagent.org/docs/latest/schemas/)
- [Open Policy Containers](https://github.com/opcr-io/policy) - Secure software supply chains for OPA policies. Push, pull, tag, test, version, and sign OPA policies.
- [Snyk IaC Rules](https://github.com/snyk/snyk-iac-rules) - Maintain library of Rego rules, run integration tests and build WASM bundles for distribution of rules. The OPA libraries are used to build WASM bundles.
- [Topaz](https://github.com/aserto-dev/topaz) - Topaz is an open-source application authorization project that uses OPA as the decision engine and supports Rego policies.
- [opactl](https://github.com/onelittlenightmusic/opactl) - A simple tool to turn your Rego rule into CLI command ([blog](https://itnext.io/implement-a-policy-and-use-it-in-cli-de906237c6ab))
- [alfred](https://github.com/dolevf/Open-Policy-Agent-Alfred) - A self-hosted OPA Playground Alternative
- [Rönd](https://github.com/rond-authz/rond) - Rönd is a lightweight container that distributes security policy enforcement throughout your application
- [rq (Rego Query)](https://git.sr.ht/~charles/rq) - jq-inspired tool to bring Rego to your shell pipelines
- [opa-explorer](https://github.com/srenatus/opa-explorer) - Visual tool for exploring the different compilation stages of the OPA topdown compiler
- [mcov](https://github.com/styrainc/mcov) - A tool that'll check your Rego source files and report the minimum compatible OPA version required
- [dependency-management-data (DMD)](https://dmd.tanna.dev) is a set of tooling to get a better understanding of the use of dependencies across your organisation. DMD supports using Open Policy Agent to write more complex rules around dependency usage than can be done using the SQL interface.

## Other Usecases

- [SansShell](https://github.com/Snowflake-Labs/sansshell) - A non-interactive daemon for host management, where any action is authorized by OPA
- [goast](https://github.com/m-mizutani/goast) - Go AST (Abstract Syntax Tree) based static analysis tool using Rego
- [ScubaGear](https://github.com/cisagov/ScubaGear/) - Using Rego policies to assess the security posture of M365 tenants, by CISA
- [Reposaur](https://github.com/reposaur/reposaur) - Audit, verify and report on development platforms (GitHub and others) easily with pre-defined and/or custom policies.

## Fun and Quirky

- [How I Used OPA to Help Me Solve Wordle](https://www.styra.com/blog/how-i-used-opa-to-help-me-solve-wordle/) - OPA as a Wordle assistant
- [Policing Christmas Tree](https://github.com/charlieegan3/policing-christmas-trees) - Using Rego to determine the correctness of Christmas tree decorations
- [Corrupting OPA to Run My Games](https://kevinhoffman.medium.com/corrupting-the-open-policy-agent-to-run-my-game-711f340adb5a) - Fun blog on using OPA for game engines
- [Colorized](https://github.com/anderseknert/colorized) - Colorized output for the OPA print function!

## Support and Community

- [Styra](https://www.styra.com/) - Commercial support, and tools for managing OPA at scale, by the creators of OPA
- [Stack Overflow](https://stackoverflow.com/questions/tagged/open-policy-agent) - Stack Overflow OPA section
- [OPA Slack](https://openpolicyagent.slack.com) - Open Policy Agent Slack workspace
- [GitHub Discussions](https://github.com/open-policy-agent/feedback/discussions) - Open Policy Agent Discussion Board

## Recommended Reading

- [OPA Guidebook](https://sangkeon.github.io/opaguide/) - Open source, free book on Open Policy Agent, by Sangkeon Lee ([source code](https://github.com/sangkeon/opaguide_src))
- [Microservices Security in Action](https://www.manning.com/books/microservices-security-in-action) - Book on microservices security, with dedicated section covering OPA. Freely available online
- [Gusto Engineering](https://engineering.gusto.com/why-logic-programming-is-the-best-choice-for-authorization/) — Why logic programming is the best choice for authorization
- [Fugue](https://www.fugue.co/blog/5-tips-for-using-the-rego-language-for-open-policy-agent-opa) - 5 tips for using the Rego language for Open Policy Agent
- [Integration](https://snowplowanalytics.com/blog/2021/12/07/how-we-integrated-our-purely-functional-scala-backend-with-the-open-policy-agent/) - How we integrated our purely functional Scala backend with the Open Policy Agent
- [Integration](https://medium.com/@nikman/control-user-access-and-permissions-in-cvat-with-open-policy-agent-a2abbd09774d) - Control User Access and Permissions in CVAT with Open Policy Agent

## People

### Maintainers

- [@open-policy-agent](https://github.com/open-policy-agent) - Official OPA account 🌎 ([Twitter](https://twitter.com/OpenPolicyAgent))
- [@tsandall](https://github.com/tsandall) - Torin Sandall 🇨🇦 - OPA co-creator ([Twitter](https://twitter.com/sometorin))
- [@timothyhinrichs](https://github.com/timothyhinrichs) - Tim Hinrichs 🇺🇸 - OPA co-creator ([Twitter](https://twitter.com/tlhinrichs))
- [@ashutosh-narkar](https://github.com/ashutosh-narkar) - Ash Narkar 🇺🇸 - OPA maintainer ([Twitter](https://twitter.com/ashtalk))
- [@johanfylling](https://github.com/johanfylling/) - Johan Fylling 🇸🇪 - OPA maintainer ([Mastodon](https://hachyderm.io/@johanfylling), [Twitter](https://twitter.com/johanfylling))
- [@philipaconrad](https://github.com/philipaconrad) - Philip Conrad 🇺🇸 - OPA maintainer ([Twitter](https://twitter.com/philip_conrad))
- [@anderseknert](https://github.com/anderseknert) - Anders Eknert 🇸🇪 - OPA developer advocate ([Mastodon](https://hachyderm.io/@anderseknert), [Twitter](https://twitter.com/anderseknert))
- [@charlieegan3](https://github.com/charlieegan3) - Charlie Egan 🇬🇧 - OPA developer advocate ([Mastodon](https://hachyderm.io/@charlieegan3), [Twitter](https://twitter.com/charlieegan3))
- [@ritazh](https://github.com/ritazh) - Rita Zhang 🇺🇸 - Gatekeeper maintainer ([Mastodon](https://hachyderm.io/@ritazh), [Twitter](https://twitter.com/ritazzhang))
- [@sozercan](https://github.com/sozercan) - Sertaç Özercan 🇺🇸 - Gatekeeper maintainer ([Mastodon](https://hachyderm.io/@sozercan@mastodon.social), [Twitter](https://twitter.com/sozercan))
- [@jpreese](https://github.com/jpreese) - John Reese 🇺🇸 - Conftest maintainer ([Mastodon](https://hachyderm.io/@jpreese), [Twitter](https://twitter.com/johnpreese))

### Community Stars

- [@Parsifal-M](https://github.com/Parsifal-M) - Peter Macdonald 🇬🇧 - OPA contributor and active community member ([Mastodon](https://hachyderm.io/@parcifal), [Twitter](https://twitter.com/_PeterM_))
- [@m-mizutani](https://github.com/m-mizutani) - Masayoshi Mizutani 🇯🇵 - Security engineer. Prolific OPA & Rego advocate ([Twitter](https://twitter.com/m_mizutani))
- [@RoyOsaki](https://github.com/RoyOsaki) - Roy Hiroyuki OSAKI 🇺🇸 - Research engineer. OPA community contributor ([Twitter](https://twitter.com/Hiroyuki_OSAKI))
- [@developer-guy](https://github.com/developer-guy) - Batuhan Apaydin 🇹🇷 - OPA and many CNCF projects ([Mastodon](https://hachyderm.io/@developerguy), [Twitter](https://twitter.com/developerguyba))
- [@nmeisenzahl](https://github.com/nmeisenzahl) - Nico Meisenzahl 🇩🇪 - All about OPA and cloud native topics ([Mastodon](https://fosstodon.org/@nmeisenzahl), [Twitter](https://twitter.com/nmeisenzahl))
- [@jaspervdj](https://github.com/jaspervdj) - Jasper Van der Jeugt 🇨🇭 - OPA contributor ([Mastodon](https://functional.cafe/@jaspervdj), [Twitter](https://github.com/jaspervdj-luminal))
- [@willbeason](https://github.com/willbeason) - Will Beason 🇺🇸 - Ex Gatekeeper maintainer ([Mastodon](https://functional.cafe/@willbeason@dair-community.social), [Twitter](https://twitter.com/willbeason))
- [@peteroneilljr](https://github.com/peteroneilljr) - Peter O'Neill 🌎 - Ex OPA community advocate ([Mastodon](https://hachyderm.io/@Peteroneilljr), [Twitter](https://twitter.com/peteroneilljr))
- [@antonioberben](https://github.com/antonioberben) - Antonio Berben 🇪🇸 - OPA Contributor & Blogger ([Twitter](https://twitter.com/antonioberben))

### Meetup Groups

- [Amsterdam OPA Users](https://www.meetup.com/opa-amsterdam/) 🇳🇱
- [London OPA Meetup](https://www.meetup.com/london-opa-meetup/) 🇬🇧
- [Stockholm OPA Users](https://www.meetup.com/stockholm-opa-meetup/) 🇸🇪

## Commercial Tools

- [Styra DAS](https://www.styra.com/styra-das) - Styra Declarative Authorization Service, from the creators of OPA
- [Enterprise OPA](https://www.styra.com/enterprise-opa) - Enterprise-grade authorization engine for data-heavy workloads
- [Scalr](https://scalr.com/) - Collaboration and Automation for Terraform, backed by OPA
- [Fairwinds Insights](https://fairwinds.com/insights) - Run OPA policies consistently across CI/CD, Admission Control, and an multi-cluster scanner
- [Snyk IaC](https://snyk.io/product/infrastructure-as-code-security/) - Test Infrastructure as Code source code repositories for security misconfigurations and best practices. The OPA golang libraries are used to evaluate Rego policies to detect misconfigurations in the repositories.
- [Spacelift](https://spacelift.io/): Flexible management platform for Infrastructure as Code, backed by OPA
- [env0](https://www.env0.com): Infrastructure as Code automation platform, with OPA extensibility.

## Contributing

Built a great OPA integration or wrote an interesting blog or article on the topic? Submit a PR!
Please just make sure to include something that describes how the project uses OPA, or how OPA is otherwise related.

## Community

For questions, discussions and announcements related to Styra products, services and open source projects, please join
the Styra community on [Slack](https://communityinviter.com/apps/styracommunity/signup)!
