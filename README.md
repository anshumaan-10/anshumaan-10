<h1 align="center">Hi 👋, I'm Anshumaan Singh</h1>
<h3 align="center">Security Systems Engineer | DevSecOps | Cloud & Application Security</h3>

<p align="center">
  <a href="mailto:anshumaansingh10jan@gmail.com">
    <img src="https://img.shields.io/badge/Email-anshumaansingh10jan%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
  <a href="https://www.linkedin.com/in/anshumaan-singh-6b51b5239/">
    <img src="https://img.shields.io/badge/LinkedIn-Anshumaan%20Singh-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="https://github.com/anshumaan-10">
    <img src="https://img.shields.io/badge/GitHub-anshumaan--10-181717?style=for-the-badge&logo=github&logoColor=white" />
  </a>
  <a href="https://medium.com/@anshumaansingh10jan">
    <img src="https://img.shields.io/badge/Medium-%40anshumaansingh10jan-000000?style=for-the-badge&logo=medium&logoColor=white" />
  </a>
</p>

<img align="right" alt="Security Engineering" width="420" src="https://raw.githubusercontent.com/devSouvik/devSouvik/master/gif3.gif">

---

## 🔥 About Me (Security Systems Engineering)

I engineer security the same way high-scale teams engineer reliability: as a **system property**—designed, enforced, and continuously verified.

I work across the SDLC, but my real domain is **security system design**: defining trust boundaries, constraining blast radius, enforcing secure defaults, and ensuring production behavior is predictable even under adversarial pressure.

I don’t treat security as “findings.”  
I treat security as **invariants**: rules that must remain true regardless of code changes, deployments, or operational stress.

📍 Bengaluru, India  
🏢 Information Security Analyst (IC-2) @ **ZEE Entertainment Enterprises Ltd**  
🧩 Secured **350+ microservices** from development → production using centralized DevSecOps security architecture

---

## 🧠 Security System Design (What I Build)

### 1) Trust Architecture & Secure Design Reviews
I design secure systems by explicitly defining:
- principals and identities (human, service, workload identity)
- trust zones and cross-boundary flows
- authorization enforcement points and decision ownership
- failure modes and safe degradation paths
- attacker paths (abuse routes, escalation edges, bypass opportunities)

I convert these into engineering constraints:
- deny-by-default access models
- scoped permissions and least privilege everywhere
- isolation boundaries to limit lateral movement
- secure-by-default interfaces and hardened baselines

---

### 2) CI/CD as a Security Control Plane (Enterprise-Grade DevSecOps)
I treat CI/CD as a security boundary that must guarantee:
- only reviewed changes produce deployable artifacts
- policy violations fail early (pre-merge + pre-deploy)
- artifacts remain traceable to change + approval
- promotions are controlled, non-bypassable, and auditable

I’ve built centralized DevSecOps pipelines at scale integrating:
- SAST / SCA / Secret scanning
- container image scanning + SBOM generation
- DAST validation workflows
- policy-as-code enforcement with hard-fail gates
- build-time binary authorization controls

---

### 3) Supply Chain Hardening & Artifact Integrity
Most breaches start with **tampering**, not exploitation.

I harden delivery pipelines by enforcing:
- controlled artifact creation and promotion flows
- strict versioning and release immutability principles
- provenance-style traceability (what was built, from where, by whom)
- verification gates so “passed” actually means “safe to ship”

---

### 4) Kubernetes Security + Runtime Threat Engineering
I secure Kubernetes by designing for runtime reality:
- workload drift
- permission sprawl
- network boundary erosion
- “temporary exceptions” becoming permanent exposure

What I enforce:
- admission control guardrails using policy engines
- CIS benchmark alignment and cluster hardening
- runtime detection that maps to response actions (not noise)
- continuous posture monitoring for misconfigurations + zero-day risk signals

---

### 5) Application & API Security (Validation-First)
I don’t ship vulnerability reports. I validate exploitability and drive durable fixes.

I focus heavily on:
- authorization failures (IDOR / broken access control)
- token handling and session trust boundaries
- API abuse patterns (enumeration, replay, privilege jumps)
- insecure assumptions between microservices and identity boundaries

---

### 6) Cloud Security Governance (GCP-first, Enterprise Controls)
I implement governance as guardrails:
- IAM hardening and scoped access patterns
- secure defaults and policy enforcement
- drift detection + post-deployment hygiene
- security posture visibility aligned with operations

---

## 🏢 Experience (Impact)

### ZEE Entertainment Enterprises Ltd — Bengaluru, IN  
**Information Security Analyst (IC-2)** | Jun 2023 – Present

- Built an end-to-end centralized DevSecOps pipeline securing **350+ microservices**
- Implemented IaC gating + misconfiguration enforcement with hard-fail PR blockers
- Enforced Kubernetes compliance via policy-as-code + runtime threat detection
- Achieved **100% CIS Kubernetes Benchmark (v1.5.1)** and **93% OWASP Top 10 2022** compliance
- Implemented Golden Image pipeline for CIS-compliant Linux images + automated OS hardening
- Strengthened GitHub Enterprise security with org-level controls, audit logging, and SIEM detections
- Enforced perimeter security using Conditional Access + IP restrictions + service controls

---

## 🧰 Tech Stack

### ☁️ Cloud Platforms
<p>
  <img src="https://img.shields.io/badge/Google%20Cloud-4285F4?style=flat-square&logo=googlecloud&logoColor=white" />
  <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white" />
  <img src="https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white" />
