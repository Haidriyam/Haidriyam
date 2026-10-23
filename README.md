# Muhammad Adeel Sajjad

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/adeel-haider-ae/)
[![GitHub](https://img.shields.io/badge/GitHub-Haidriyam-181717?style=flat&logo=github&logoColor=white)](https://github.com/Haidriyam)
[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/)
[![Docker](https://img.shields.io/badge/Docker-Rootless-2496ED?style=flat&logo=docker&logoColor=white)](https://www.docker.com/)
[![CI/CD](https://img.shields.io/badge/Pipeline-GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white)](https://github.com/Haidriyam)

Systems & Cyber-Physical Security Engineer bridging classical Electrical Power foundations with production-grade Linux systems, protocol telemetry parsers, and reproducible software-defined CPS testbeds.

---

### Research & Technical Focus Areas

- **Smart Grid & Microgrid Resilience:** Discrete Extended Kalman Filtering (EKF), secondary $P\text{-}f$ and $Q\text{-}V$ droop dynamics, multi-agent consensus algorithms, and False Data Injection (FDI) mitigation in distributed energy resources.
- **Electromagnetics & Power Electronics Modeling:** Mathematical modeling of Series-Series (SS) resonant inductive links, mutual inductance parameter extraction ($k, M$), Zero-Voltage Switching (ZVS) topologies, and Li-ion Thevenin equivalent circuits.
- **OT/SCADA & Network Security:** Deep-packet APDU dissection for Modbus-TCP, zero-trust command whitelisting, application-layer telemetry anomaly detection, and edge Mutual TLS (mTLS) architectures.
- **Computational Poetics & Diachronic Semantics:** Discrete sequence modeling, multi-scale Shannon entropy trajectories, Orthogonal Procrustes matrix alignment (SVD), and diachronic lexical fossilization across historical text corpora.
- **Production Systems & DevSecOps:** Automated Bandit SAST security sweeps, flake8/PEP8 compliance gates, rootless Docker packaging, and automated continuous integration pipelines.

---

### Featured Research Repositories & Software Testbeds

#### 1. Cyber-Physical Systems & Electrical Infrastructure

| Repository | Focus & Architecture | Security & CI/CD Pipeline | Status |
| :--- | :--- | :--- | :--- |
| **[microgrid-resilient-control](https://github.com/Haidriyam/microgrid-resilient-control)** | Secondary frequency consensus restoration on islanded AC microgrids. Implements inverter $P\text{-}f$ droop dynamics and outlier-rejection consensus to isolate False Data Injection (FDI) attacks. | Dynamic CPS test suite, flake8 style checks, rootless Docker container | ![CI](https://github.com/Haidriyam/microgrid-resilient-control/actions/workflows/devsecops-ci.yml/badge.svg) |
| **[battery-ekf-state-estimator](https://github.com/Haidriyam/battery-ekf-state-estimator)** | Discrete Extended Kalman Filter (EKF) for Li-ion SoC tracking using a 1-RC Thevenin equivalent circuit, paired with boundary-checked CAN-bus telemetry frame parsing. | Stochastic noise convergence tests, CAN frame validation suite, Bandit SAST | ![CI](https://github.com/Haidriyam/battery-ekf-state-estimator/actions/workflows/devsecops-ci.yml/badge.svg) |
| **[scada-ids-telemetry-engine](https://github.com/Haidriyam/scada-ids-telemetry-engine)** | Software-defined deep-packet APDU dissector for Modbus-TCP. Enforces zero-trust command whitelisting (blocking unauthorized coil writes) and checks telemetry against physical domain limits. | MBAP header boundary tests, malformed payload fuzzing, Bandit security sweeps | ![CI](https://github.com/Haidriyam/scada-ids-telemetry-engine/actions/workflows/devsecops-ci.yml/badge.svg) |
| **[wireless-power-transmission-sim](https://github.com/Haidriyam/wireless-power-transmission-sim)** | Coupled-mode magnetic resonance simulator modeling mutual inductance decay ($M$), unloaded quality factors ($Q$), and frequency bifurcation over variable air gaps (0–150 mm). | Deterministic numerical solvers, PEP8 compliance tests, automated GitHub CI | ![CI](https://github.com/Haidriyam/wireless-power-transmission-sim/actions/workflows/devsecops-ci.yml/badge.svg) |

#### 2. Enterprise Infrastructure, Zero-Trust & Network Defense

| Repository | Focus & Architecture | Security & CI/CD Pipeline | Status |
| :--- | :--- | :--- | :--- |
| **[zero-trust-pki-mesh](https://github.com/Haidriyam/zero-trust-pki-mesh)** | Multi-tier X.509 Certificate Authority provisioning root, intermediate, and leaf certificates for edge Mutual TLS (mTLS) reverse proxy enforcement and CIDR access control. | Cryptographic chain validation, Nginx mTLS handshake tests, SAST auditing | ![CI](https://github.com/Haidriyam/zero-trust-pki-mesh/actions/workflows/devsecops-ci.yml/badge.svg) |
| **[quantum-pqc-tls-canary](https://github.com/Haidriyam/quantum-pqc-tls-canary)** | NIST FIPS 203 ML-KEM-768 + X25519 hybrid key encapsulation canary evaluating handshake latency and MTU wire overhead for edge CPS telemetry links. | Downgrade attack detection test harness, wire overhead profiler, automated CI | ![CI](https://github.com/Haidriyam/quantum-pqc-tls-canary/actions/workflows/devsecops-ci.yml/badge.svg) |
| **[gitops-mesh-orchestrator](https://github.com/Haidriyam/gitops-mesh-orchestrator)** | Service mesh platform featuring dynamic TTL leases, round-robin load distribution, token-bucket burst rate-limiting, and ingress packet inspection. | Multi-node distributed test harness, injection payload defense, rootless container | ![CI](https://github.com/Haidriyam/gitops-mesh-orchestrator/actions/workflows/devsecops-ci.yml/badge.svg) |
| **[attack-surface-intel-pipeline](https://github.com/Haidriyam/attack-surface-intel-pipeline)** | External Attack Surface Management (EASM) engine aggregating reconnaissance data, scoring exposure vectors, and emitting SIEM-ready JSON telemetry. | Exposure heuristic unit tests, Bandit SAST security gate, automated Docker build | ![CI](https://github.com/Haidriyam/attack-surface-intel-pipeline/actions/workflows/devsecops-ci.yml/badge.svg) |

#### 3. Computational Humanities & Quantitative Language Systems

| Repository | Focus & Architecture | Interactive Demo & Pipeline | Status |
| :--- | :--- | :--- | :--- |
| **[victorian-serial-entropy](https://github.com/Haidriyam/victorian-serial-entropy)** | Information-theoretic analysis of serialized literary corpora. Validates the *Informational Bottleneck Hypothesis* across multi-scale sliding windows ($W=600, S=150$) and structural cliffhanger boundaries ($\Delta H < -0.45\text{ bits}$). | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Haidriyam/victorian-serial-entropy/blob/main/notebooks/demo.ipynb) | Active Research |
| **[diachronic-semantic-drift](https://github.com/Haidriyam/diachronic-semantic-drift)** | Diachronic lexical drift and statutory fossilization tracking across historical vector spaces aligned via Orthogonal Procrustes SVD ($W^{(t_1)} \approx W^{(t_2)}Q$). | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Haidriyam/diachronic-semantic-drift/blob/main/notebooks/drift_colab.ipynb) | Active Research |

---

### Engineering & Verification Standards

Every repository implements automated verification workflows to ensure reproducible execution and security isolation:
- **Continuous Integration (CI):** Automated GitHub Actions workflows trigger on every commit and pull request.
- **Static Application Security Testing (SAST):** Scanned via `bandit` to identify and block security vulnerabilities.
- **Code Style & Quality:** Strict PEP8 compliance enforced via `flake8` (`--max-line-length=120`).
- **Mathematical & Protocol Verification:** Automated `pytest` suites asserting convergence tolerances, protocol boundary constraints, and numerical stability.
- **Container Hardening:** Minimalist, rootless Docker images executing as unprivileged users (`UID 10001`).
