<!--
  GitHub Profile README
  Username: phuonghx
-->

<h1 align="center">Hi 👋, I'm Phuong</h1>

<h3 align="center">
  Solution Architect • Software Engineer • Data Platforms • GIS • Remote Sensing • AI
</h3>

<p align="center">
  <a href="https://github.com/phuonghx">
    <img src="https://img.shields.io/badge/GitHub-phuonghx-181717?style=flat-square&logoColor=white&logo=github" />
  </a>
  <a href="mailto:phuonghx.me@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-phuonghx.me-181717?style=flat-square&logoColor=white&logo=gmail" />
  </a>
  <a href="mailto:phuonghx.me@gmail.com">
    <img src="https://img.shields.io/badge/LinkedIn-phuonghx-181717?style=flat-square&logoColor=white&logo=linkedIn" />
  </a>
</p>


## About Me

I'm a **Solution Architect and Software Engineer** focused on designing and building data-intensive, distributed systems.

My work spans the full solution lifecycle - from **requirements and architecture to implementation, deployment and operations**.

I work across:

* Solution & System Architecture
* Application & API Platforms
* Data Platforms & Analytics
* GIS, WebGIS & Spatial Systems
* Remote Sensing & Earth Observation
* AI & Intelligent Applications
* Digital Twin & 3D Visualization
* Cloud Infrastructure & DevOps
* Security, Governance & Integration

I enjoy working on problems where **software, data, spatial information and intelligent systems** need to work together as one coherent platform.

---

## GitHub Profile

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=phuonghx&hide_border=true" />
</p>

---

# Solution Architecture

I approach architecture from the **problem and system boundaries first**, then work down toward implementation and infrastructure.

```text
                         BUSINESS & USER NEEDS
                                  │
                                  ▼
                       ┌─────────────────────┐
                       │  SOLUTION ANALYSIS  │
                       │                     │
                       │ Requirements        │
                       │ Constraints         │
                       │ NFRs                │
                       │ System Boundaries   │
                       └──────────┬──────────┘
                                  │
                                  ▼
                    ┌───────────────────────────┐
                    │   SOLUTION ARCHITECTURE   │
                    │                           │
                    │ Components • Interfaces   │
                    │ Data • Integration        │
                    │ Security • NFR            │
                    └────────────┬──────────────┘
                                 │
          ┌──────────────────────┼──────────────────────┐
          │                      │                      │
          ▼                      ▼                      ▼
 ┌────────────────┐     ┌────────────────┐     ┌────────────────┐
 │ Application    │     │ Data Platform  │     │ Geospatial     │
 │ & API          │     │ & Analytics    │     │ Systems        │
 │                │     │                │     │                │
 │ Services       │     │ Data Ingestion │     │ GIS / WebGIS   │
 │ APIs           │     │ Processing     │     │ Spatial Data   │
 │ Workflows      │     │ Analytics      │     │ EO / Raster    │
 └───────┬────────┘     └────────┬───────┘     └────────┬───────┘
         │                       │                      │
         └───────────────────────┼──────────────────────┘
                                 │
                    ┌────────────┴────────────┐
                    │                        │
                    ▼                        ▼
             ┌──────────────┐        ┌────────────────┐
             │ AI &         │        │ 3D / Digital   │
             │ Intelligence │        │ Twin / XR      │
             │              │        │                │
             │ RAG          │        │ 3D GIS         │
             │ Agents       │        │ Visualization  │
             │ Retrieval    │        │ AR / VR        │
             └──────┬───────┘        └───────┬────────┘
                    │                        │
                    └────────────┬───────────┘
                                 │
                                 ▼
                     ┌───────────────────────┐
                     │ Cross-Cutting Concerns│
                     │                       │
                     │ Security & IAM        │
                     │ Governance            │
                     │ Observability         │
                     │ Reliability           │
                     │ Data Quality          │
                     └───────────┬───────────┘
                                 │
                                 ▼
                     ┌───────────────────────┐
                     │ Cloud & Platform      │
                     │                       │
                     │ Infrastructure        │
                     │ Deployment            │
                     │ Automation            │
                     │ Networking            │
                     └───────────┬───────────┘
                                 │
                                 ▼
                     ┌─────────────────────────┐
                     │ Production & Operations │
                     │                         │
                     │ Monitor • Scale         │
                     │ Backup • Recover        │
                     │ Maintain                │
                     └─────────────────────────┘
```

### Architecture Focus

**Solution & System Architecture**
Requirements analysis, system boundaries, architecture patterns, component design, non-functional requirements and technology decisions.

**Application & API Architecture**
Service boundaries, API contracts, asynchronous workflows, distributed services and backend architecture.

**Data Architecture**
Data ingestion, storage, processing, analytical workloads, data lifecycle and governance.

