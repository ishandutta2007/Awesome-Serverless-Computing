# Awesome-Serverless-Computing

# Top Serverless Computing Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Function-as-a-Service, Event-Driven Runtimes & Self-Hosted Serverless Platforms*
**Last updated: October 2026**

This repository tracks notable **commercial serverless platforms** and **open-source projects** that provide Function-as-a-Service (FaaS), event-driven execution, and scale-to-zero runtimes. These tools let developers deploy code without managing servers, paying only for execution time.

**Examples** include Azure Functions, AWS Lambda, Google Cloud Functions, Cloudflare Workers, Vercel Serverless Functions, Netlify Functions, Fastly Compute, Oracle Cloud Functions, IBM Cloud Code Engine, and Baseten (the category leaders).

**Open-source emphasis**: Serverless computing is a rapidly maturing open-source domain. **Fission**, **OpenFaaS**, **Refunc**, and **OpenWhisk** provide production-grade Kubernetes-native FaaS, while **Beta9** delivers ultrafast serverless GPU inference. **self-hosted-serverless** offers a lightweight Go-based alternative for edge deployments. This section is heavily expanded.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[AWS Lambda](https://aws.amazon.com/lambda/)**
  The pioneer of serverless computing with the broadest ecosystem. **Event-driven execution with sub-second billing**, 15-minute maximum runtime, and native integration with 200+ AWS services. Supports Python, Node.js, Java, Go, .NET, Ruby, and custom runtimes.

- **[Azure Functions](https://azure.microsoft.com/en-us/products/functions/)**
  Microsoft's serverless compute with Durable Functions for stateful workflows, Azure Logic Apps integration, and strong enterprise compliance credentials.

- **[Google Cloud Functions](https://cloud.google.com/functions)**
  Google's event-driven serverless platform with CloudEvents support, Cloud Run integration, and Firebase triggers.

- **[Cloudflare Workers](https://workers.cloudflare.com/)**
  **Edge-native serverless with V8 isolates** — sub-millisecond cold starts, no cold starts for most requests. **The fastest serverless runtime available** with global distribution across 300+ cities.

- **[Vercel Serverless Functions](https://vercel.com/docs/functions)**
  Frontend-optimized serverless with automatic scaling, edge middleware, and seamless Next.js integration.

- **[Netlify Functions](https://www.netlify.com/products/functions/)**
  JAMstack-focused serverless with background functions and scheduled tasks.

- **[Fastly Compute](https://www.fastly.com/products/edge-compute)**
  Edge computing platform with Wasm-based execution at Fastly's global edge network.

- **[Oracle Cloud Functions](https://www.oracle.com/cloud-native/functions/)**
  Open-source FaaS built on Project Fn, deployable on OCI or on-premises.

- **[IBM Cloud Code Engine](https://www.ibm.com/cloud/code-engine)**
  Unified serverless platform for containers, batch jobs, and functions.

- **[Baseten](https://www.baseten.co/)**
  **Serverless GPU inference platform** for AI model deployment with Truss serving framework, autoscaling, and support for custom models .

## Open-Source GitHub Projects

- **[Fission](https://github.com/fission/fission)**
  **The leading Kubernetes-native serverless framework**, Apache-2.0 licensed . **100msec cold starts** via pool of warm containers with dynamic loaders . Supports **NodeJS, Python, Ruby, Go, PHP, Bash, and any Linux executable** . **Event-driven triggers** from HTTP, message queues, and scheduled tasks . **The de facto open-source Lambda replacement for Kubernetes** — abstractions hide Docker and Kubernetes complexity while remaining extensible .

- **[OpenFaaS](https://github.com/openfaas/faas)**
  **The most widely adopted open-source FaaS platform**, MIT licensed . **Deploy functions as Docker containers** — any language, any binary . **faasd** provides lightweight single-node deployment without Kubernetes . **The standard for self-hosted function platforms** — used by enterprises for event-driven automation and API backends .

- **[Refunc](https://github.com/refunc/refunc)**
  **Kubernetes-native serverless platform with AWS Lambda compatible API** , Apache-2.0 licensed . **Scale from zero** — autoscale from zero-to-many and vice versa . **Portable** — run everywhere that has Kubernetes . **AWS CLI compatible** — manage functions locally using standard AWS tooling . **Best for teams wanting Lambda compatibility with Kubernetes portability** .

- **[Apache OpenWhisk](https://github.com/apache/openwhisk)**
  **Apache's serverless platform for event-driven computing** , Apache-2.0 licensed . **The foundation for OpenServerless** — an Apache incubator project using OpenWhisk as FaaS engine with Apache APISIX and Kvrocks . **Production-proven at IBM Cloud Functions scale** . **Best for organizations wanting Apache-governed serverless infrastructure** .

- **[Beta9 (Beam)](https://github.com/beam-cloud/beta9)**
  **Ultrafast serverless GPU runtime for AI workloads** , open-source with self-hosting option . **Cold starts under one second** via custom container runtime and embedded caching . **GPU support** — run on A10G, H100, RTX 4090, or bring your own GPUs . **Pythonic interface** — deploy inference endpoints, background tasks, and sandboxes with decorators . **Used by Coca-Cola, Magellan AI, and Shippabo** . **The leading open-source Modal alternative** for serverless AI .

- **[Self-Hosted Serverless](https://github.com/mstgnz/self-hosted-serverless)**
  **Lightweight, self-hostable alternative to AWS Lambda and Google Cloud Functions** , MIT licensed . **Built in Go** for fast cold starts and minimal resource footprint . **HTTP and gRPC support** with WebAssembly runtime for multi-language functions . **API key auth, rate limiting, and per-execution timeout** built in . **Best for edge deployments and resource-constrained environments** .

- **[fn0](https://github.com/namseent/fn0)**
  **Fully open-source FaaS platform using V8 and Wasmtime** , positioned as a self-hostable Cloudflare Workers alternative . **Run WebAssembly components (WASI 0.3)** and **JavaScript/TypeScript in V8-based runtime** . **Built-in transactional document storage** and **S3-compatible object storage** . **OpenTelemetry observability** with standard OTLP export . **Best for teams wanting Workers-like execution on their own infrastructure** .

- **[KubeFunction](https://github.com/KubeFunction/KubeFunction)**
  **Kubernetes Operator-based serverless/FaaS platform** , Apache-2.0 licensed . **Declarative function management via CRDs** — define functions and events as Kubernetes resources . **Event-driven automatic deployment and execution** . **Best for Kubernetes-native teams wanting declarative function management** .

- **[OpenServerless (Apache Incubator)](https://cwiki.apache.org/confluence/pages/viewpage.action?pageId=309496241)**
  **Apache incubator project for open-source serverless** , Apache-2.0 licensed . **Built on Apache OpenWhisk, APISIX, and Kvrocks** . **Kubernetes-deployable with no vendor lock-in** . **15+ contributors from Nuvolaris and community** . **Best for organizations wanting Apache-governed serverless** .

- **[Tau](https://github.com/taubyte/tau)**
  **Open-source distributed Platform as a Service** — self-hosted Vercel/Netlify/Cloudflare alternative . **Git-native CDN PaaS** — no API calls to create resources; Git is the only way to alter infrastructure . **Single binary with minimal configuration** — auto-discovery for node coordination . **4,421+ GitHub stars, BSD-3-Clause licensed** . **Best for teams wanting a complete self-hosted PaaS with GitOps workflow** .

### Additional Strong Open-Source Options

- **celld** — Ryan Dahl's self-hosted distributed Durable Objects/Workers implementation, Apache-2.0 licensed. **V8 + S3 + SQLite architecture** for stateful serverless .
- **SlimFaas** — "The slimmest and simplest Function As A Service" .
- **faasm** — High-performance stateful serverless runtime based on WebAssembly .
- **OpenFunction** — CNCF Sandbox project for cloud-native FaaS .
- **BentoML** — Unified model serving framework for ML deployment, Apache-2.0 licensed .
- **Nexa SDK** — On-device AI inference across CPU, GPU, and NPU hardware, Apache-2.0 licensed .

**Frameworks for building custom serverless platforms**: Combine **Fission** for production-grade Kubernetes-native FaaS with 100msec cold starts . Use **OpenFaaS** for the broadest ecosystem and Docker-based function deployment . Deploy **Refunc** for AWS Lambda compatibility with Kubernetes portability . Choose **Beta9** for serverless GPU inference with sub-second cold starts . Use **Self-Hosted Serverless** for lightweight edge deployments with WebAssembly support . Note that true enterprise serverless with global infrastructure, managed SLAs, and integrated observability remains primarily commercial territory; open-source stacks provide strong function runtimes, event triggers, and scale-to-zero foundations that require integration for complete serverless architectures.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Serverless platforms execute arbitrary code and handle sensitive data. Self-hosted solutions require proper security hardening, function isolation, and compliance with data privacy regulations.
- **Cold start performance varies significantly** — Fission achieves ~100msec , Beta9 sub-second , and Cloudflare Workers near-instant via V8 isolates. Self-hosted solutions depend on your infrastructure and warm pool configuration.
- **GPU serverless adds complexity** — Beta9 requires GPU infrastructure for AI workloads . Evaluate GPU availability and cost against your inference needs.
- The open-source ecosystem provides strong function runtimes, event triggers, and scale-to-zero foundations, but **global infrastructure, managed SLAs, and integrated observability** remain primarily commercial offerings.

---

**Made for platform engineers, backend developers, and architects building serverless applications.**
Let's make serverless computing more open, transparent, and accessible.
