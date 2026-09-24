# Cloud Platform Recommendations

## Client A – Startup Company
**Recommended Platform:** AWS

**Recommendation:**
AWS is ideal for this startup because it offers a generous Free Tier to minimize early costs and scales seamlessly as the company grows. Its broad service marketplace means the startup can adopt new tools without switching platforms. AWS also has the largest community and documentation, which helps small teams move quickly.

**Recommended Services:**
- **Amazon EC2** — Host the mobile application backend.
- **Amazon S3** — Store user uploads, app assets, and backups affordably.
- **Amazon RDS** — Managed database service to handle growing user data without administration overhead.

---

## Client B – University
**Recommended Platform:** Microsoft Azure

**Recommendation:**
Azure is the natural choice because the university already relies on Windows Server, Active Directory, and Microsoft 365. Azure integrates directly with these systems, reducing the need to retrain staff or rebuild identity management from scratch. It also offers educational pricing and licensing benefits.

**Recommended Services:**
- **Azure Virtual Machines** — Migrate existing Windows-based campus services.
- **Microsoft Entra ID** — Extend current Active Directory identities into the cloud.
- **Azure SQL Database** — Host student information systems with built-in security and automated backups.

---

## Client C – AI Research Company
**Recommended Platform:** Google Cloud Platform (GCP)

**Recommendation:**
GCP is best suited because it leads in AI innovation and offers specialized hardware like Tensor Processing Units (TPUs) designed specifically for machine learning workloads. As the creator of Kubernetes, GCP also provides the most stable environment for containerized research pipelines.

**Recommended Services:**
- **Google Compute Engine** — High-performance virtual machines with GPU/TPU acceleration.
- **Google Kubernetes Engine (GKE)** — Orchestrate large-scale model training jobs efficiently.
- **Google BigQuery** — Analyze massive research datasets with serverless data warehousing.

---

## Client D – Global E-Commerce Company
**Recommended Platform:** AWS

**Recommendation:**
AWS has the most mature global infrastructure and proven experience supporting large-scale retail platforms. Its auto-scaling and content delivery capabilities ensure the store remains fast and available worldwide, even during traffic spikes.

**Recommended Services:**
- **Amazon EC2 with Auto Scaling** — Automatically adjust capacity during sales events or holidays.
- **Amazon S3 + CloudFront** — Store product images and serve them globally with low latency.
- **Amazon RDS with Multi-AZ** — Highly available database to prevent data loss and ensure reliability.

---

## Multi-Cloud Decision Matrix

| Business Requirement | Recommended Platform | Justification |
|---|---|---|
| Startup Company | AWS | Free Tier, broad service selection, strong community, scalable growth path |
| Enterprise Organization | AWS | Mature compliance, global reach, proven reliability, extensive enterprise tools |
| Microsoft Environment | Azure | Native integration with Windows, AD, and Office 365; consistent management experience |
| AI / Machine Learning | GCP | TPUs, built-in ML tools, TensorFlow integration; Google's own AI infrastructure |
| Kubernetes Deployment | GCP | Invented Kubernetes; GKE is most feature-complete and stable |
| Global Web Application | AWS | Largest edge network, auto-scaling maturity, longest track record of availability |