**Geospatial Architecture**
Spatial data models, GIS services, WebGIS platforms, remote sensing and spatial processing pipelines.

**AI Application Architecture**
Retrieval, knowledge systems, LLM applications, agent workflows and intelligent services.

**Cloud & Platform Architecture**
Infrastructure, deployment models, automation, scalability, observability and operational design.

---

# Featured Work

## Data Platforms & Analytics

### Data Lakehouse Platform

Designed an architecture for integrating data from multiple sources into a unified analytical platform.

**Architecture**

```text
Data Sources
     │
     ▼
Ingestion & Validation
     │
     ▼
Raw Data
     │
     ▼
Standardized Data
     │
     ▼
Curated Data
     │
     ├──────────────► Analytics
     ├──────────────► Reporting
     └──────────────► Applications
```

Key architectural considerations:

* Separated data storage from processing workloads.
* Established clear data layers and lifecycle boundaries.
* Designed ingestion for heterogeneous sources and varying data quality.
* Added validation and failure-handling mechanisms.
* Introduced metadata and data discovery processes.
* Designed access policies around organizational and data ownership boundaries.
* Structured the platform to support both analytical and downstream application workloads.

---

### Real-Time Data Platform

Designed a streaming architecture for systems that require continuous data ingestion and near-real-time processing.

```text
                Event Sources
                     │
                     ▼
              Event Ingestion
                     │
                     ▼
              Stream Processing
                ┌────┴────┐
                │         │
                ▼         ▼
          Real-Time    Historical
           Path          Path
                │         │
                ▼         ▼
           Operational   Data
            Analytics   Platform
                │         │
                └────┬────┘
                     ▼
             Analytics & Apps
```

Key architectural considerations:

* Decoupled producers and consumers through event-based communication.
* Separated real-time processing from historical analytical workloads.
* Designed for continuous processing and horizontal scaling.
* Supported window-based aggregation and event correlation.
* Included monitoring and rule-based alerting.
* Considered failure recovery, replay and data consistency.

---

## Data Integration & Interoperability

### Enterprise Data Integration

Designed integration architectures connecting heterogeneous systems and organizational data sources.

```text
 System A ────┐
              │
 System B ────┼──► Integration Layer ───► Consumers
              │
 System C ────┘
```

Key architectural considerations:

* Clearly defined system ownership and boundaries.
* Established explicit integration contracts.
* Designed versioned APIs and backward-compatible interfaces.
* Separated authentication, authorization and business logic.
* Added validation and traceability to data exchange.
* Designed integrations so individual systems can evolve independently.

---

### Federated Data Exchange

Designed a distributed data exchange model where participating organizations retain control of their own systems and data.

```text
                 ┌───────────────┐
                 │ Central       │
                 │ Coordination  │
                 └───────┬───────┘
                         │
              ┌──────────┼──────────┐
              │          │          │
              ▼          ▼          ▼
          Gateway A   Gateway B   Gateway C
              │          │          │
              ▼          ▼          ▼
           Source A   Source B   Source C
```

Key architectural considerations:

* Distributed ownership instead of centralized data ownership.
* Gateway-based controlled exchange.
* Policy-driven access to shared resources.
* Centralized identity with distributed enforcement.
* Data lifecycle and archival policies.
* Clear separation between providers, exchange services and consumers.

---

# GIS & Earth Observation

## WebGIS Platform

Designed layered WebGIS architectures connecting users, application services, geospatial services and spatial data.

```text
                         Users
                           │
              ┌────────────┴────────────┐
              │                         │
              ▼                         ▼
           Web App                  Mobile App
              │                         │
              └────────────┬────────────┘
                           ▼
                    WebGIS Application
                           │
               ┌───────────┴───────────┐
               │                       │
               ▼                       ▼
          GIS Services            Application API
               │                       │
               └───────────┬───────────┘
                           ▼
                    Spatial Data Layer
                           │
              ┌────────────┼────────────┐
              ▼            ▼            ▼
           Vector        Raster       External
            Data         Data          Sources
```

Key architectural considerations:

* Separation between presentation, application and GIS service layers.
* Spatial database design and data access patterns.
* Standardized geospatial service interfaces.
* Raster and vector data management.
* Map visualization and spatial query workflows.
* Integration with external spatial and non-spatial data sources.

---

## Earth Observation Data Pipeline

Designed processing workflows for satellite and environmental data from acquisition through analysis.

```text
Satellite / EO Data
        │
        ▼
Data Ingestion
        │
        ▼
Pre-processing
        │
        ▼
Quality Control
        │
        ▼
Analysis-ready Data
        │
        ▼
Spatial Processing
        │
        ▼
Indicators / Products
        │
        ▼
WebGIS / Analytics / Applications
```

Areas of work include:

