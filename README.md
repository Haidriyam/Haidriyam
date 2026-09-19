# Muhammad Adeel Sajjad

Systems, Infrastructure & Cyber-Physical Security Engineer specializing in cloud operations, network reliability, industrial protocol security, and embedded physical modeling.

---

### Core Competencies

- **Enterprise Systems & Cloud Infrastructure:** Zero-Downtime Blue/Green Deployments, Service Discovery Mesh, Token-Bucket Traffic Shaping, Docker, Nginx Reverse Proxy Architecture
- **DevSecOps & Zero-Trust Security:** X.509 PKI/mTLS Mesh Authentication, Dynamic CIDR Policy Enforcement, Bandit SAST Auditing, CAN-Bus & SCADA APDU Fuzzing
- **Cyber-Physical Systems (CPS) & EE Foundations:** Coupled-Mode Inductive Modeling, Inverter P-f/Q-V Droop Dynamics, Byzantine/FDI Resilient Consensus, Discrete Extended Kalman Filtering (EKF)

---

### Featured Showcase Repositories

#### 1. Cyber-Physical Systems & Electrical Infrastructure

| Repository | Focus & Architecture | Security & CI/CD Pipeline |
| :--- | :--- | :--- |
| **[microgrid-resilient-control](https://github.com/Haidriyam/microgrid-resilient-control)** | Secondary frequency consensus restoration on islanded AC microgrids under False Data Injection (FDI) attacks. | Bandit SAST, PEP8 linting, CPS dynamics test suite, hardened Docker image |
| **[battery-ekf-state-estimator](https://github.com/Haidriyam/battery-ekf-state-estimator)** | Discrete Extended Kalman Filter (EKF) for Li-ion SoC estimation combined with boundary-checked CAN-bus telemetry parsing and frame fuzzing. | Stochastic convergence verification, frame fuzzing suite, rootless container build |
| **[scada-ids-telemetry-engine](https://github.com/Haidriyam/scada-ids-telemetry-engine)** | Deep-packet APDU dissector for Modbus TCP/IEC SCADA protocols with zero-trust command whitelisting and substation physical anomaly detection. | Memory safety fuzzing, physical boundary rule tests, Bandit security scans |
| **[wireless-power-transmission-sim](https://github.com/Haidriyam/wireless-power-transmission-sim)** | Mathematical modeling of resonant magnetic inductive coupling, unloaded Q-factor dynamics, and mutual link efficiency optimization. | Deterministic numerical testing, PEP8 style enforcement, automated CI workflow |

#### 2. Enterprise IT, Zero-Trust & DevSecOps

| Repository | Focus & Architecture | Security & CI/CD Pipeline |
| :--- | :--- | :--- |
| **[zero-trust-pki-mesh](https://github.com/Haidriyam/zero-trust-pki-mesh)** | Internal X.509 Certificate Authority provisioning root, intermediate, and leaf certificates for edge Mutual TLS (mTLS) reverse proxy enforcement. | Cryptographic lifecycle validation, Nginx mTLS handshake tests, SAST auditing |
| **[gitops-mesh-orchestrator](https://github.com/Haidriyam/gitops-mesh-orchestrator)** | Service mesh orchestrator featuring dynamic TTL heartbeat leases, round-robin load distribution, token-bucket burst rate-limiting, and CIDR ingress inspection. | Distributed multi-node test harness, injection payload defense, rootless container |
| **[attack-surface-intel-pipeline](https://github.com/Haidriyam/attack-surface-intel-pipeline)** | External Attack Surface Management (EASM) engine aggregating multi-source recon data, scoring exposure vectors, and outputting SIEM-ready JSON telemetry. | Exposure heuristic unit tests, Bandit SAST security gate, automated Docker builds |

---

### Pipeline Quality & Verification Standard

Every repository adheres to production-grade DevSecOps standards:
- **Continuous Integration (CI):** Fully automated GitHub Actions pipelines running on every commit and pull request.
- **Static Analysis (SAST):** Automated vulnerability scanning using `bandit` to ensure zero high/medium security issues in application logic.
- **Strict Code Hygiene:** Enforced PEP8 compliance with `flake8` zero-tolerance configurations.
- **Automated Testing:** Test suites verifying mathematical convergence, security perimeter fuzzing, and failure recovery.
- **Hardened Packaging:** Rootless Docker containers prepared for microservice orchestration.
