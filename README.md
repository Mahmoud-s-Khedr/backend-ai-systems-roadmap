# Backend, AI & Systems Engineering Roadmap

A long-term, project-driven study roadmap focused on **backend engineering, distributed systems, production AI, cloud/platform engineering, SRE/observability, security, and Go**.

This repository is not meant to be a collection of certificates or passive course notes. The goal is to turn each study block into **working systems, benchmarks, architecture decisions, operational evidence, and portfolio-quality engineering artifacts**.

## Core rule

> Keep one serious production-style system alive throughout the roadmap and continuously improve it as new topics are learned.

Examples of evidence to produce as the roadmap progresses:

- load-test and latency reports
- PostgreSQL query-plan investigations
- architecture diagrams and ADRs
- Terraform modules and reproducible environments
- CI/CD pipelines
- SLOs, dashboards, traces and alerts
- incident postmortems
- security reviews against ASVS / LLMSVS
- production AI evaluations and cost/latency measurements
- Go services with profiling and benchmark results

**DDIA runs in parallel starting from the database phase.**

---

# Study roadmap

## Phase 1 — Systems foundations

- [ ] **1. Hussein Nasser — Fundamentals of Operating Systems**  
  https://www.udemy.com/course/fundamentals-of-operating-systems/  
  Build the OS foundation underneath backend and infrastructure engineering: processes, threads, syscalls, memory, CPU/cache behavior, filesystems, sockets and asynchronous I/O.

- [ ] **2. Hussein Nasser — Fundamentals of Network Engineering**  
  https://www.udemy.com/course/fundamentals-of-networking-for-effective-backend-design/  
  Deepen TCP/IP, UDP, routing, DNS, TLS and network behavior from a backend perspective. This later compounds into AWS, NGINX, Kubernetes and troubleshooting.

- [ ] **3. Hussein Nasser — Fundamentals of Backend Engineering**  
  https://www.udemy.com/course/fundamentals-of-backend-communications-and-protocols/  
  Connect OS and networking knowledge to HTTP, HTTP/2/3, gRPC, WebSockets, TLS, QUIC, proxies and backend communication design.

## Phase 2 — Databases and distributed systems

- [ ] **4. Hussein Nasser — Fundamentals of Database Engineering**  
  https://www.udemy.com/course/database-engines-crash-course/  
  Study ACID, pages, indexes, B-trees, concurrency, replication, partitioning, sharding and storage-engine trade-offs.

- [ ] **5. Designing Data-Intensive Applications, 2nd Edition — Martin Kleppmann & Chris Riccomini** *(parallel)*  
  https://www.oreilly.com/library/view/designing-data-intensive-applications/9781098119058/  
  Build the distributed-systems mental model behind storage, replication, consistency, transactions, failures, streams and architectural trade-offs. Read slowly in parallel with the rest of the roadmap.

- [ ] **6. PostgreSQL — Performance Tips**  
  https://www.postgresql.org/docs/current/performance-tips.html  
  Apply database theory to PostgreSQL using `EXPLAIN`, `EXPLAIN ANALYZE`, planner statistics and real query-performance investigations.

## Phase 3 — Deepen the current Node backend stack

- [ ] **7. Hussein Nasser — NodeJS Internals and Architecture**  
  https://www.udemy.com/course/nodejs-internals-and-architecture/  
  Understand the commercial stack underneath Express/Fastify: V8, libuv, event loop, async I/O, streams, networking, worker threads and performance.

- [ ] **8. Hussein Nasser — Troubleshooting Backend Systems**  
  https://www.udemy.com/course/discovering-backend-bottlenecks-unlocking-peak-performance/  
  Learn to diagnose latency and bottlenecks using measurement, packet inspection, proxies and production-style debugging techniques.

- [ ] **9. Grafana k6 — Get Started**  
  https://grafana.com/docs/k6/latest/get-started/  
  Learn reproducible load testing. Measure throughput, errors, p50/p95/p99 latency and breaking points before and after optimizations.

- [ ] **10. Hussein Nasser — Introduction to NGINX**  
  https://www.udemy.com/course/nginx-crash-course/  
  Deepen reverse proxying, L4/L7 load balancing, TLS termination, HTTP/2, WebSockets, upstreams and timeout behavior.

- [ ] **11. Hussein Nasser — Realtime Backend System Design with WebSockets**  
  https://www.udemy.com/course/scalable-real-time-backends-with-websockets/  
  Go beyond Socket.io usage and understand persistent connections, scaling, proxying and real-time backend architecture.