* Optical and SAR imagery.
* Raster processing pipelines.
* Spatial data transformation.
* Environmental indicators.
* Land-cover analysis.
* Monitoring and change detection.
* Delivery of analysis-ready geospatial products.

---

# Digital Twin & 3D Systems

## Digital Twin Architecture

Designed systems that combine spatial models, 3D assets, sensor information and operational data.

```text
                 Physical Environment
                         │
                  Sensors / IoT
                         │
                         ▼
                  Data Integration
                         │
          ┌──────────────┼──────────────┐
          ▼              ▼              ▼
       Spatial         Temporal       Operational
        Data             Data            Data
          │              │              │
          └──────────────┼──────────────┘
                         ▼
                  Digital Twin Model
                         │
              ┌──────────┼──────────┐
              ▼          ▼          ▼
             3D       Analytics   Simulation
              │          │          │
              └──────────┼──────────┘
                         ▼
                 Visualization / XR
```

Key architectural areas:

* Spatial and 3D data integration.
* Real-time state synchronization.
* Temporal and historical data.
* 3D visualization.
* Asset inspection.
* Spatial analytics.
* AR / VR interaction.

---

# AI & Intelligent Applications

## AI Knowledge & Retrieval Platform

Designed AI applications that combine structured knowledge, unstructured content and retrieval systems.

```text
                    User
                     │
                     ▼
              AI Application
                     │
          ┌──────────┼──────────┐
          ▼          ▼          ▼
       Retrieval    LLM       Tools
          │          │          │
      ┌───┴───┐      │          │
      ▼       ▼      │          │
   Semantic  Keyword │          │
    Search    Search │          │
      │       │      │          │
      └───┬───┘      │          │
          └──────────┼──────────┘
                     ▼
              Context Assembly
                     │
                     ▼
              Response / Action
```

Key architectural considerations:

* Separation between retrieval, reasoning and application logic.
* Hybrid retrieval across different knowledge sources.
* Context construction and relevance filtering.
* Tool and function integration.
* Stateful and multi-step workflows.
* Evaluation of retrieval and generated responses.
* Access control over knowledge and application capabilities.

---

# Backend & Distributed Systems

## Backend & API Platforms

Designing backend systems around clear domain boundaries and well-defined interfaces.

Key architectural areas:

* Domain-oriented service design.
* REST and asynchronous APIs.
* Event-driven communication.
* Background processing.
* Caching and performance optimization.
* Database access patterns.
* Authentication and authorization.
* Logging and observability.
* Resilience and failure handling.
* CI/CD and production deployment.

---

# Architecture Principles

My approach to architecture is guided by a few practical principles:

```text
                     BUSINESS VALUE
                           │
                           ▼
                    SYSTEM CLARITY
                           │
          ┌────────────────┼────────────────┐
          ▼                ▼                ▼
      Simplicity       Reliability       Security
          │                │                │
          └────────────────┼────────────────┘
                           ▼
                    Observability
                           │
                           ▼
                       Automation
                           │
                           ▼
                     Operability
```

### Principles I value

* Start with the problem, not the technology.
* Define system boundaries before selecting implementation patterns.
* Keep architecture as simple as the problem allows.
* Separate responsibilities between components.
* Treat data ownership and lifecycle as architectural concerns.
* Design security and access control from the beginning.
* Prefer explicit interfaces and contracts.
* Design for failure, recovery and observability.
* Automate repeatable processes.
* Choose technologies based on architectural requirements rather than trends.

---

# Technical Skills

## Architecture

* Solution Architecture
* System Architecture
* Application Architecture
* Data Architecture
* Integration Architecture
* API Architecture
* Distributed Systems
* Event-Driven Architecture
* Security Architecture
* Cloud Architecture

## Data Platforms

* Data Lakehouse
* Data Engineering
* Batch & Stream Processing
* Real-Time Analytics
* Big Data
* OLAP
* Data Governance
* Metadata Management
* Data Quality
* Data Lifecycle Management

## Geospatial

* GIS
* WebGIS
* Spatial Databases
* Spatial Data Infrastructure
* Remote Sensing
* Earth Observation
* Raster / Vector Processing
* Spatial Analytics
* Geospatial APIs
* 3D GIS

## AI

* LLM Applications
* Retrieval-Augmented Generation
* AI Agents
* Vector Search
* Embeddings
* Hybrid Retrieval
* Tool Calling
* Knowledge Systems
* AI Evaluation

## Visualization

* 3D Visualization
* Digital Twin
* WebGL
* Three.js
* AR / VR
* Spatial Visualization

## Backend

* Python
* Node.js
* REST APIs
* Service-Oriented Systems
* Event-Driven Systems
* Async Processing
* Background Workers
* Caching
* Observability

## Databases

