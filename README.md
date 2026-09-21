# Muhammad Adeel Sajjad

Cyber-Physical Systems, Infrastructure & Security Engineer bridging first-principle Electrical Engineering models (power dynamics, resonant electromagnetics, metrology) with hardened, production-grade systems software (eBPF, binary protocol parsers, Time-Sensitive Networking, and DevSecOps).

---

### Research & Technical Focus Areas

- **Smart Grid & Power System Dynamics:** Non-linear generator swing equation state estimation (EKF), secondary $P\text{--}f$ droop restoration, Byzantine-resilient consensus (W-MSR), and False Data Injection (FDI) mitigation.
- **Power Electronics & Non-Invasive Metrology:** GaN/SiC electro-thermal degradation tracking ($\Delta R_{ds(on)}$), 85 kHz SAE J2954 resonant WPT parameter extraction ($k, M, \text{ZVS}$), and Biot-Savart spatial magnetic field inversion via Tikhonov regularization.
- **OT/SCADA & Network Security:** IEEE 802.1Qbv Time-Aware Traffic Shaping (TAS), binary IEEE C37.118 synchrophasor frame parsing, deep-packet Modbus/IEC APDU inspection, and hybrid Post-Quantum Cryptography (NIST FIPS 203 ML-KEM).
- **Hardened Systems & DevSecOps:** Automated Bandit SAST security sweeps, zero-warning PEP8 code hygiene, rootless container packaging, and automated continuous integration.

---

### Research Repositories & Laboratory Testbeds

#### 1. Power Systems Dynamics, Synchrophasors & Microgrids

