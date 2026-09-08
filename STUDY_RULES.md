# Study Rules

This roadmap is intentionally broad. These rules prevent it from turning into passive course consumption.

## 1. Build continuously

Every major topic must modify or improve a real production-style system.

Examples:

- OS/networking → inspect sockets, processes, syscalls, latency and resource behavior.
- Databases → investigate query plans, indexes and transaction behavior.
- k6 → establish performance baselines and breaking points.
- Terraform → reproduce infrastructure from code.
- SRE → define SLIs/SLOs and failure budgets.
- Observability → instrument traces, metrics and alerts.
- Security → run verification checklists and fix findings.
- Go → build something where Go has a legitimate systems/backend advantage.

## 2. Evidence beats completion

A course is not complete merely because all videos were watched.

For important resources, produce at least one artifact:

- benchmark
- architecture decision record
- debugging write-up
- test suite
- dashboard
- postmortem
- infrastructure module
- security review
- cost analysis
- small production service

## 3. AI is allowed — dependency is not

Use coding agents aggressively for implementation, exploration, test generation and repetitive work.

But be able to explain and debug without AI:

- processes/threads and async I/O
- TCP, DNS, HTTP and TLS basics
- transactions, indexes and query plans
- Node event-loop behavior
- Python async behavior
- Terraform state and dependency behavior
- container/networking fundamentals
- Kubernetes core objects and debugging flow
- SLO/incident concepts
- authentication/authorization boundaries
- Go concurrency and memory semantics once Go becomes a specialization

If AI generated code fails in production, ownership remains mine.

## 4. Measure before optimizing

Never claim a performance improvement without a baseline.

Record at minimum where applicable:

- throughput
- p50/p95/p99 latency
- error rate
- CPU/memory
- database query time
- external API/model latency
- AI tokens/cost per operation

## 5. Prefer depth over adding resources

Do not keep expanding this roadmap every time a new tool becomes popular.

New resources should be added only if they close a demonstrated gap in:

- a current project
- a target job description
- a client requirement
- an interview weakness

## 6. Use documentation as documentation

Official docs do not always need to be read cover-to-cover. For tools such as Terraform, Kubernetes, PostgreSQL, OpenTelemetry and Go, learn the core path and then return to documentation just in time while building.

## 7. Keep DDIA slow

DDIA runs in parallel. Do not pause practical learning for weeks just to finish the book.

Suggested rhythm: roughly one chapter per week, slower when a chapter deserves experiments or further reading.

## 8. Do not abandon the current monetization stack prematurely

Node.js remains useful while deeper backend, infrastructure, AI and Go capabilities are developed. New languages should expand capability rather than reset professional experience.

## 9. Review every 8–12 weeks

Ask:

- What did I actually ship?
- What can I now debug that I could not before?
- What evidence can an employer/client inspect?
- Which roadmap topics are proving commercially useful?
- Which resources should be delayed because they are not relevant yet?