## Phase 4 — Production Python

- [ ] **12. Python — Official Tutorial**  
  https://docs.python.org/3/tutorial/  
  Fast bridge into idiomatic Python for an experienced programmer. Focus on Python-specific semantics and skip generic programming basics.

- [ ] **13. Python — `asyncio`**  
  https://docs.python.org/3/library/asyncio.html  
  Learn Python's async/concurrency model and consciously compare it with Node/libuv.

- [ ] **14. FastAPI — Official Tutorial**  
  https://fastapi.tiangolo.com/tutorial/  
  Build production Python APIs and AI-facing services with validation, dependencies, security, async behavior and testing.

- [ ] **15. SQLAlchemy 2.0 — Unified Tutorial**  
  https://docs.sqlalchemy.org/en/20/tutorial/  
  Learn engines, connection pools, transactions, SQL expressions, sessions and ORM behavior properly.

- [ ] **16. pytest — Getting Started + Documentation**  
  https://docs.pytest.org/en/stable/getting-started.html  
  Transfer a test-heavy workflow into Python with unit, integration and API/service testing.

## Phase 5 — Applied AI engineering

- [ ] **17. Ed Donner — AI Coder**  
  https://www.udemy.com/course/ai-coder-from-vibe-coder-to-agentic-engineer/  
  Formalize AI-assisted development workflows: coding agents, context management, subagents, orchestration, MCP, Claude Code and Codex.

- [ ] **18. Ed Donner — AI Leader**  
  https://www.udemy.com/course/executive-briefing-generative-ai-and-large-language-models-llm/  
  Learn the commercial layer: AI project selection, ROI, model/product trade-offs and communicating AI investments with clients and founders.

- [ ] **19. Ed Donner — AI Engineer Core Track**  
  https://www.udemy.com/course/llm-engineering-master-ai-and-large-language-models/  
  Main applied-AI foundation: model selection, multimodality, embeddings, RAG, retrieval, fine-tuning concepts, tools/function calling and agents.

- [ ] **20. Ed Donner — AI Builder**  
  https://www.udemy.com/course/ai-builder-with-n8n-create-agents-voice-agents/  
  Learn rapid commercial AI delivery with n8n, integrations, RAG, voice agents, MCP and automation workflows.

## Phase 6 — Infrastructure as Code and AWS delivery

- [ ] **21. KodeKloud — HashiCorp Certified Terraform Associate 004**  
  https://kodekloud.com/courses/hashicorp-certified-terraform-associate-004  
  Structured Terraform foundation through labs: HCL, resources, providers, workflow, state, modules, imports and lifecycle.

- [ ] **22. KodeKloud — AWS Workshop with Terraform**  
  https://kodekloud.com/courses/learn-by-doing-aws-workshop-with-terraform  
  Convert AWS knowledge into reproducible infrastructure and practice real AWS provisioning with Terraform.

- [ ] **23. HashiCorp — Terraform AWS Get Started**  
  https://developer.hashicorp.com/terraform/tutorials/aws-get-started  
  Reinforce the canonical Terraform workflow directly from HashiCorp: initialize, plan, provision, change and destroy.

- [ ] **24. HashiCorp — Terraform Modules**  
  https://developer.hashicorp.com/terraform/tutorials/modules  
  Learn reusable infrastructure design instead of maintaining giant environment-specific Terraform files.

- [ ] **25. HashiCorp — Terraform State**  
  https://developer.hashicorp.com/terraform/tutorials/state  
  Understand drift, imports, state migration/refactoring and the mapping between configuration and real infrastructure.

- [ ] **26. HashiCorp — Terraform S3 Backend**  
  https://developer.hashicorp.com/terraform/language/backend/s3  
  Learn production remote-state storage, locking and recovery rather than keeping state only on a laptop.

- [ ] **27. HashiCorp — Terraform Tests**  
  https://developer.hashicorp.com/terraform/tutorials/configuration-language/test  
  Extend the testing discipline into IaC using Terraform's native test framework.

- [ ] **28. GitHub Actions — Quickstart + Documentation**  
  https://docs.github.com/en/actions/get-started/quickstart  
  Implement CI/CD: test → build image → push image → deploy. The goal is a working pipeline, not course completion.

## Phase 7 — Production AI and agents

