# DevOps & Development Learning Roadmap

A progressive curriculum from zero to working proficiency. Time estimates assume ~8–10 hours/week. 

**How to use this:** Check off lessons as you complete them. Build something small and real at the end of every section — the tooling only sticks through repetition.

**Progress:** 0 / 17 sections complete

---

## Section 1 — Computing Foundations
*Estimated: 2–3 weeks*

- [ ] How computers execute programs: CPU, memory, disk, processes
- [ ] Operating system basics: kernel, user space, system calls
- [ ] Filesystems, paths, permissions, and inodes
- [ ] Processes, threads, signals, and exit codes
- [ ] Environment variables and the shell environment
- [ ] Text encoding, line endings, and why they break things

---

## Section 2 — Linux and the Command Line
*Estimated: 3–4 weeks*

- [ ] Navigating the filesystem: `ls`, `cd`, `find`, `tree`
- [ ] Reading and editing files: `cat`, `less`, `vim`/`nano`
- [ ] Text processing: `grep`, `sed`, `awk`, `cut`, `sort`, `uniq`
- [ ] Pipes, redirection, and exit-status chaining
- [ ] Users, groups, `sudo`, and file permission models
- [ ] Package management: `apt`/`yum`/`dnf`
- [ ] Process management: `ps`, `top`, `htop`, `kill`, `systemd`
- [ ] Disk and resource inspection: `df`, `du`, `free`, `lsof`
- [ ] SSH: keys, config files, tunneling, agent forwarding
- [ ] Cron, systemd timers, and scheduled jobs

---

## Section 3 — Networking Fundamentals
*Estimated: 2–3 weeks*

- [ ] The OSI and TCP/IP models in practical terms
- [ ] IP addressing, subnets, and CIDR notation
- [ ] DNS: record types, resolution, TTLs, propagation
- [ ] TCP vs. UDP, ports, and the three-way handshake
- [ ] HTTP/HTTPS: methods, status codes, headers, keep-alive
- [ ] TLS: certificates, chains of trust, expiry, Let's Encrypt
- [ ] Load balancing: L4 vs. L7, round-robin, health checks
- [ ] Reverse proxies: Nginx or Caddy configuration
- [ ] Firewalls, NAT, and security groups
- [ ] Debugging tools: `dig`, `curl`, `netstat`/`ss`, `tcpdump`, `traceroute`

---

## Section 4 — Programming and Scripting
*Estimated: 4–6 weeks*

- [ ] Bash scripting: variables, conditionals, loops, functions
- [ ] Bash robustness: `set -euo pipefail`, quoting, trap handlers
- [ ] Python fundamentals: types, control flow, functions, modules
- [ ] Python for ops: `os`, `subprocess`, `pathlib`, `argparse`, `requests`
- [ ] Working with JSON, YAML, and TOML
- [ ] Virtual environments and dependency pinning
- [ ] Writing a CLI tool with proper error handling and logging
- [ ] *(Optional but valuable)* Go basics — the language most infra tooling is written in

---

## Section 5 — Version Control with Git
*Estimated: 2 weeks*

- [ ] The Git object model: commits, trees, blobs, refs
- [ ] Core workflow: `add`, `commit`, `push`, `pull`, `fetch`
- [ ] Branching, merging, and resolving conflicts
- [ ] Rebasing, interactive rebase, and cherry-picking
- [ ] Undoing things: `reset`, `revert`, `restore`, `reflog`
- [ ] Tags, semantic versioning, and release conventions
- [ ] Branching strategies: trunk-based vs. GitFlow
- [ ] Pull requests, code review etiquette, and `CODEOWNERS`
- [ ] Git hooks and pre-commit automation

---

## Section 6 — Software Development Practices
*Estimated: 3–4 weeks*

- [ ] Clean code: naming, function size, separation of concerns
- [ ] Unit testing and test-driven development
- [ ] Integration and end-to-end testing
- [ ] Test doubles: mocks, stubs, fakes
- [ ] Linting, formatting, and static analysis
- [ ] Debugging methodically: breakpoints, bisection, logging
- [ ] REST API design and versioning
- [ ] Twelve-Factor App methodology
- [ ] Configuration management and secrets handling in code
- [ ] Technical documentation and READMEs that work

---

## Section 7 — Databases and Storage
*Estimated: 2–3 weeks*

- [ ] Relational modeling and normalization
- [ ] SQL: joins, aggregates, subqueries, window functions
- [ ] Indexes, query plans, and performance tuning
- [ ] Transactions, isolation levels, and locking
- [ ] NoSQL categories: key-value, document, column, graph
- [ ] Caching with Redis: patterns and invalidation
- [ ] Backups, restores, and point-in-time recovery
- [ ] Schema migrations in a CI/CD pipeline
- [ ] Replication, read replicas, and sharding basics

---

## Section 8 — Containers
*Estimated: 3 weeks*

- [ ] Why containers: namespaces, cgroups, union filesystems
- [ ] Docker CLI: images, containers, volumes, networks
- [ ] Writing Dockerfiles and understanding layer caching
- [ ] Multi-stage builds and minimal base images
- [ ] Image security: scanning, non-root users, distroless
- [ ] Docker Compose for multi-service local development
- [ ] Registries: tagging strategies, pushing, pulling, cleanup
- [ ] Container logging, resource limits, and health checks

---

## Section 9 — Container Orchestration with Kubernetes
*Estimated: 5–6 weeks*

