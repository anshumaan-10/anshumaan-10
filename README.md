<h1 align="center">Hi 👋, I'm Anshumaan Singh</h1>
<h3 align="center">Security Systems Engineer | DevSecOps | Cloud & Application Security</h3>

<p align="center">
  <a href="mailto:anshumaansingh10jan@gmail.com"><img src="https://img.shields.io/badge/Email-anshumaansingh10jan%40gmail.com-red?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/anshumaan-singh-6b51b5239/"><img src="https://img.shields.io/badge/LinkedIn-Anshumaan%20Singh-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="https://github.com/anshumaan-10"><img src="https://img.shields.io/badge/GitHub-anshumaan--10-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
  <a href="https://medium.com/@anshumaansingh10jan"><img src="https://img.shields.io/badge/Medium-%40anshumaansingh10jan-000000?style=for-the-badge&logo=medium&logoColor=white" /></a>
</p>

<img align="right" alt="Security Engineering" width="420" src="https://raw.githubusercontent.com/devSouvik/devSouvik/master/gif3.gif">

---

## 🔐 About Me (Security Systems Engineering Mindset)

I engineer security the same way high-scale teams engineer reliability: as a **system property**—designed, enforced, and continuously verified.

I work across the SDLC, but my real domain is **security system design**: defining trust boundaries, constraining blast radius, enforcing secure defaults, and ensuring production behavior is predictable even under adversarial pressure.

I don’t treat security as “findings.”  
I treat security as **invariants**: rules that must remain true regardless of code changes, deployments, or operational stress.

### 🧭 My operating principles
- **Security is architecture** → not a toolchain
- **Controls must be enforceable** → not advisory
- **Verification > trust** → pipelines prove safety
- **Runtime reality matters** → production is the final test
- **Risk must be measurable** → decisions require signals

📍 Bengaluru, India  
🏢 Information Security Analyst (IC-2) @ **ZEE Entertainment Enterprises Ltd**  
🧩 Built and enforced centralized security controls for **350+ microservices** (Dev → Prod) :contentReference[oaicite:1]{index=1}

---

## 🧠 What I Build (Security by Design, Not by Checklist)

### 1) Trust Architecture & Secure System Design
I design systems by explicitly defining:
- **Principals & identities** (human, service, workload identity)
- **Trust zones** and cross-boundary flows
- **Authorization enforcement points** and decision ownership
- **Failure modes** (what breaks first, what becomes exploitable)
- **Attacker paths** (abuse routes, escalation edges, bypass attempts)

I translate these into engineering constraints:
- deny-by-default access models
- least privilege at identity + runtime layers
- isolation boundaries to limit lateral movement
- secure-by-default interfaces and hardened baselines

---

### 2) CI/CD as a Security Control Plane (Not a Build Script)
I treat CI/CD as a **security boundary**. A production pipeline must guarantee:
- only reviewed changes produce deployable artifacts
- only trusted identities can publish artifacts
- artifacts are traceable to change + approval
- promotions are controlled and non-bypassable

I’ve designed an enterprise-grade DevSecOps pipeline for **350+ microservices** with:
- SAST / SCA / Secret Scanning
- Container Image Scanning + SBOM generation
- DAST integration for runtime validation
- Binary authorization at build-time
- Policy-as-Code gates that break builds based on risk thresholds :contentReference[oaicite:2]{index=2}

---

### 3) Supply Chain Hardening & Artifact Integrity
Most modern breaches begin with **tampering**, not exploitation.

I harden software delivery by enforcing:
- controlled artifact creation + promotion flows
- strict versioning and release immutability
- provenance-style traceability (what, where, who, when)
- consistent verification gates so “passed” means “safe to ship”

---

### 4) Kubernetes & Runtime Security as Engineering Constraints
I secure Kubernetes by designing for runtime reality:
- workloads drift
- permissions sprawl
- network boundaries degrade
- exceptions become permanent exposure

