# Kin + Carta
Kin + Carta is a B Corp certified technology, data and experience consultancy that believes in using business as a force for good. Focusing on digitally-native technology K+C exports to clients its positive, ambitious, and curious transformative culture while delivering for our clients the tools, skills, and capabilities for true, long term digital transformation.

Kin + Carta as a consultancy is unique in its approach to client relationships in that we chose to partner, pair, and share engineering experience in real-time with client engineering teams. Those engagements tend to be more successful due to the nature of those relationships: K+C consultants are not interested in building a system and "throwing the technology over the fence" to our clients, hoping for some long-term support contract. Instead, our long-term partnerships tend to form through exploration of other areas in the client portfolio of applications and identifying new opportunities to modernize and level up entirely new teams in our clients' organizations.

Kin + Carta recongizes the value of consultant-client partnerships in a practical way - consulting engineers learn about the requirements of enterprise, while enterprise learns the process, management, and technology a rapidly iterative team focused explicitly on modern digital transformation can provide.

The company focuses on socially responsible business that champions inclusion, diversity, and equality - and is the world's _first_ publicly-traded certified B Corp. During my time, Kin + Carta has grown from ~150 employees when I began, to over 1,100 employees globally, with offices in Chicago, Denver, Buenos Aires (Argentina), and London (UK).

## Tech Stack
### Infrastructure/DevOps/Platform

