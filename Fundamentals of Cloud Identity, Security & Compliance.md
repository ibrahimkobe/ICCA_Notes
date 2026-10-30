### 1. Defense in Depth

Security must be layered. The typical layers of defense include (from outer to inner): DDoS protection -> Public firewall -> nACL -> Local Network Monitoring -> Operating System Hardening -> Authentication & Authorization -> Patching -> Auditing -> Data access control -> Encryption at rest & Encryption in transit.

### 2. Common Cloud Attacks

- **Attack Targets:** Identities (SaaS, Platform, Data plane), Data, and Services.
    
- **Attack Methods:** * Misconfiguration (Intentional or inadvertent, allowing unauthorized third-party access to databases, public APIs, or services).
    
    - Account Hijacking.
        
    - Service Hijacking.
        
    - Malware.
        

### 3. Identity Protection & Compromise Response

- **Account Vulnerabilities:** Weak passwords, leaked credentials, general threat intelligence.
    
- **Login Vulnerabilities:** IP Address and location anomalies, password spraying, brute force attacks.
    
- **Identity Protection Services:** * AWS: CloudTrail, Trusted Advisor.
    
    - Azure: Identity Protection, Azure AD Logs.
        
    - GCP: Advanced Protection Program, G-suite alert center, Titan security keys.
        
- **The Five R's of Incident Response (If an identity is compromised):**
    
    1. **Revoke:** Revoke permissions, session tokens, API keys, resource access keys, and any form of trusted identity. Isolate the identity from data services and resources.
        
    2. **Reset**.
        
    3. **Review:** Review with IT and business personnel to determine the impact.
        
    4. **Remediate:** Conduct remedial training, improve processes, define a forward plan of action, and report as necessary.
        
    5. **Return:** Return to operating state and monitor.
        

### 4. Data Protection

- **Types of Cloud Data:** * _Files:_ Blobs, Buckets, File services.
    
    - _Relational/Non-relational:_ Managed, Proprietary, IaaS hosted.
        
    - _Big data:_ Semi-structured.
        
    - _Sensitive:_ Keys, Certificates, Audit.
        
- **Protecting Data at Rest:** Use Network Controls, Permissions, Backup, Replication, Encryption, and Hardware Security Modules (HSMs).
    
- **Protecting Data in Transit:** Always encrypt your data in transit.
    
- **Best Practices:** Limit access across resource, data, and network boundaries. Always encrypt (at rest, in transit, end-to-end). Protect from failure using replication and backup. Always audit.
    

### 5. Network Protection

- **Provider Responsibility:** Protects the physical facility, physical infrastructure, and virtualized infrastructure (providing baseline DDoS and general threat protection).
    
- **Tenant Responsibility (Cloud Network Controls):**
    
    - _AWS:_ Network ACL, Security Group. Private Link.
        
    - _Azure:_ Network Security Group (NSG). Private Endpoint.
        
    - _GCP:_ Firewall rule. VPC Service Control.
        
- **Network Security Services:** * _AWS:_ AWS Shield, AWS WAF, AWS GuardDuty.
    
    - _Azure:_ Azure Firewall, Application Gateway, Azure FrontDoor.
        
    - _GCP:_ Google Cloud Armor.
        
- **Best Practices:** Leverage provider tools, limit the public attack surface, monitor traffic, alert on atypical usage patterns, and have a playbook ready.
    

### 6. Compute Protection

- **Infrastructure Compute Protection:** Requires patch management (OS patching can be automated in AWS/Azure; you must patch the services like web/DB servers), OS hardening, monitoring, resource protection, attack surface minimization, and utilizing multiple instances.
    
- **Platform Compute Protection:** PaaS compute is always patched by the provider.
    
- **Confidential Compute:** Uses a **Trusted Execution Environment (Enclave)**. This protects against unauthorized data access and code corruption while the data is actually _in use_. Note: This is only available on specific compute instance sizes.
    

### 7. Regulatory Compliance

- **Cloud Compliance Tools:** * _Tools:_ Amazon GuardDuty, Azure Compliance Manager, GCP Security Command Center.
    
    - _Documentation/Reporting:_ Amazon Artifact, Microsoft Trust Center, GCP Compliance Resource Center.
        
- **Tenant Responsibilities:** Understand your regulatory requirements, document the provider's compliance with those regulations, implement your own security responsibilities, and use provider tools to achieve, maintain, and document full compliance.
    
- **Common Protected Data Types:** * _Personal:_ PII, Health Care (PHI).
    
    - _Financial:_ PCI-DSS, Sarbanes Oxley.
        
    - _Regional/Legal:_ GDPR-EU, California privacy laws, US Federal Protected Data (research, technology, weapons).
        
    - _Business:_ Intellectual Property, Legal Considerations, Business Reputation.