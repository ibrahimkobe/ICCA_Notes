# ☁️ Cloud Computing & Security Notes

> Structured study notes covering cloud fundamentals, cloud management, and cloud identity, security & compliance, with a vendor-neutral view across **AWS**, **Microsoft Azure**, and **Google Cloud Platform (GCP)**.

![Topic](https://img.shields.io/badge/Topic-Cloud%20Security-blue)
![Providers](https://img.shields.io/badge/Providers-AWS%20%7C%20Azure%20%7C%20GCP-orange)
![Format](https://img.shields.io/badge/Format-Markdown-lightgrey)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 📖 Overview

This repository contains concise, well-organized notes built from cloud computing course material. Each document is written to work both as a first-time learning resource and as a quick revision sheet, with side-by-side comparisons of the three major cloud providers wherever possible.

---

## 📂 Repository Structure

```text
.
├── Cloud Foundations.md
├── Cloud Management Concepts.md
├── Fundamentals of Cloud Identity, Security & Compliance.md
└── README.md
```

| File | Focus |
|------|-------|
| [Cloud Foundations](./Cloud%20Foundations.md) | What the cloud is, IaaS/PaaS/SaaS, market and providers, CapEx vs OpEx, scalability, SLAs and support tiers |
| [Cloud Management Concepts](./Cloud%20Management%20Concepts.md) | Shared responsibility, control plane vs data plane, asset lifecycle, cost optimization, monitoring, IAM best practices |
| [Fundamentals of Cloud Identity, Security & Compliance](./Fundamentals%20of%20Cloud%20Identity,%20Security%20%26%20Compliance.md) | Defense in depth, common attacks, identity protection, data/network/compute protection, regulatory compliance |

---

## 🧭 Topics Covered

### 1. Cloud Foundations
- On-premises vs cloud architecture and who owns which layer
- Service models: **IaaS**, **PaaS**, **SaaS** with provider-specific examples
- Cloud market share and provider profiles (AWS, Azure, GCP)
- Cloud economics: **CapEx vs OpEx**, capacity-based vs consumption-based pricing
- Scalability, availability, the 99.99% VM SLA and its multi-zone exception
- Support tiers across providers

### 2. Cloud Management Concepts
- **Shared Responsibility Model** and resiliency responsibility
- **Control Plane vs Data Plane** (REST APIs, consoles, CLIs)
- Asset lifecycle: provision, configure, maintain, monitor, change management
- Cost management and optimization (right-sizing, autoscaling, serverless, commitments)
- Native and third-party monitoring and alerting
- **IAM** tooling and best practices (least privilege, root minimization, access audits)

### 3. Cloud Identity, Security & Compliance
- **Defense in Depth** layers, from DDoS protection to encryption
- Common attack targets and methods (misconfiguration, account and service hijacking, malware)
- Identity protection and the **Five R's** of incident response: Revoke, Reset, Review, Remediate, Return
- Data protection at rest and in transit
- Network and compute protection, including **Confidential Compute** (Trusted Execution Environments)
- Compliance tooling and protected data types (PII, PHI, PCI-DSS, SOX, GDPR)

---

## ☁️ Provider Quick Reference

| Area | AWS | Azure | GCP |
|------|-----|-------|-----|
| Monitoring | CloudWatch | Azure Monitor | Cloud Monitoring |
| Identity | IAM Users, Roles, Policies | Azure AD Users, Service Principals, Managed Identities | Google Account, Service Account, Role, Policy |
| Network Controls | Network ACL, Security Group | Network Security Group | Firewall Rule, VPC Service Controls |
| Network Security | Shield, WAF, GuardDuty | Azure Firewall, Application Gateway, Front Door | Cloud Armor |
| Cost Optimization | Cost Anomaly Detection | Azure Advisor | Google Recommender |
| Compliance | Artifact | Trust Center, Compliance Manager | Compliance Resource Center, Security Command Center |

---

## 🎯 Who This Is For

- Students learning cloud computing and cloud security fundamentals
- Aspiring cloud, security, and DevOps engineers
- Anyone preparing for cloud or cybersecurity certifications
- Professionals who want a fast, structured refresher

---

## 🚀 How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/ibrahimkobe/<repository-name>.git
   ```
2. Open any `.md` file in your editor or browse it directly on GitHub.
3. Start with **Cloud Foundations**, then move to **Cloud Management Concepts**, and finish with **Cloud Identity, Security & Compliance**.

---

## ⚠️ Disclaimer

These notes are for educational purposes. Cloud services, pricing, SLAs, and market figures change frequently. Always verify against the official AWS, Azure, and Google Cloud documentation before making technical or business decisions.

---

## 🤝 Contributing

Corrections and improvements are welcome:

1. Fork the repository
2. Create a branch (`git checkout -b fix/topic-name`)
3. Commit your changes (`git commit -m "Improve topic section"`)
4. Push and open a Pull Request

---

## 👤 Author

**Ibrahim**
Cybersecurity student at Al-Hussein Technical University (HTU), Amman, Jordan

- GitHub: [@ibrahimkobe](https://github.com/ibrahimkobe)
- LinkedIn: [linkedin.com/in/ibrahimabukobe](https://linkedin.com/in/ibrahimabukobe)

---

## 📄 License

This project is licensed under the [MIT License](./LICENSE).

⭐ If you find these notes useful, consider giving the repository a star.