What I implement:
- admission control guardrails with **OPA Gatekeeper** to block non-compliant workloads :contentReference[oaicite:3]{index=3}
- Kubernetes Threat Detection (KTD) using **Falco**, integrated with **Google Cloud SCC** :contentReference[oaicite:4]{index=4}
- GKE Security Posture Management for misconfig and threat visibility
- pre-merge manifest scanning + PR policy enforcement
- runtime threat visibility using **CrowdStrike Falcon XDR** on cluster nodes :contentReference[oaicite:5]{index=5}

Results delivered:
- **100% CIS Kubernetes Benchmark (v1.5.1)** compliance
- **93% OWASP Top 10 (2022)** compliance :contentReference[oaicite:6]{index=6}

---

### 5) Application & API Security (Validation-First)
I don’t ship vulnerability reports. I validate exploitability and drive durable fixes.

I focus heavily on:
- authorization failures and IDOR-class issues
- token handling and session trust boundaries
- API abuse patterns (enumeration, replay, privilege jumps)
- insecure assumptions between microservices and identity boundaries

I’ve delivered AppSec outcomes using:
- centralized reporting + remediation tracking (Strobes + Jira)
- runtime API monitoring and abuse detection (SALT Security + AppSentinels)
- API-level use cases for piracy prevention with content protection teams :contentReference[oaicite:7]{index=7}

---

### 6) Cloud Governance that Enables Speed (GCP-first)
Cloud security fails when it becomes documentation instead of enforcement.

I implement governance as guardrails:
- IAM hardening + scoped access patterns
- policy enforcement for secure defaults
- drift detection + post-deployment hygiene
- security visibility aligned with response workflows

I’ve implemented:
- CSPM posture monitoring with **Google Cloud SCC + Prisma Cloud** :contentReference[oaicite:8]{index=8}
- IaC gating using custom Terraform Vet policies + automated enforcement :contentReference[oaicite:9]{index=9}

---

### 7) Golden Images + OS Hardening (Repeatable & Auditable)
I treat OS hardening as a product: versioned, repeatable, and measurable.

I built a Golden Image pipeline that:
- produces CIS-compliant images (Ubuntu/Debian/CentOS/RHEL/GCP)
- automates hardening using OpenSCAP + Ansible
- publishes hardened images to GCP image registry
- validates posture using Rapid7 agents
- enables continuous monitoring using Cortex XDR :contentReference[oaicite:10]{index=10}

---

## 🏢 Experience (Impact-Driven)

### ZEE Entertainment Enterprises Ltd — Bengaluru, IN  
**Information Security Analyst (IC-2)** | Jun 2023 – Present :contentReference[oaicite:11]{index=11}

Key engineering outcomes:
- Built a centralized DevSecOps pipeline securing **350+ microservices**
- Implemented pre-merge gating for IaC misconfigurations using policy enforcement
- Achieved **100% CIS Kubernetes Benchmark** compliance + **93% OWASP Top 10 2022** alignment
- Strengthened GitHub Enterprise security with SSO/2FA, audit logging, and Chronicle SIEM detections
- Implemented enterprise perimeter controls using Conditional Access + IP restrictions + VPC Service Controls
- Delivered continuous threat visibility using Falcon XDR and Cortex XDR

---

## 🎓 Education
- **BITS Pilani (WILP)** — M.Tech Software Systems (Cybersecurity) *(Jan 2026 – Dec 2028, Pursuing)* :contentReference[oaicite:12]{index=12}  
- **VIT Chennai** — B.Tech Electronics & Communication Engineering *(Jun 2019 – May 2023)* :contentReference[oaicite:13]{index=13}  

---

## 🏅 Certifications (Verified)
<p>
  <img src="https://img.shields.io/badge/CKS-Certified%20Kubernetes%20Security%20Specialist-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" />
  <img src="https://img.shields.io/badge/CKA-Certified%20Kubernetes%20Administrator-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" />
  <img src="https://img.shields.io/badge/GCP-Professional%20Cloud%20Security%20Engineer-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white" />
  <img src="https://img.shields.io/badge/GCP-Professional%20Cloud%20Architect-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white" />
  <img src="https://img.shields.io/badge/GCP-Associate%20Cloud%20Engineer-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white" />
  <img src="https://img.shields.io/badge/Terraform-HashiCorp%20Certified-623CE4?style=for-the-badge&logo=terraform&logoColor=white" />