- [ ] **29. Ed Donner — AI Engineer Production Track**  
  https://www.udemy.com/course/generative-and-agentic-ai-in-production/  
  Combine AI with production engineering: cloud deployment, Terraform, CI/CD, observability, security, resilience, guardrails, cost and production architecture.

- [ ] **30. Ed Donner — AI Engineer Agentic Track**  
  https://www.udemy.com/course/the-complete-agentic-ai-engineering-course/  
  Deepen agent systems: tools, MCP, OpenAI Agents SDK, LangGraph, CrewAI, AutoGen and multi-agent architectures.

## Phase 8 — Kubernetes and reliability engineering

- [ ] **31. Kubernetes — Official Tutorials**  
  https://kubernetes.io/docs/tutorials/  
  Learn Pods, Deployments, Services, configuration, storage, workloads, networking and security from the canonical docs.

- [ ] **32. KodeKloud — Certified Kubernetes Administrator (CKA) Course**  
  https://kodekloud.com/courses/cka-certification-course-certified-kubernetes-administrator  
  Go substantially deeper through labs: cluster architecture, networking, storage, scheduling, security, upgrades and troubleshooting.

- [ ] **33. Google — Site Reliability Workbook**  
  https://sre.google/workbook/table-of-contents/  
  Study SLIs/SLOs, error budgets, monitoring, alerting, toil, incidents, postmortems, overload and canary releases.

## Phase 9 — Observability

- [ ] **34. OpenTelemetry — JavaScript Documentation**  
  https://opentelemetry.io/docs/languages/js/  
  Instrument Node services for traces and metrics and learn context propagation, exporters, SDKs and sampling.

- [ ] **35. Prometheus — Official Tutorials**  
  https://prometheus.io/docs/tutorials/  
  Learn metrics, instrumentation, PromQL fundamentals and alerting.

- [ ] **36. Grafana — Fundamentals**  
  https://grafana.com/tutorials/grafana-fundamentals/  
  Turn metrics/logs into dashboards and alerts that answer operational questions about production systems.

## Phase 10 — Application and AI security

- [ ] **37. PortSwigger — Web Security Academy**  
  https://portswigger.net/web-security  
  Practical application-security labs. Prioritize auth/authz, OAuth/JWT, API security, SSRF, injection, uploads, race conditions and Web LLM attacks.

- [ ] **38. OWASP — Application Security Verification Standard 5.0**  
  https://owasp.org/www-project-application-security-verification-standard/  
  Use ASVS as a verification checklist against software you actually build rather than a book to memorize.

- [ ] **39. OWASP — Large Language Model Security Verification Standard (LLMSVS)**  
  https://owasp.org/www-project-llm-verification-standard/  
  Extend application security into LLM systems: integrations, agents, lifecycle, storage, monitoring and AI-specific attack surfaces.

## Phase 11 — Go specialization

- [ ] **40. Go — Official Tutorials**  
  https://go.dev/doc/tutorial/  
  Learn Go quickly as an experienced engineer: modules, methods/interfaces, databases, HTTP services, generics, tests and language fundamentals.

- [ ] **41. Ardan Labs — Ultimate Go Tour**  
  https://tour.ardanlabs.com/  
  Bridge the gap between syntax and deeper Go mechanics, concurrency, memory semantics and systems-oriented engineering.

- [ ] **42. Ardan Labs — Ultimate Go Bundle**  
  https://www.ardanlabs.com/training/self-paced/individuals/bundles/go/  
  Final deep specialization if Go becomes a principal professional language: production services, concurrency, performance, debugging and design.

---

# How to use this repository

1. Check off resources only when the corresponding capability has been **applied**, not merely watched/read.
2. Keep concise notes under `notes/`.
3. Store performance investigations under `benchmarks/`.
4. Record architecture choices under `architecture/`.
5. Write realistic postmortems under `incidents/` when something breaks.
6. Store SLOs, dashboards and telemetry notes under `observability/`.
7. Track infrastructure work under `infra/`.
8. Track security reviews under `security/`.
9. Use `projects/` to document the continuing production-style project(s).
10. Use `go/` for the final Go specialization and systems experiments.

## Completion standard

A phase is not complete just because the course is finished. It is complete when I can:

- explain the key concepts without relying on AI;
- debug the common failure modes;
- apply the ideas in a real system;
- measure or verify the result;
- publish evidence of what changed and why.

See [`STUDY_RULES.md`](STUDY_RULES.md) and [`PROGRESS.md`](PROGRESS.md) for the operating system for this roadmap.
