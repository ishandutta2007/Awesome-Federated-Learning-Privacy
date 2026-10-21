# Awesome-Federated-Learning-Privacy

## Top Federated Learning & Privacy Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Privacy-Preserving Collaborative Training, Healthcare Deployments & Self-Hosted FL Frameworks*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Federated Learning & Privacy**. These tools enable multiple parties to collaboratively train machine learning models without sharing raw data—critical for healthcare, finance, and any domain where data sovereignty and regulatory compliance (GDPR, HIPAA) are non-negotiable.



**Examples** include NVIDIA Clara/FLARE, Owkin/Substra, Rhino Health, Flower, IBM Federated Learning, FedML, OpenMined PySyft, EdgeDelta, and Apheris (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, healthcare-grade deployments, and transparent privacy guarantees—ideal for hospitals, research consortia, and enterprises that cannot centralize sensitive data. The open-source landscape is anchored by **NVIDIA FLARE** (enterprise/regulated deployments), **Flower** (framework-agnostic research standard), **Substra** (healthcare production-proven from Owkin), and **PySyft** (encrypted computation), with **FedML** bridging research and production.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[NVIDIA Clara](https://www.nvidia.com/en-us/clara/)**  

  NVIDIA's healthcare AI platform, with NVIDIA FLARE as its federated learning runtime. Clara provides domain-specific tooling for medical imaging and genomics, while FLARE handles the federated orchestration . Best for healthcare organizations seeking an integrated NVIDIA ecosystem.



- **[Owkin](https://www.owkin.com/)**  

  AI biotech company that originated Substra and remains its primary contributor. Offers federated learning services for pharmaceutical research and clinical trials, with Substra as the underlying open-source foundation .



- **[Rhino Health](https://www.rhinohealth.com/)**  

  Federated learning platform specifically designed for healthcare and life sciences. Focuses on enabling multi-institutional collaboration while maintaining HIPAA and GDPR compliance. Commercial offering with healthcare-specific workflows.



- **[Flower (Cloud/Enterprise)](https://flower.ai/)**  

  Commercial tier of the Flower federated learning framework. Offers managed infrastructure and enterprise support for the open-source core. Flower is framework-agnostic and widely used in research .



- **[IBM Federated Learning](https://www.ibm.com/products/federated-learning)**  

  IBM's enterprise federated learning offering, integrated with IBM Cloud Pak for Data and Watson Studio. Supports both horizontal and vertical federated learning. Commercial support and integration with IBM's broader AI governance tooling.



- **[EdgeDelta](https://edgedelta.com/)**  

  Observability platform with edge processing capabilities. While not a pure federated learning platform, it supports distributed data processing at the edge, relevant for privacy-sensitive inference scenarios.



- **[Apheris](https://www.apheris.com/)**  

  Enterprise federated learning platform focused on regulated industries (healthcare, finance, manufacturing). Provides governance, audit trails, and compliance controls for multi-party data collaboration.



## Open-Source GitHub Projects



- **[NVIDIA FLARE](https://github.com/NVIDIA/NVFlare)**  

  NVIDIA Federated Learning Application Runtime Environment. Domain-agnostic Python SDK supporting horizontal and vertical federated learning, with built-in FedAvg, FedProx, FedOpt, and Scaffold algorithms . **Privacy mechanisms**: differential privacy, homomorphic encryption, and private set intersection (PSI) filters . Component-based architecture with Controller/Worker execution model, customizable communication drivers (gRPC by default), and support for both simulation and production deployment . Apache 2.0 licensed. Best for enterprise and regulated deployments, including clinical use cases .



- **[Flower](https://github.com/adap/flower)**  

  Framework-agnostic federated learning framework with a client-server abstraction that works with PyTorch, TensorFlow, JAX, and scikit-learn. Widely adopted in research for its simplicity and flexibility . Ranked among the most mature FL tools alongside OpenFL and IBM-Federated, with the highest growth rate in comparative studies . Apache 2.0 licensed. Best for research and teams that want to avoid framework lock-in.



- **[Substra](https://github.com/Substra/substra)**  

  The most proven open-source federated learning software designed for healthcare research . Originally developed by Owkin and now hosted by the Linux Foundation for AI and Data. Provides a flexible Python interface and web application for running FL training at scale. Deployed in production by hospitals and biotech companies (e.g., the MELLODDY project) . Apache 2.0 licensed. Specifically designed for medical data applications alongside Fed-BioMed . Best for healthcare consortia and production clinical research.



- **[PySyft (OpenMined)](https://github.com/OpenMined/PySyft)**  

  A library for computing on data you do not own and cannot see. Emphasizes privacy-preserving and encrypted computation over distributed data, rather than being purely a federated averaging framework . Apache 2.0 licensed. Backed by the OpenMined community (12,000+ Slack members) . Best for scenarios requiring encrypted computation and advanced privacy primitives beyond standard FL.



- **[FedML](https://github.com/FedML-AI/FedML)**  

  Unified and scalable ML library for large-scale distributed training, model serving, and federated learning. Targets cross-device and cross-silo production workflows with a unified research library . 4,170+ GitHub stars, Apache 2.0 licensed . Best for teams that want to bridge research experimentation and production federated learning.



### Additional Strong Open-Source Options



- **OpenFL (Intel)** — Open framework for federated learning, ranked among the most mature FL tools . Best for Intel-based research clusters and teams seeking an alternative to Flower.

- **TensorFlow Federated (TFF)** — Tightly integrated with TensorFlow, supports simulation at scale . Best for TensorFlow-centric research teams.

- **FATE (WeBank)** — Federated AI Technology Enabler, widely used in Chinese enterprise deployments. Best for organizations operating in or integrating with the Chinese fintech ecosystem.

- **Fed-BioMed** — Specifically designed for medical data applications alongside Substra . Best for healthcare research with a focus on medical imaging and clinical data.

- **Frameworks for building custom systems**: Pair **NVIDIA FLARE** for enterprise orchestration with its built-in privacy filters (homomorphic encryption, differential privacy). Use **Flower** for framework-agnostic research prototypes, and **Substra** when healthcare production deployment and regulatory compliance are primary requirements. **PySyft** provides the encrypted computation layer when standard FL aggregation is insufficient.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Federated learning frameworks vary significantly in privacy guarantees (differential privacy, homomorphic encryption, secure aggregation), healthcare compliance readiness, and operational complexity; evaluate against your regulatory requirements.

- Self-hosted solutions require proper PKI setup, network security, and audit logging to ensure that "privacy-preserving" claims hold in practice.



---



**Made for healthcare AI researchers, privacy engineers, data governance teams, and organizations building collaborative intelligence without centralizing sensitive data.**  

Let's make federated learning more open, auditable, and deployable in regulated environments.
