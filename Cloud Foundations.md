### 1. What is the Cloud?

**On-Premises Architecture:**

- In a traditional on-premises model, your organization must manage **everything**: Power, Network, Racks, Storage, Physical Facility, Physical Infrastructure, Virtualization, Virtual Machines, Services, and the Workload.
    
- This also means your organization incurs the costs of Platform Maintenance, Licensing, Space, Physical Security, and Personnel.
    

**Cloud Architecture:**

- Cloud computing shifts the responsibility of the bottom layers to the cloud provider.
    
- The cloud provider assumes responsibility for the **Physical Facility**, **Physical Infrastructure**, **Virtualization**, and the **Management Plane (Control Plane)**.
    

### 2. Types of Cloud Services

Cloud services are categorized by the level of control you retain vs. the ease of administration provided.

- **Infrastructure as a Service (IaaS):** Offers the highest control, but requires the most administration. You manage the Virtual Machine (OS), Services, and Workload.
    
    - _Examples:_ Cloud Compute (AWS EC2, Azure VMs, Google Compute Engine) and Cloud Storage (AWS S3, Azure Storage Accounts, Google Cloud Storage).
        
- **Platform as a Service (PaaS):** Offers a balance. The provider manages the underlying OS and infrastructure; you manage the Workload.
    
    - _Application Hosting Examples:_ AWS (Lightsail, Lambda, Beanstalk, Elastic Container Service), Azure (Web Apps, Function Apps, Logic Apps, Container Registry), Google Cloud (App Engine, Cloud Functions, Cloud Run).
        
    - _Data Hosting Examples:_ AWS (RDS, DynamoDB, Redshift), Azure (SQL database, Cosmos DB, Synapse), Google Cloud (Cloud SQL, Firestore, BigQuery).
        
- **Software as a Service (SaaS):** Offers the lowest control, but the highest ease of administration. The provider manages the full stack, you only manage customizations and your data.
    
    - _Examples:_ SalesForce (the leader in CRM), Microsoft 365, G Suite, Slack, Zoom, Microsoft Teams.
        

### 3. The Cloud Market & Providers

**2019 Market Share:**

- **AWS:** 45%
    
- **Microsoft Azure:** 20%
    
- **Alibaba:** 9%
    
- **Google Cloud Platform (GCP):** 5%
    
- **Tencent:** 3%
    
- **Others (IBM, Oracle, Digital Ocean, Private Clouds):** 18%
    
- _Note:_ The estimated market size was $216B in 2019, scaling to $823B by 2025.
    

**Major Provider Profiles:**

- **AWS:** Officially launched in 2006. Boasts over 1,000,000 active users, 18 global regions, over 190 countries, and over 175 products and services.
    
- **Azure:** Publicly available in 2010. Boasts over 300k customers, over 169 services, 57 regions, and 31 geographies.
    
- **GCP:** Cloud Storage launched in 2010. Offers over 90 services.
    

### 4. Cloud Economics

**CapEx vs. OpEx:**

- **On-Premises (Capital Expense - CapEx):** Requires purchasing equipment and licensing up-front, depreciating/replacing equipment, and renewing licenses.
    
- **Cloud (Operational Expense - OpEx):** Capacity expansion is an operational expense. You are billed monthly for exactly what is used, with no equipment purchase required. If you need a capacity reduction, you instantly reduce your monthly cost (unlike on-prem where you have to try and sell excess equipment).
    

**Pricing Models:**

- **Capacity-based:** Spending is based on allocated resources (e.g., Virtual Machines, on-premises resources).
    
- **Consumption-based:** Spending is based strictly on what is used (e.g., Serverless Functions/Lambda, Storage, Services). Beware of data transfer and transactional costs!
    

**Functional Advantages:**

- Provision environments in minutes instead of days/weeks/months.
    
- No capital equipment purchases, streamlined provisioning, built-in access/allocation management, and reduced administrative overhead.
    
- _Reasons not to move to the cloud:_ Existing investments, ongoing operational expenses, data fencing requirements, and regulatory compliance hurdles.
    

### 5. Cloud Scalability, Availability & SLAs

- **Scalability:** Allows you to instantly add terabytes of storage or thousands of virtual machines.
    
- **Availability & SLAs:** The baseline SLA for virtual machines across AWS, Azure, and Google is **99.99% uptime**. _Important Exception:_ Azure and Google virtual machines MUST have multiple instances deployed across different availability zones to qualify for this 99.99% SLA.
    
- **Cloud Support Tiers:**
    
    - _AWS:_ Basic, Developer, Business, Enterprise.
        
    - _Azure:_ Basic, Developer, Standard, Professional direct.
        
    - _GCP:_ Basic, Developer, Production, Premium.