</p>

### ☸️ Containers & Orchestration
<p>
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white" />
  <img src="https://img.shields.io/badge/GKE-4285F4?style=flat-square&logo=googlecloud&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white" />
</p>

### 🏗 Infrastructure as Code (IaC) + Policy-as-Code
<p>
  <img src="https://img.shields.io/badge/Terraform-623CE4?style=flat-square&logo=terraform&logoColor=white" />
  <img src="https://img.shields.io/badge/Ansible-EE0000?style=flat-square&logo=ansible&logoColor=white" />
  <img src="https://img.shields.io/badge/OPA%20Gatekeeper-7A1FA2?style=flat-square&logoColor=white" />
</p>

### 🔁 CI/CD & Build Systems
<p>
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" />
  <img src="https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white" />
  <img src="https://img.shields.io/badge/CircleCI-343434?style=flat-square&logo=circleci&logoColor=white" />
  <img src="https://img.shields.io/badge/GitLab-FC6D26?style=flat-square&logo=gitlab&logoColor=white" />
</p>

### 🔍 Secure SDLC (SAST / SCA / Secrets / Code Security)
<p>
  <img src="https://img.shields.io/badge/GitHub%20Advanced%20Security-181717?style=flat-square&logo=github&logoColor=white" />
  <img src="https://img.shields.io/badge/CodeQL-181717?style=flat-square&logo=github&logoColor=white" />
  <img src="https://img.shields.io/badge/Semgrep-3C3C3C?style=flat-square&logo=semgrep&logoColor=white" />
  <img src="https://img.shields.io/badge/Snyk-4C4A73?style=flat-square&logo=snyk&logoColor=white" />
  <img src="https://img.shields.io/badge/SonarQube-4E9BCD?style=flat-square&logo=sonarqube&logoColor=white" />
  <img src="https://img.shields.io/badge/TruffleHog-000000?style=flat-square&logoColor=white" />
</p>

### 🧪 DAST / Web / API / Mobile Security
<p>
  <img src="https://img.shields.io/badge/Burp%20Suite%20Pro-FF6633?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/OWASP%20ZAP-000000?style=flat-square&logo=owasp&logoColor=white" />
  <img src="https://img.shields.io/badge/MobSF-2E7D32?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white" />
</p>

### 🐳 Container / Image Security + Runtime Protection
<p>
  <img src="https://img.shields.io/badge/Prisma%20Cloud-005571?style=flat-square&logo=prisma&logoColor=white" />
  <img src="https://img.shields.io/badge/Trivy-4A90E2?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/Anchore-2C3E50?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/Sysdig-1A73E8?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/Aqua%20Security-00BFA5?style=flat-square&logoColor=white" />
</p>

### 🛡 Vulnerability Management + Threat Intelligence + ASM
<p>
  <img src="https://img.shields.io/badge/Rapid7-FE5000?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/Qualys-ED2E26?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/Mandiant-FF0000?style=flat-square&logoColor=white" />
  <img src="https://img.shields.io/badge/Jira-0052CC?style=flat-square&logo=jira&logoColor=white" />
</p>

### 📊 Logging / SIEM / Monitoring
<p>
  <img src="https://img.shields.io/badge/Google%20Chronicle-4285F4?style=flat-square&logo=googlecloud&logoColor=white" />
  <img src="https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white" />
  <img src="https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white" />
</p>

### 💻 OS / Scripting / Automation
<p>
  <img src="https://img.shields.io/badge/Linux-000000?style=flat-square&logo=linux&logoColor=white" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white" />
</p>

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

- CKS — Sep 2025  
- Google Professional Cloud Security Engineer — May 2025  
- Google Associate Cloud Engineer — Apr 2025  
- Google Professional Cloud Architect — Apr 2025  
- CKA — Jan 2025  
- Terraform Associate (HCTA-003) — Sep 2024  

---

## 🎓 Education
- **BITS Pilani (WILP)** — M.Tech Software Systems (Cybersecurity) *(Jan 2026 – Dec 2028, Pursuing)*  
- **VIT Chennai** — B.Tech Electronics & Communication Engineering *(Jun 2019 – May 2023)*  

---

## 📌 Featured Projects

### 🔐 Enterprise-Level DevSecOps CI/CD Pipeline (Nov 2024)
- Designed and implemented enterprise-grade CI/CD security pipeline on GCP
- Integrated SAST/SCA/container security + IaC enforcement
- Enabled observability and production-grade audit readiness

### ☁️ Cloud-Native MERN Stack Deployment with End-to-End DevSecOps (Aug 2024)
- Deployed full-stack MERN app on AWS EKS with GitOps workflows
- Automated infra provisioning and secure CI/CD pipelines
- Implemented monitoring with Prometheus + Grafana


## 🏗️ Reference Architecture: Secure-by-Default Delivery (End-to-End)

<img width="8192" height="1335" alt="image" src="https://github.com/user-attachments/assets/13201c3b-def7-4b5a-8283-c718708a7826" />


## 🏆 Achievements
- ⭐ Promoted to **IC-2** + Top Performance Rating **5-A** (FY 2024–25)
- 🥇 **ZeeOlympics Best Performer Award** (FY 2023–24 and FY 2024–25)
- 🧠 Winner — **GitHub Tech After Dark Quiz**
- ☁️ Multiple **Google Cloud Skills Boost** achievements

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
