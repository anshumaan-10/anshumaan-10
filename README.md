<h1 align="center">Hi 👋, I'm Anshumaan Singh</h1>
<h3 align="center">Security Systems Engineer | DevSecOps | Cloud & Application Security</h3>

<img align="right" alt="Security Engineering" width="400" src="https://raw.githubusercontent.com/devSouvik/devSouvik/master/gif3.gif">

---

## 🔐 About Me

I engineer security the same way high-scale teams engineer reliability: as a **system property**—designed, enforced, and continuously verified.

I work across the SDLC, but my real domain is **security system design**: defining trust boundaries, constraining blast radius, enforcing secure defaults, and ensuring production behavior is predictable even under adversarial pressure.

I don’t treat security as “findings.”  
I treat security as **invariants**: rules that must remain true regardless of code changes, deployments, or operational stress.

- 📍 Bengaluru, India  
- 🏢 Information Security Analyst (IC-2) @ **ZEE Entertainment Enterprises Ltd**
- 🧩 Secured **350+ microservices** from development → production using centralized DevSecOps security architecture :contentReference[oaicite:1]{index=1}

---

## 🧠 What I Build (Security by Design, not by Checklist)

### 1) Trust Architecture & Secure System Design
I design secure systems by explicitly defining:
- **principals** (human identities, service identities, workload identities)
- **trust zones** and cross-boundary traffic flows
- **authorization decisions** (who can do what, where enforcement happens)
- **data boundaries** (PII/Secrets, storage, transit, exposure surfaces)
- **failure modes** (what breaks first, how it degrades, what becomes exploitable)
- **attacker paths** (abuse routes, escalation edges, bypass opportunities)

I convert these into engineering constraints:
- **deny-by-default** access models
- least privilege at identity + runtime
- isolation boundaries that limit lateral movement
- secure-by-default interfaces and hardened configuration baselines

---

### 2) CI/CD as a Security Control Plane (not a build script)
I treat CI/CD as a **security boundary** and build pipelines that guarantee:
- only reviewed changes can become deployable artifacts
- policy violations fail early (pre-merge / pre-deploy)
- artifacts are traceable to change + approval (auditability)
- promotion paths are controlled and non-bypassable

I’ve built centralized DevSecOps pipelines for **350+ microservices** with:
- SAST / DAST / SCA / Secret scanning
- container image scanning + SBOM generation
- binary authorization at build time
- Policy-as-Code enforcement that breaks builds on defined risk thresholds :contentReference[oaicite:2]{index=2}

---

### 3) Supply Chain Hardening & Artifact Integrity
Most modern incidents start with **tampering**, not “exploitation”.

I harden the supply chain by enforcing:
- controlled artifact creation + promotion paths
- strict versioning and release immutability principles
- provenance-style traceability (what was built, where, by whom)
- consistent verification gates so “passed” actually means “safe to ship”

---

### 4) Kubernetes & Runtime Security as Engineering Constraints
Kubernetes security fails when it’s treated as YAML hygiene.  
I secure clusters by designing for runtime reality:
- workloads drift
- permissions sprawl
- network boundaries get ignored
- “temporary exceptions” become permanent exposure

What I implement and enforce:
- admission-time guardrails using **OPA Gatekeeper** policies to block non-compliant workloads :contentReference[oaicite:3]{index=3}
- detection + threat visibility using **Falco-based Kubernetes Threat Detection (KTD)** through Google Cloud SCC :contentReference[oaicite:4]{index=4}
- posture enforcement using **GKE Security Posture Management**
- pre-merge Kubernetes manifest scanning + PR blocking for policy violations
- runtime threat visibility using **CrowdStrike Falcon XDR** on cluster nodes :contentReference[oaicite:5]{index=5}

Results delivered:
- **100% CIS Kubernetes Benchmark (v1.5.1)** compliance
- **93% OWASP Top 10 (2022)** compliance :contentReference[oaicite:6]{index=6}

---

### 5) Cloud Security Governance that Enables Speed (GCP-first)
Cloud security fails when it becomes documentation instead of enforcement.

I build governance as guardrails:
- IAM hardening + policy enforcement patterns
- secure defaults for infrastructure provisioning
- post-deployment drift detection and hygiene
- security visibility aligned to operations (not compliance theater)

I’ve implemented:
- CSPM posture monitoring using **Google Cloud SCC + Prisma Cloud**
- Terraform static analysis with automated gating using custom + managed policies
- enforcement rules to hard-fail PRs with critical IaC misconfigurations :contentReference[oaicite:7]{index=7}

---

### 6) VM / Endpoint Hardening at Scale (Golden Images)
I treat OS hardening as a product: versioned, repeatable, auditable.

I implemented a **Golden Image pipeline** to produce CIS-compliant images across:
- Ubuntu, Debian, CentOS, RHEL, and GCP base images
- automated hardening using OpenSCAP + Ansible
- publishing hardened images to GCP image registry
- verifying zero critical vulnerabilities via Rapid7 agents
- continuous threat monitoring using Cortex XDR :contentReference[oaicite:8]{index=8}

---

### 7) Enterprise Security Controls (Identity + Perimeter + Governance)
I’ve enforced enterprise-grade access controls including:
- Azure AD Conditional Access + Context-Aware policies
- corporate IP allowlisting, device compliance, and MFA enforcement
- isolating management APIs using GCP VPC Service Controls
- strengthening GitHub Enterprise security:
  - branch protections, CODEOWNERS, repo policy controls
  - SSO + 2FA enforcement
  - restricting outside collaborators + SSH key access
  - audit logging integration into Chronicle SecOps with detection rules :contentReference[oaicite:9]{index=9}