</p>

Issued:
- CKS — Sep 2025 :contentReference[oaicite:14]{index=14}  
- Google Professional Cloud Security Engineer — May 2025 :contentReference[oaicite:15]{index=15}  
- Google Associate Cloud Engineer — Apr 2025 :contentReference[oaicite:16]{index=16}  
- Google Professional Cloud Architect — Apr 2025 :contentReference[oaicite:17]{index=17}  
- CKA — Jan 2025 :contentReference[oaicite:18]{index=18}  
- Terraform Associate (HCTA-003) — Sep 2024 :contentReference[oaicite:19]{index=19}  

---

## 🧰 Tech Stack (FAANG-style Categories)

### ☁️ Cloud, Infra & Platform
<p>
  <img src="https://img.shields.io/badge/Google%20Cloud-4285F4?style=flat-square&logo=googlecloud&logoColor=white" />
  <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white" />
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Terraform-623CE4?style=flat-square&logo=terraform&logoColor=white" />
  <img src="https://img.shields.io/badge/Ansible-EE0000?style=flat-square&logo=ansible&logoColor=white" />
</p>

### 🔐 DevSecOps / Security Engineering
<p>
  <img src="https://img.shields.io/badge/GitHub%20Advanced%20Security-181717?style=flat-square&logo=github&logoColor=white" />
  <img src="https://img.shields.io/badge/Prisma%20Cloud-005571?style=flat-square&logo=prisma&logoColor=white" />
  <img src="https://img.shields.io/badge/Snyk-4C4A73?style=flat-square&logo=snyk&logoColor=white" />
  <img src="https://img.shields.io/badge/SonarQube-4E9BCD?style=flat-square&logo=sonarqube&logoColor=white" />
  <img src="https://img.shields.io/badge/Qualys-ED2E26?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/Rapid7-FE5000?style=flat-square&logoColor=white" />
</p>

### 🛠 CI/CD & Automation
<p>
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" />
  <img src="https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white" />
  <img src="https://img.shields.io/badge/CircleCI-343434?style=flat-square&logo=circleci&logoColor=white" />
  <img src="https://img.shields.io/badge/Linux-000000?style=flat-square&logo=linux&logoColor=white" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white" />
</p>

### 📊 Observability / Detection
<p>
  <img src="https://img.shields.io/badge/Google%20Chronicle-4285F4?style=flat-square&logo=googlecloud&logoColor=white" />
  <img src="https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white" />
  <img src="https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white" />
</p>

---

## 📌 Projects (Security Engineering)

### 🔐 Enterprise-Level DevSecOps CI/CD Pipeline (Nov 2024) :contentReference[oaicite:20]{index=20}
- Designed enterprise-grade CI/CD pipeline using GitHub Actions on GCP
- Integrated SAST/SCA/container security + IaC enforcement
- Enabled observability and production-grade audit readiness

### ☁️ Cloud-Native MERN Stack Deployment with End-to-End DevSecOps (Aug 2024) :contentReference[oaicite:21]{index=21}
- Deployed full-stack MERN app on AWS EKS with GitOps workflows
- Automated infra provisioning and CI/CD pipelines
- Implemented monitoring and operational readiness

---

## 🏆 Achievements
- ⭐ Promoted to **IC-2** + Top Performance Rating **5-A** (FY 2024–25) :contentReference[oaicite:22]{index=22}
- 🥇 **ZeeOlympics Best Performer Award** (FY 2023–24 and FY 2024–25) :contentReference[oaicite:23]{index=23}
- 🧠 Winner — **GitHub Tech After Dark Quiz** :contentReference[oaicite:24]{index=24}
- ☁️ Multiple **Google Cloud Skills Boost** achievements :contentReference[oaicite:25]{index=25}

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
