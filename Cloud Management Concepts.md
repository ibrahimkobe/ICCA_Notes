### 1. Shared Responsibility Model

- **Provider Responsibility:** Always responsible for physical security (facility), infrastructure security, platform security, virtualization, and the cloud management plane.
    
- **Customer Responsibility:** Always responsible for identity security (e.g., managing your Azure AD tenant), data security, application security, standards compliance, and managing access to the subscription.
    
- **Resiliency Responsibility:** While the provider offers a 99.99% SLA, the customer must actively build redundancy to support availability and build resiliency into their applications. Workloads still fail in the cloud; good software lifecycle management is crucial.
    

### 2. Control Plane vs. Data Plane

- **Control Plane (Management Plane):** This is "the cloud" itself. It is used to manage cloud assets and is accessed via:
    
    - REST APIs.
        
    - Web-based Consoles (Azure Portal, AWS Management Console, GCP Console).
        
    - Command Line Tools (AWS CLI, Azure CLI/PowerShell, Google Cloud SDK/Cloud Shell).
        
- **Data Plane:** This is your actual workload. For IaaS, this is the virtual machine OS and everything above it. For PaaS, it includes databases (like Azure Cosmos DB) and applications. You connect to the data plane using tools like SQL Server Management Studio or SSH/RDP.
    

### 3. Managing Cloud Assets

The lifecycle of managing cloud resources includes:

1. **Provisioning:** Creating the resources (e.g., choosing an AMI, instance type, storage, and tags in AWS).
    
2. **Configuring:** Setting up networking, firewalls, and subnets (e.g., Azure Cosmos DB network rules).
    
3. **Maintaining:** Maintaining code bases, data, and security.
    
4. **Monitoring:** Keeping an eye on logs, metrics, and alerts.
    
5. **Change Management:** Governance is critical because it is extremely easy to change things in the cloud. Use platform-specific and vendor-neutral tools.
    

### 4. Cost Management & Optimization

- **Billing Concepts:** Billing entity, billing cycle, billing rate, billing management, and marketplace billing.
    
- **Cost Monitoring:** Utilize budgets, alerts, native monitoring tools, and 3rd party tools.
    
- **Cost Optimization Tools:** * AWS: Cost anomaly detection.
    
    - Azure: Azure Advisors.
        
    - GCP: Google Recommender.
        
- **Cost Optimization Strategies:** Right-sizing, autoscaling, utilizing "Serverless" options, and purchasing long-term commitments.
    

### 5. Monitoring & Alerts

- **Platform Monitoring:** AWS CloudWatch, Azure Monitor, Google Cloud Monitoring.
    
- **Unified Monitoring (3rd Party):** Nagios, Splunk, PRTG.
    
- **Proactive Resource Management:** Utilize cloud automation and alerting (e.g., setting up Auto Scaling groups and Launch Templates).
    

### 6. Identity and Access Management (IAM)

- **Identity Tools:** * _AWS:_ IAM Users, IAM Roles, IAM Policies.
    
    - _Azure:_ Azure AD Users, Azure AD Service Principals, Azure AD Managed Identities, Roles.
        
    - _GCP:_ Google Account, Service Account, Role, Policy.
        
- **IAM Best Practices:** * Always apply the principle of least privilege.
    
    - Minimize "root" user access.
        
    - Organize users into groups.
        
    - Use dynamic access policies/management when possible.
        
    - Audit resource access and unused accounts.
        
    - Separate control plane and data plane access.