* PostgreSQL
* PostGIS
* MySQL / MariaDB
* Redis
* OLAP Databases
* Vector Databases

## Cloud & DevOps

* Linux
* Docker
* Kubernetes
* CI/CD
* Infrastructure as Code
* Networking
* Reverse Proxy
* Monitoring & Observability
* Backup & Disaster Recovery

---

# Technology Landscape

The technologies I work with or explore include:

<p align="center">

<img src="https://img.shields.io/badge/Python-000000?style=flat-square&logoColor=white&logo=python"/>
<img src="https://img.shields.io/badge/Node.js-000000?style=flat-square&logoColor=white&logo=node.js"/>
<img src="https://img.shields.io/badge/PostgreSQL-000000?style=flat-square&logoColor=white&logo=postgresql"/>
<img src="https://img.shields.io/badge/PostGIS-000000?style=flat-square&logoColor=white&logo=postgis"/>
<img src="https://img.shields.io/badge/Redis-000000?style=flat-square&logoColor=white&logo=redis"/>

<br/>

<img src="https://img.shields.io/badge/Apache%20Kafka-000000?style=flat-square&logoColor=white&logo=apachekafka"/>
<img src="https://img.shields.io/badge/Apache%20Spark-000000?style=flat-square&logoColor=white&logo=apachespark"/>
<img src="https://img.shields.io/badge/Apache%20Flink-000000?style=flat-square&logoColor=white"/>
<img src="https://img.shields.io/badge/Apache%20Iceberg-000000?style=flat-square&logoColor=white"/>
<img src="https://img.shields.io/badge/ClickHouse-000000?style=flat-square&logoColor=white"/>

<br/>

<img src="https://img.shields.io/badge/GeoServer-000000?style=flat-square&logoColor=white"/>
<img src="https://img.shields.io/badge/GDAL-000000?style=flat-square&logoColor=white"/>
<img src="https://img.shields.io/badge/Three.js-000000?style=flat-square&logoColor=white&logo=threedotjs"/>
<img src="https://img.shields.io/badge/WebGL-000000?style=flat-square&logoColor=white"/>

<br/>

<img src="https://img.shields.io/badge/Docker-000000?style=flat-square&logoColor=white&logo=docker"/>
<img src="https://img.shields.io/badge/Kubernetes-000000?style=flat-square&logoColor=white&logo=kubernetes"/>
<img src="https://img.shields.io/badge/GitHub%20Actions-000000?style=flat-square&logoColor=white&logo=githubactions"/>
<img src="https://img.shields.io/badge/Linux-000000?style=flat-square&logoColor=white&logo=linux"/>

</p>

---

# Current Interests

```text
Solution Architecture
 ├── System Design
 ├── Application Architecture
 ├── Data Architecture
 ├── Integration Architecture
 └── Cloud Architecture

Data Platforms
 ├── Lakehouse
 ├── Streaming
 ├── Big Data Analytics
 ├── Real-Time Systems
 └── Data Governance

Geospatial
 ├── GIS / WebGIS
 ├── Spatial Databases
 ├── Remote Sensing
 ├── Earth Observation
 └── Spatial Analytics

AI
 ├── LLM Applications
 ├── RAG
 ├── AI Agents
 ├── Knowledge Systems
 └── Intelligent Workflows

Digital Twin
 ├── 3D GIS
 ├── Digital Twin
 ├── WebGL
 ├── AR
 └── VR

Cloud & Platform
 ├── Cloud Infrastructure
 ├── Containers
 ├── CI/CD
 ├── Infrastructure as Code
 └── Observability
```

---

# Engineering Mindset

I enjoy solving problems where different engineering disciplines intersect.

```text
                         BUSINESS
                            │
                            ▼
                    SOLUTION ARCHITECTURE
                            │
          ┌─────────────────┼─────────────────┐
          ▼                 ▼                 ▼
       SOFTWARE            DATA              GIS
          │                 │                 │
          └─────────────────┼─────────────────┘
                            │
                            ▼
                           AI
                            │
                            ▼
                     CLOUD / PLATFORM
                            │
                            ▼
                       PRODUCTION
```

The goal is not simply to build individual components.

It is to design **coherent, maintainable and operable systems** where software, data, infrastructure, geospatial information and intelligent capabilities work together.

---

# Connect With Me

<p align="center">
  <a href="https://github.com/phuonghx">
    <img src="https://img.shields.io/badge/GitHub-phuonghx-181717?style=flat-square&logoColor=white&logo=github" />
  </a>
  <a href="mailto:phuonghx.me@gmail.com">
    <img src="https://img.shields.io/badge/Email-phuonghx.me-181717?style=flat-square&logoColor=white&logo=gmail" />
  </a>
</p>

<p align="center">
  <i>Architecture • Engineering • Data • GIS • AI</i>
</p>