---

### 8) Application / API Security (Validation-first)
I don’t ship vulnerability reports. I validate impact and drive durable fixes.

I’ve performed security testing for:
- Web applications
- API services
- Mobile applications

With centralized remediation tracking via:
- Strobes + Jira workflows

I’ve also worked on runtime API monitoring and abuse detection using:
- SALT Security and AppSentinels
- API-level use cases for piracy prevention with content protection teams :contentReference[oaicite:10]{index=10}

---

## 🚀 Key Expertise
- Secure SDLC + Threat Modeling → enforceable controls
- CI/CD pipeline hardening and policy enforcement
- Container security + Kubernetes security + runtime detection
- IaC security + cloud governance + posture management
- Vulnerability management with risk-based prioritization (EPSS/QDS + exploitability) :contentReference[oaicite:11]{index=11}
- Security metrics and compliance enablement (ISO 27001:2022, CIS, OWASP, NIST) :contentReference[oaicite:12]{index=12}

---

## 🧰 Tools, Technologies & Platforms

### ☁️ Cloud & Infrastructure
![GCP](https://img.shields.io/badge/GCP-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-623CE4?style=flat-square&logo=terraform&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

### 🛠 CI/CD & Automation
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white)
![CircleCI](https://img.shields.io/badge/CircleCI-343434?style=flat-square&logo=circleci&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-000000?style=flat-square&logo=linux&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)

### 🔒 Security Engineering
![Prisma Cloud](https://img.shields.io/badge/-Prisma-005571?style=flat-square&logo=prisma&logoColor=white)
![Snyk](https://img.shields.io/badge/Snyk-4C4A73?style=flat-square&logo=snyk&logoColor=white)
![Burp Suite](https://img.shields.io/badge/Burp%20Suite%20Pro-FF6633?style=flat-square&logoColor=white)
![SonarQube](https://img.shields.io/badge/SonarQube-4E9BCD?style=flat-square&logo=sonarqube&logoColor=white)

---

## 🏅 Certifications
- ✅ Certified Kubernetes Security Specialist (**CKS**) — Sep 2025 :contentReference[oaicite:13]{index=13}
- ✅ Google Cloud **Professional Cloud Security Engineer** — May 2025 :contentReference[oaicite:14]{index=14}
- ✅ Google Cloud **Associate Cloud Engineer** — Apr 2025 :contentReference[oaicite:15]{index=15}
- ✅ Google Cloud **Professional Cloud Architect** — Apr 2025 :contentReference[oaicite:16]{index=16}
- ✅ Certified Kubernetes Administrator (**CKA**) — Jan 2025 :contentReference[oaicite:17]{index=17}
- ✅ HashiCorp Certified: Terraform Associate (**HCTA-003**) — Sep 2024 :contentReference[oaicite:18]{index=18}

---

## 🎓 Education
- **M.Tech (Software Systems), Cybersecurity (WILP)** — BITS Pilani (Pursuing: Jan 2026 – Dec 2028) :contentReference[oaicite:19]{index=19}
- **B.Tech (Electronics & Communication Engineering)** — VIT Chennai (Jun 2019 – May 2023) :contentReference[oaicite:20]{index=20}

---

## 📌 Featured Projects

### 🔐 Enterprise-Level DevSecOps CI/CD Pipeline (Nov 2024)
- Designed and implemented enterprise-grade CI/CD security pipeline on GCP
- Integrated SAST/SCA/container scanning + IaC security enforcement
- Enabled observability and security reporting for production readiness :contentReference[oaicite:21]{index=21}

### ☁️ Cloud-Native MERN Stack Deployment with End-to-End DevSecOps (Aug 2024)
- Deployed full-stack MERN app on AWS EKS using GitOps workflows
- Automated infra provisioning and built secure CI/CD pipelines
- Enabled monitoring with Prometheus + Grafana and operational controls :contentReference[oaicite:22]{index=22}

---

## 🏆 Achievements
- ⭐ Promoted to **IC-2** and awarded **Top Performance Rating (5-A)** (FY 2024–25) :contentReference[oaicite:23]{index=23}
- 🥇 **ZeeOlympics Best Performer Award** (FY 2023–24 and FY 2024–25) :contentReference[oaicite:24]{index=24}
- 🧠 Winner — **GitHub Tech After Dark** Quiz :contentReference[oaicite:25]{index=25}
- ☁️ Earned multiple **Google Cloud Skills Boost** achievements :contentReference[oaicite:26]{index=26}

---

## 📫 Connect with Me
- 📧 Email: **anshumaansingh10jan@gmail.com**
- 💼 LinkedIn: **linkedin.com/in/anshumaan-singh-6b51b5239**
- ✍️ Medium: **medium.com/@anshumaansingh10jan**
- 📂 GitHub: **github.com/anshumaan-10**

---

## 📄 Want to learn more?
[👉 View Resume (PDF)](https://drive.google.com/file/d/1FSYPYKnoltpLTqC7Zu6yV3Kdk5scXA3f/view?usp=sharing)  
📬 Or [email me](mailto:anshumaansingh10jan@gmail.com?subject=Requesting%20Resume)

![Profile views](https://komarev.com/ghpvc/?username=anshumaan-10&label=Profile%20views&color=0e75b6&style=flat)