| Repository | Focus & Mathematical Core | Verification & DevSecOps | Status |
| :--- | :--- | :--- | :--- |
| **[synchrophasor-c37118-dynamic-estimator](https://github.com/Haidriyam/synchrophasor-c37118-dynamic-estimator)** | Binary IEEE C37.118.2 streaming PMU frame parser coupled with an observable 2nd-order non-linear swing equation Extended Kalman Filter (EKF) tracking rotor angle ($\delta$) and speed deviation ($\Delta\omega$). | IEEE C37.118 framing boundary tests, dynamic EKF convergence suites, Bandit SAST | ![CI](https://github.com/Haidriyam/synchrophasor-c37118-dynamic-estimator/actions/workflows/devsecops-ci.yml/badge.svg) |
| **[distributed-microgrid-der-consensus](https://github.com/Haidriyam/distributed-microgrid-der-consensus)** | Distributed secondary frequency restoration and battery SoC balancing engine using a Weighted Mean Subsequence Reduced (W-MSR) consensus filter to isolate adversarial Byzantine nodes under FDI attacks. | Multi-agent network graph convergence, out-of-band FDI outlier isolation tests, Docker build | ![CI](https://github.com/Haidriyam/distributed-microgrid-der-consensus/actions/workflows/devsecops-ci.yml/badge.svg) |
| **[microgrid-resilient-control](https://github.com/Haidriyam/microgrid-resilient-control)** | Secondary frequency consensus restoration and active power balance on islanded AC microgrids under distributed denial and manipulation attacks. | CPS dynamics test suite, PEP8 linting, rootless container deployment | ![CI](https://github.com/Haidriyam/microgrid-resilient-control/actions/workflows/devsecops-ci.yml/badge.svg) |
| **[battery-ekf-state-estimator](https://github.com/Haidriyam/battery-ekf-state-estimator)** | Discrete Extended Kalman Filter for Li-ion battery State-of-Charge (SoC) estimation paired with an automated, boundary-enforced CAN-bus telemetry frame fuzzer. | Stochastic noise convergence verification, CAN injection fuzzer tests, Bandit SAST | ![CI](https://github.com/Haidriyam/battery-ekf-state-estimator/actions/workflows/devsecops-ci.yml/badge.svg) |

#### 2. Power Electronics, Resonant Links & Contactless Metrology

| Repository | Focus & Mathematical Core | Verification & DevSecOps | Status |
| :--- | :--- | :--- | :--- |
| **[converter-health-telemetry-guard](https://github.com/Haidriyam/converter-health-telemetry-guard)** | Online prognostic health monitoring for wide-bandgap (GaN/SiC) semiconductors in data center DC-DC converters. Implements a Foster electro-thermal network to decouple junction heating ($T_j$) from lattice degradation ($\Delta R_{ds(on)} > 15\%$). | Electro-thermal ODE solver verification, premature failure trigger tests, Bandit SAST | ![CI](https://github.com/Haidriyam/converter-health-telemetry-guard/actions/workflows/devsecops-ci.yml/badge.svg) |
| **[wpt-adaptive-impedance-tracker](https://github.com/Haidriyam/wpt-adaptive-impedance-tracker)** | Analytical parameter observer for 85 kHz SAE J2954 resonant inductive links. Reconstructs mutual inductance ($M$) and coupling factor ($k$) solely from primary-side envelopes to enforce Zero-Voltage Switching (ZVS) phase margins. | Resonant RLC impedance modeling, lateral coil misalignment mitigation tests, CI pipeline | ![CI](https://github.com/Haidriyam/wpt-adaptive-impedance-tracker/actions/workflows/devsecops-ci.yml/badge.svg) |
| **[contactless-tmr-current-inverter](https://github.com/Haidriyam/contactless-tmr-current-inverter)** | Non-invasive current metrology testbed utilizing an 8-sensor Tunnel Magnetoresistance (TMR) circular array. Reconstructs 3-phase conductor currents ($I_a, I_b, I_c$) via 2D Biot-Savart geometric mapping and Tikhonov regularized pseudo-inversion. | Regularized condition number testing, 40 dB SNR noise injection suites, Docker packaging | ![CI](https://github.com/Haidriyam/contactless-tmr-current-inverter/actions/workflows/devsecops-ci.yml/badge.svg) |
| **[wireless-power-transmission-sim](https://github.com/Haidriyam/wireless-power-transmission-sim)** | High-frequency electromagnetic resonator modeling, analyzing unloaded quality factors ($Q$), spatial magnetic flux gradients, and link transfer efficiency. | Deterministic numerical solvers, PEP8 formatting checks, automated Actions CI | ![CI](https://github.com/Haidriyam/wireless-power-transmission-sim/actions/workflows/devsecops-ci.yml/badge.svg) |

#### 3. Industrial Protocol Security & Time-Sensitive Networking

| Repository | Focus & System Architecture | Verification & DevSecOps | Status |
| :--- | :--- | :--- | :--- |
| **[scada-priority-queue-canary](https://github.com/Haidriyam/scada-priority-queue-canary)** | Deterministic IEEE 802.1Qbv Time-Aware Shaper (TAS) emulating mixed-criticality substation communications. Enforces cyclic Gate Control Lists (GCL) to guarantee sub-4ms delivery of IEC 61850 GOOSE trip packets during line-rate DoS floods. | Cyclic GCL scheduling tests, DoS queue saturation isolation verification, Bandit SAST | ![CI](https://github.com/Haidriyam/scada-priority-queue-canary/actions/workflows/devsecops-ci.yml/badge.svg) |
| **[scada-ids-telemetry-engine](https://github.com/Haidriyam/scada-ids-telemetry-engine)** | Deep-packet APDU dissector for Modbus TCP and industrial telemetry with zero-trust function-code whitelisting and substation physical anomaly detection. | Memory safety fuzzing, protocol boundary rule enforcement, security scans | ![CI](https://github.com/Haidriyam/scada-ids-telemetry-engine/actions/workflows/devsecops-ci.yml/badge.svg) |

#### 4. Enterprise Infrastructure, Zero-Trust & Post-Quantum Systems

| Repository | Focus & Architecture | Verification & DevSecOps | Status |
| :--- | :--- | :--- | :--- |
| **[quantum-pqc-tls-canary](https://github.com/Haidriyam/quantum-pqc-tls-canary)** | NIST FIPS 203 ML-KEM-768 + X25519 hybrid key encapsulation mechanism protecting edge telemetry ingress against Harvest-Now-Decrypt-Later (HNDL) quantum vectors. | Cipher downgrade prevention tests, MTU wire overhead benchmarking, Bandit SAST | ![CI](https://github.com/Haidriyam/quantum-pqc-tls-canary/actions/workflows/devsecops-ci.yml/badge.svg) |
| **[zero-trust-pki-mesh](https://github.com/Haidriyam/zero-trust-pki-mesh)** | Automated X.509 Certificate Authority provisioning root, intermediate, and leaf certificates for mutual TLS (mTLS) reverse proxy enforcement across services. | Certificate lifecycle validation, Nginx mTLS handshake tests, SAST auditing | ![CI](https://github.com/Haidriyam/zero-trust-pki-mesh/actions/workflows/devsecops-ci.yml/badge.svg) |
| **[gitops-mesh-orchestrator](https://github.com/Haidriyam/gitops-mesh-orchestrator)** | Service mesh platform featuring dynamic TTL leases, round-robin load distribution, token-bucket burst rate-limiting, and CIDR ingress boundary inspection. | Multi-node distributed test harness, payload injection defense, rootless container | ![CI](https://github.com/Haidriyam/gitops-mesh-orchestrator/actions/workflows/devsecops-ci.yml/badge.svg) |
| **[attack-surface-intel-pipeline](https://github.com/Haidriyam/attack-surface-intel-pipeline)** | External Attack Surface Management (EASM) engine aggregating multi-source reconnaissance data, scoring exposure vectors, and emitting SIEM-ready JSON telemetry. | Exposure heuristic unit tests, Bandit security gate, automated container compilation | ![CI](https://github.com/Haidriyam/attack-surface-intel-pipeline/actions/workflows/devsecops-ci.yml/badge.svg) |

---

### Pipeline Quality & Verification Standard

Every repository operates under strict production engineering standards:
- **Continuous Integration (CI):** Automated GitHub Actions workflows trigger on every commit and pull request.
- **Static Application Security Testing (SAST):** Scanned via `bandit` with high-severity issue blocking.
- **Code Style & Quality:** Formatted to PEP8 standards verified via `flake8` (`--max-line-length=120`).
- **Mathematical & Protocol Verification:** Pytest suites assert convergence tolerances, boundary validations, and numerical stability.
- **Container Hardening:** Minimalist, rootless Docker builds run as unprivileged users (`UID 10001`).
