---
config:
  layout: dagre
---
flowchart LR
 subgraph L1["Engineering and Source Governance"]
        Dev["Developer Workstation"]
        PreCommit["Pre-commit Checks"]
        Signed["Signed Commits"]
        PR["Pull Request"]
        Review["CODEOWNERS Review"]
        Branch["Branch Protection"]
        Checks["Required Status Checks"]
        Repo["Main Branch"]
  end
 subgraph L2["Identity and Access Plane"]
        OIDC["OIDC Federation"]
        STS["Token Service"]
        ShortCreds["Short Lived Credentials"]
        IAM["IAM Boundaries"]
  end
 subgraph L3["CI Boundary and Secure SDLC Verification"]
        CI["CI Orchestrator"]
        Runner["Ephemeral Runner"]
        Build["Build and Package"]
        Tests["Unit and Integration Tests"]
        SAST["SAST"]
        SCA["SCA"]
        SecretsScan["Secrets Scan"]
        IaC["IaC Scan"]
        DAST["DAST Validation"]
        Quality["Quality Gate"]
  end
 subgraph L4["Supply Chain Integrity and Evidence"]
        ImgBuild["Container Image Build"]
        ImgScan["Image Vulnerability Scan"]
        SBOM["SBOM Generation"]
        Provenance["Provenance Metadata"]
        Sign["Artifact Signing"]
        Attest["Attestation Bundle"]
  end
 subgraph L5["Risk Engine and Release Governance"]
        Risk["Risk Scoring Engine"]
        CVSS["CVSS Severity"]
        EPSS["EPSS Probability"]
        Exploit["Exploit Maturity"]
        PolicyGate["Risk Policy Gate"]
        Registry["Artifact Registry"]
        Immutable["Immutable Tags"]
        Promote["Promotion Workflow"]
        Approvals["Approval Gate"]
  end
 subgraph L6["Environment Separation"]
        DevEnv["Dev"]
        UATEnv["UAT"]
        ProdEnv["Prod"]
  end
 subgraph L7["Kubernetes Control Plane and Policy Enforcement"]
        Admission["Admission Controller"]
        PolicyEngine["Policy Engine"]
        RBAC["RBAC and Namespace Controls"]
        Ingress["Ingress Boundary"]
        EastWest["East West Segmentation"]
        Egress["Egress Control"]
        Mesh["Service Mesh"]
        mTLS["mTLS Identity"]
  end
 subgraph L8["Runtime Plane and Data Plane"]
        Deploy["Deployment Controller"]
        Pods["Workloads and Pods"]
        SecCtx["Security Context Hardening"]
        RuntimeDet["Runtime Detection"]
        Drift["Drift Detection"]
        SecretsStore["Secrets Manager"]
        KMS["KMS Encryption"]
        DB["Datastores"]
        PII["PII Boundary"]
  end
 subgraph L9["Observability and Security Operations"]
        Audit["Audit Logs"]
        Metrics["Metrics"]
        Traces["Traces"]
        SIEM["SIEM"]
        Detect["Detections"]
        IR["Incident Response"]
        Case["Case Management"]
  end
 subgraph KC["Kill Chain Mapping and Kill Switch Controls"]
        Recon["Recon"]
        Initial["Initial Access"]
        PrivEsc["Privilege Escalation"]
        Lateral["Lateral Movement"]
        Exfil["Exfiltration"]
        Impact["Impact"]
  end
    Dev --> PreCommit
    PreCommit --> Signed
    Signed --> PR
    PR --> Review
    Review --> Branch
    Branch --> Checks
    Checks --> Repo
    Repo --> OIDC & CI
    OIDC --> STS
    STS --> ShortCreds
    ShortCreds --> IAM
    CI --> Runner
    Runner --> Build
    Build --> Tests & SAST & SCA & SecretsScan & IaC
    Tests --> Quality
    SAST --> Quality
    SCA --> Quality
    SecretsScan --> Quality
    IaC --> Quality
    Quality --> DAST
    DAST --> ImgBuild
    ImgBuild --> ImgScan
    ImgScan --> SBOM
    SBOM --> Provenance
    Provenance --> Attest
    Sign --> Attest
    Attest --> Risk
    Risk --> CVSS & EPSS & Exploit
    CVSS --> PolicyGate
    EPSS --> PolicyGate
    Exploit --> PolicyGate
    PolicyGate --> Registry
    Registry --> Immutable
    Immutable --> Promote
    Promote --> Approvals
    Approvals --> DevEnv
    DevEnv --> UATEnv
    UATEnv --> ProdEnv
    ProdEnv --> Admission
    Admission --> PolicyEngine
    PolicyEngine --> RBAC
    PolicyEngine -- Block --> CI
    RBAC --> Ingress
    Ingress --> EastWest
    EastWest --> Egress & Mesh
    Mesh --> mTLS
    mTLS --> Deploy
    Deploy --> Pods
    Pods --> SecCtx & RuntimeDet & Drift & SecretsStore & DB & Metrics & Traces
    SecretsStore --> KMS
    DB --> PII
    RuntimeDet --> Audit
    Audit --> SIEM
    Drift --> Audit
    Metrics --> SIEM
    Traces --> SIEM
    SIEM --> Detect
    Detect --> IR
    IR --> Case
    Recon --> Initial
    Initial --> PrivEsc
    PrivEsc --> Lateral
    Lateral --> Exfil
    Exfil --> Impact
    WAF["WAF"] -. blocks .-> Recon
    Rate["Rate"] -. throttles .-> Recon
    SecretsScan -. prevents .-> Initial
    SAST -. reduces .-> Initial
    Admission -. denies .-> Initial
    RBAC -. limits .-> PrivEsc
    SecCtx -. prevents .-> PrivEsc
    EastWest -. blocks .-> Lateral
    Mesh -. enforces .-> Lateral
    mTLS -. denies .-> Lateral
    Egress -. restricts .-> Exfil
    PII -. reduces .-> Exfil
    SIEM -. detects .-> Impact
    IR -. contains .-> Impact