- [ ] Cluster architecture: control plane, nodes, etcd
- [ ] Pods, ReplicaSets, and Deployments
- [ ] Services, Ingress, and cluster networking
- [ ] ConfigMaps and Secrets
- [ ] Volumes, PersistentVolumes, and StorageClasses
- [ ] Namespaces, resource quotas, requests and limits
- [ ] StatefulSets, DaemonSets, Jobs, and CronJobs
- [ ] Autoscaling: HPA, VPA, and cluster autoscaling
- [ ] RBAC, service accounts, and pod security
- [ ] Helm charts and templating
- [ ] Probes, rolling updates, and rollback strategies
- [ ] Troubleshooting: `kubectl describe`, `logs`, `exec`, `events`

---

## Section 10 — Infrastructure as Code
*Estimated: 3–4 weeks*

- [ ] Declarative vs. imperative infrastructure
- [ ] Terraform: providers, resources, state, and the plan/apply cycle
- [ ] Terraform modules, variables, outputs, and workspaces
- [ ] Remote state, locking, and drift detection
- [ ] Ansible: inventories, playbooks, roles, idempotency
- [ ] Packer and immutable machine images
- [ ] Testing and policy-checking infrastructure code
- [ ] GitOps with ArgoCD or Flux

---

## Section 11 — CI/CD
*Estimated: 3 weeks*

- [ ] Continuous integration principles and fast feedback loops
- [ ] Pipeline anatomy: build, test, scan, package, deploy
- [ ] Hands-on with GitHub Actions (or GitLab CI / Jenkins)
- [ ] Artifact management and build reproducibility
- [ ] Managing pipeline secrets and OIDC-based cloud auth
- [ ] Deployment strategies: blue-green, canary, rolling, feature flags
- [ ] Automated rollback and deployment gates
- [ ] Pipeline optimization: caching, parallelism, matrix builds

---

## Section 12 — Cloud Platforms
*Estimated: 4–5 weeks — pick ONE provider*

- [ ] Cloud service models and the shared responsibility model
- [ ] Identity and access management: users, roles, policies, least privilege
- [ ] Compute: VMs, autoscaling groups, serverless functions
- [ ] Networking: VPCs, subnets, routing, gateways, peering
- [ ] Storage: object, block, and file storage tiers
- [ ] Managed databases and caching services
- [ ] Managed Kubernetes: EKS / GKE / AKS
- [ ] Cloud-native CI/CD and container registries
- [ ] Cost management, tagging, and budget alerts
- [ ] Multi-region design and disaster recovery

---

## Section 13 — Observability and Monitoring
*Estimated: 3 weeks*

- [ ] The three pillars: metrics, logs, traces
- [ ] Prometheus: exporters, PromQL, scraping, recording rules
- [ ] Grafana dashboards and visualization design
- [ ] Structured logging and centralized aggregation (Loki / ELK)
- [ ] Distributed tracing with OpenTelemetry and Jaeger
- [ ] Alerting: thresholds, alert fatigue, routing, escalation
- [ ] Instrumenting your own applications
- [ ] The USE and RED methods for signal selection

---

## Section 14 — Security and DevSecOps
*Estimated: 3 weeks*

- [ ] Threat modeling and the OWASP Top 10
- [ ] Secrets management: Vault, cloud secret stores, rotation
- [ ] Dependency scanning and SBOM generation
- [ ] SAST, DAST, and container image scanning in CI
- [ ] Network security: zero trust, mTLS, service meshes
- [ ] Compliance basics: audit logs, CIS benchmarks, policy as code
- [ ] Incident response for security events
- [ ] Supply-chain security and artifact signing

---

## Section 15 — Site Reliability Engineering
*Estimated: 3 weeks*

- [ ] SLIs, SLOs, SLAs, and error budgets
- [ ] Capacity planning and load testing
- [ ] Designing for failure: retries, timeouts, circuit breakers, backoff
- [ ] On-call rotations and runbook writing
- [ ] Incident command and effective communication during outages
- [ ] Blameless postmortems and root cause analysis
- [ ] Chaos engineering fundamentals
- [ ] Toil identification and automation prioritization

---

## Section 16 — Culture and Collaboration
*Estimated: 1–2 weeks*

- [ ] What DevOps actually is: the cultural argument, not the toolchain
- [ ] Agile and Scrum in practice
- [ ] Platform engineering and internal developer platforms
- [ ] DORA metrics: deployment frequency, lead time, MTTR, change failure rate
- [ ] Writing design docs and RFCs
- [ ] Working across dev, ops, and security boundaries

---

## Section 17 — Capstone Projects

- [ ] Deploy a three-tier web app on a single VM, configured entirely by Ansible
- [ ] Containerize it and run it locally with Docker Compose
- [ ] Build a full CI/CD pipeline with tests, scanning, and automated deploy
- [ ] Provision the entire cloud environment with Terraform from scratch
- [ ] Migrate the app to Kubernetes with Helm and horizontal autoscaling
- [ ] Add full observability: metrics, dashboards, alerts, and traces
- [ ] Define SLOs, then intentionally break the system and write a postmortem

---

## Notes to Self

**Pick one, not all.** One cloud provider, one CI tool. The concepts transfer. Chasing breadth before depth is the most common way people stall out.

**Don't skip Sections 1–7.** They're the "Development" half and are non-negotiable prerequisites. A lot of people jump straight to Kubernetes and end up unable to debug anything.

**Build after every section.** Even something small.

### Personal log

| Date | Section | What I built / learned |
|------|---------|------------------------|
|      |         |                        |
|      |         |                        |
|      |         |                        |