- Infrastructure as Code (IAC)
  - Hashicorp Stack: Terraform, Packer
  - Google Cloud: Anthos, ConfigConnector, Deployment Manager
  - AWS: Cloud Formation
  - Other tooling I have interest & experience with, but not in production
    - [Crossplane](https://crossplane.io)
    - [Pulumi](https://www.pulumi.com/)
    - [Atlas DDL](https://atlasgo.io/)
- Cloud Providers (IaaS), Platform-as-a-Service (PaaS), & hosted private cloud
  - Google Cloud Platform (GCP)
  - Microsoft Azure
  - Amazon Web Services (AWS)
  - VMWare vSphere
  - Cloud Foundry (Pivotal)
  - Other Managed PaaS Providers (Heroku, DigitalOcean)
  - Other Hosted/Managed Private Cloud (Rackspace, Linode)
- Runtimes
  - Container-native
    - Kubernetes 
      - managed: GKS, AKS, EKS
      - onPrem: Rancher/Suse, Cloud Foundry (with Pivotal PKS Kubernetes extensions)
      - Vanilla K8s via KOPS (Never again!)
    - Docker Swarm
    - AWS ECS
  - Virtualized Machine (VM w/ managed autoscalers in applicable situations)
    - GCP: Compute Engine 
    - AWS: EC2
    - Azure Virutal Machines/Spot Virutal Machines
    - VMWare vSphere Compute
    - Bare-metal Hypervisors: Microsoft HyperV, Citrix XenServer, VMWare ESXi, KVM)
  - Serverless
    - GCP:  AppEngine, Cloud Run, Cloud Functions
    - AWS: Lambda (light experience)
  - Hybrid
    - Hashicorp Nomad
  - Bare Metal
    - Ubuntu Enterprise, RHEL, 
    - Traditional Windows stack
- Networking
  - VPC
    - Google Cloud VPC: including Shared VPC, various Hybrid Connectivity options, Cloud DNS, Cloud CDN, Traffic Director & Service Catalog, Firewalls
    - AWS VPC, AppMesh, API Gateway, Route53
    - VMWare VPC
  - Hypervisor (Layer II & III)
    - Citrix XenServer Network Bonding/XenBridge (never again, hopefully!)
    - Hyper-V Virtual Switching
  - Bare Metal
    - Cisco Routing & Switching (it's been a while!)
  - Service Mesh
    - Envoy w/ Istio Control Plane
    - Hashicorp Consul
    - NGINX Service Mesh (not in prod)
  - Load balancing
    - Cloud Load Balancers (Google, AWS)
    - NGINX
    - HAProxy
    - F5 Load balancing
  - Security
    - Google Cloud Armor, Cloud NAT, VPC IAM & Service Controls, Cloud WAF
    - Snort Network Intrusion Detection System (NIDS)
- Application & Infrastructure Observability
  - Tooling
    - Dynatrace (Logging, service telemetry, APM)
    - Google Cloud Operations (Logging, Monitoring, Error reporting, Network Trace, Profiler, Debugger, Network Telemetry via Istio Control plane in an Envoy service mesh)
    - Datadog
    - Prometheus/Grafana/Jaeger
    - Elastic (ELK/EFK) stack w/ APM tooling
    - Nagios
  - Other Exception Monitoring Tools (mainly in Rails/JS)
    - LogRocket
    - Rollbar
    - Sentry
  - Observability scopes
    - APM: Application Performance Monitoring
    - Runtime Application Security Monitoring
    - Static Security Scanning (Snyk, container & artifact scanning, static code analysis)
    - Service Mesh Network Observability (Jaeger)
- Data Persistence, Delivery, Management
  - Async Data Transmission, Messaging, & Event Sourcing
    - Google Cloud Pub/Sub
    - AWS SNS/SQS/MQ
    - RabbitMQ
    - Apache Kafka
  - ETL: Extract, Translate, Load
    - Google Cloud Dataflow, Dataproc, Data Fusion
  - Structured Data/Databases:
    - Various RDBs: Postgres, MySQL, T-SQL, Google Cloud SQL
    - Distributed Search: Elasticsearch
    - Document Store: GCP Firestore/Datastore, MongoDB
    - Time Series: Prometheus
    - Columnar: Google BigQuery
    - Wide Column: Google BigTable
    - Key-Value: Redis (Managed & Enterprise), AWS DynamoDB, Azure Cosmos, etcd, memcached
    - Graph: Neo4J (light experience)
  - BLOB Storage
    - Google Cloud Storage, Persistent Disk
    - AWS S3
- Security, Identity, Compliance
  - Google Cloud
    - Identity
      - IAM, Cloud Identity, Resource Manager
    - Compliance
      - Risk Manager (Infra compliance)
    - Security
      - Security Command Center, Cloud KMS, Secrets Manager, Cloud DLP
      - Cloud Armor, Cloud WAF, Cloud Firewall (Network security)
  - AWS 
    - Identity
      - IAM
    - Service Scoping
      - Organizations
      - Resource Access Manager
    - Security
      - Network: Firewall Manager
      - Key Manager, Certificate manager, Secrets Manager
  - Hashicorp 
    - Vault: Dynamic, rules-based Identity Provisioning/Deprovisioning & secrets management
    - Sentinel: Infrastructure Policy-as-Code (pre-provisioning security & compliance)
    - WayPoint: (not in prod) Dynamic, rules-based User Identity & provisioning of services, APIs, & applications

### Application Domain
- Application languages & Frameworks
  - Ruby: Sinatra, Trailblazer, and of course Rails (I have some years here)
  - Go (I'm a newbie Gopher but *love* the language and the lack of reliance on frameworks)
  - Python: for scripting (typically I prefer Ruby, and now Go - fast compile, excellent libs, strongly typed, and great cross platform support, plus... Go binaries! Why write a script when you can write a tool?)
  - Rust (again, newbie - contending with Go for my attention & currently losing)
  - Swift: hoping to see Server-side Swift get popular one day!
  - Javascript/Typescript:
    - backend: NodeJS
    - frontend (ask me to do frontend at  your own risk!): React, Angular, Vue, Ember
  - Java: Spring Boot, Spring Cloud (I've supported and built build systems and platforms for large enterprise enviroments, so I know the quirks in Java/Spring at scale. Never loved writing Java though.)
  - Bash
  - Powershell
- Build Systems
  - Java: Maven, Gradle Jib (Container native)
  - Ruby: Bundler and Rake, pretty standard
  - Python: pipenv, venv, condae
  - Javascript/TS: NPM
  - Go: standard tooling, [GoReleaser](https://goreleaser.com/)
- Continuous Integration (CI)
  - Jenkins
  - Container-native:
    - GitHub Actions
    - Google Cloud Build
    - BitBucket Cloud Pipelines
    - GitLab
    - CircleCI
    - Jenkins-X
  - Container Native Build Tools:
    - Skaffold
    - Kaniko
    - CNCF Buildpacks
    - Jib
    - Ko (for GoLang)
- Imperative Workflows + Task Orchestration
  - GitHub Actions
  - BitBucket Cloud Pipelines
  - Argo Workflows & Events
  - Tekton
  - Google Cloud Workflows
  - GitLab
  - Spinnaker
  - Harness
  - Apache Airflow (for ML training)
- Continuous Delivery (CD) - Declarative, GitOps Application Delivery Tooling
  - Google Anthos
  - Argo CD & Rollouts
  - GitLab
  - Flux
- Artifact, Container, Image management
  - Google Artifact Repository (Conatiners, libs, compiled artifacts)
  - Sonatype Nexus
  - JFrog Artifactory
  - Hashicorp HCP Packer Cloud (VM Image management, functionally similar to container image management)
  - Github Packages (for OSS)
  - DockerHub (for OSS)
- Kubernetes Deployment tooling
  - Kustomize
  - Helm
  - Kubernetes Operators (Elasticsearch, Spinnaker, Istio, Grafana, ArgoCD)
  - Raw K8s YAML (preferably not)
- Testing Patterns
  - Unit/Integration testing
  - Automated User-Acceptance
  - Performance Testing & Application Profiling
  - Contract testing/validation
  - Smoke Testing
- Developer Experience
  - Portable Dev Environments
    - GitHub Codespaces
    - VSCode DevSpaces on Docker
    - DevSpaces
    - Okteto
    - GitPod
  - Dev Observability in the deployed environment
    - Skaffold
    - Rancher Desktop (RKE, K3s) local K8s development environment


## Kin & Carta Cloud Architect, Senior Site Reliability Engineer - Cloud Capabilites

Promotion to this position was more a recognition and formal advancement of the processes and skills in my prior role. Importantly, it did provide a wider reach across teams beyond my own primary project (Gordon Food Services), giving me the opportunity to touch numerous other projects within Kin + Carta (whenever they asked and I had cycles!)

Interestingly, this widend perspective across projects made me a bit more "bookish". I invested far more time in the DevOps/SRE literature. I also spent more time learning high-level Application Architecture patterns:

- Microservice Design: Gateway Routing, Endpoint Monitoring, application Bulkheads & Circuit Breaking, retry & rate limiting, application sidecars
- Service Reliability, Data Transmission: sync vs async, publisher/subscriber, event sourcing
- Security: Identity as a Service
- Networking & Traffic Services: HTTP vs gRPC protocols, network telemetry & intrusion detection

The promotion also provided some budgetary allowance (in time, specfically) to focus on areas where Kin + Carta had a gap:

1. "Shift Left" - Developer Experience Improvement
   
   Defining "The Kin + Carta Way" in Cloud Capabilities proved difficult to pin down (this is the nature of consulting due to the rapid evolution of tech and the wide gamut of challenge-scopes), but we did extract some core fundamental skillsets, expectations, and team dynamics that we could test for and inquire about with candidates.
   
   Ultimately, I began a journey that could be replicated across teams and various client projects that enabled a "shift left" mentality - instead of siloing "Platform Engineering" to manage infrastructure, we focused on building tools and frameworks that allow the developer to easily declare the infrastructure they _need_ to run their application.  Abstraction of platform and cloud provider was the goal, and GitOps with declarative and simple (testable and secured) DSLs were the implementation pattern. 
   
   Shifting Left enabled Platform and Security engineers to focus on their specific domain, upskill without dramatic dev cycle impact, _and_ deliver new features in a low-impact way to developer teams. Platform teams got more time to embed with dev teams and deliver that "SRE Experience" (defining and building SLOs & SLIs, automating testing, automating for failure, etc). 
   
   Critically, during the height of the COVID pandemic, it also meant we could whittle away at burnout from toil. Platform engineers could be software engineers again, spending time solving for manual labor problems at a time when reduced headcount and increased individual contribution expectations were at their peak.

2. Talent Acquisition - Improving the DevOps/Platform Engineering Interview Process
   
   Interviewing for Platform, Cloud, and DevOps related engineering roles are uniquely challenging insofar as meaningful and useful challenges provided to applicants typically have far more solutions than your average application challenge. Choice of tooling, platform, delivery method, and provisioned cloud "space" need to be tested and made available for prospects, if the desire is to measure applied knowledge in the space. 
   
   Struggling with truly understanding someone's capability beyond simply asking questions, I asked for (and got) C-suite support to improve the candidate interview & testing process for Platform/DevOps engineers. The outcome was a series of challenges and expectations, broken down for various skill levels and engineering domains, maintained in a Kin + Carta git repository, that could be delivered to an applicant, temporarily provision a space in a given Cloud Provider for that applicant, and deliver solutions to the TA & interviewing teams for review, then deprovision the workspace.

3. Upskilling the Internal Kin + Carta IT capability - London - UK, Buenos Aires - Argentina, Chicago - IL
   
   Toward the end of my tenure at Kin + Carta I was asked to assist in Buenos Aires and London offices "upskilling" our internal IT teams, as leadership desired the same simplification of internal services management as we provided to our clients by shifting to cloud services from local DCs. Offering tooling, documentation, hiring, mentorship, and running remote educational sessions with experience from client work, I assisted the team kicking off this process.
   
   *Update:* I just read that Kin + Carta recently declared (March, 2022) the total transition to cloud of all internal applications and services from their regoinal DCs.

## Kin & Carta Platform & DevOps Engineer - Technical Consultant

In early 2018 I joined Kin + Carta as the firm's first full-time engineer focused on modern DevOps application delivery practices - including Platform Engineering, CI/CD pipepines, Automated Testing (pre- and post- deployment), robust monitoring, security, networking, managing various runtimes (serverless, managed virtualized environments, onPrem virtualization, Cloud Foundry, and most importantly, Kubernetes. 

In essence, Kin + Carta were transforming from a mobile and frontend web-application consultancy, to a full-service “Cloud Modernization” consultancy:
- buiding API-first backend services (initially on Java/Spring)
- application modernization focused on scalability and ease-of-iteration (with a strong preference for microservice architecture)
- an active proponent of Agile development _with_ their own clients' developers through Flexible “Extreme Programming” (Fl-EXp, creatively borrowed from Pivotal's "XP" practice)
- ultimately offering clients solid pathways to onboard cloud services through practical, pragmatic, on-the-ground experience while "upskilling" our clients' own engineers.

My roles in this transformation were:

1. Deliver Successful Client Engagements 
   
   I was assigned to Kin + Carta's first enterprise-scale greenfield Cloud initiatives working mainly on Google Cloud Platform. I touched other projects using Pivotal Cloud Foundry (PCF) and Microsoft Azure. 
   
   Generally, I helped build a portfolio of Kubernetes deployment patterns, Spinnaker example orchestrations, standardized application security with templates and sample Dockerfile code (with explanations why certain things were done). I also designed and built Buildpacks, distributed modularlized Cloud infrastructure code (mostly Terraform, some Ainsible Playbooks), worked with Data Teams to provision and operationalize various databases (Elastic, MongoDB, Couchbase, and a slew of RDBs).
   
   Most importantly I focused on teaching our engineers how to teach themselves (and thereby, their clients). It is especially challenging for application engineers to accept the systems-level paradigm - there's clearly a lot of "magic", and is absolutely scary to simply _accept_ in the early phases of learning complex systems like Kubernetes or the relationship between Cloud provisioning APIs and the tools which call them.
   
   DevOps principles, luckily, helped mitigate some of that fear:
     - accepting (and expecting) failure
     - blameless developer culture
     - trusting the process and your team
     - focus on your customer (both the end-user and your developers are your customer)
     - constant iteration and improvement to cope with new problems
     - maintaing open channels between various operations and development teams
     - reject siloing and build a means to cross-educate for those interested
     - build "happy paths" between teams to discuss new ideas or needs while avoiding or removing friction for developer workcycles (keep it calm, let everyone do their job for the day)
     - treat engineer burnout as a real metric to be monitored just as applications are monitored
     - strategically automate everything that causes undue manual toil (but leave some for the new folks to learn from!)

1. Build & Enable Cloud Provider Partnerships:
   
   Help build and enrich partnerships with Cloud services vendors - specifically Google, Microsoft, Hashicorp, and vmWare/Pivotal. Such partnerships drove business to Kin + Carta, and as those partnerships found success, K+C's status as a "Trusted Service Provider" flourished. 

   As part of the Cloud Partnership team we became [Certified Google Cloud Partners in an number of fields](https://www.kinandcarta.com/en-us/partners/google/), and later reached [Gold Partner status with Microsoft](https://www.kinandcarta.com/en-us/partners/microsoft/)

1. Build and formalize the Platform/DevOps Engineering team:
   
   While K+C has _numerous_ excellent engineers, the company did not yet have the _specialization_, nor had it yet built a coherent, defined, and marketable view of what "DevOps Engineering" meant _in Kin + Carta_. So, I would be reguarly tapped for input from Sales & Marketing, Engineering, and various internal teams for my on-the-ground experience, as Kin + Carta started to formalize those definitions and means of understanding.

1. Build fast-tracks to success for Entprise-sized Greenfield Engagements
   
   Infrastucture as Code (IAC) tooling enables not only rapid platform iteration but also reusable and shareable tooling & patterns. Knowing this we built and formalized some of the first repositories of standard and maintained IAC in Kin + Carta. Additionally, K+C engineers began reguarly contributing to public code repositories maintained by companies like Google, Microsoft, Elasticsearch, Redis, Netflix, Datadog, Dynatrace, and numerous others where public contribution positively impacted our experience with those tools and services at home.