# Cloud Platform Recommendations

## Client A — Startup Company
**Recommended: AWS**

AWS is the best choice for this startup. Their Free Tier program helps keep costs low while the business is growing. Services like EC2 and S3 are easy to set up and can grow automatically as more people use the app.

**Services to use:**
- Amazon EC2 for the app server
- Amazon S3 for storing files
- Amazon RDS for the database

## Client B — University
**Recommended: Azure**

Azure fits perfectly here because the university already uses Windows Server, Microsoft 365, and Active Directory. Everything will work together without extra setup. Students and staff can use the same accounts they already have.

**Services to use:**
- Azure Virtual Machines for existing servers
- Entra ID for user accounts
- Azure Files for shared storage

## Client C — AI Research Company
**Recommended: Google Cloud Platform**

GCP has the best tools for AI and machine learning. They offer special hardware that speeds up AI work, and their data services work together smoothly. Many researchers already use Google tools, so the team will feel comfortable.

**Services to use:**
- Vertex AI for building models
- Google Compute Engine with fast processors
- BigQuery for research data

## Client D — Global E-Commerce Company
**Recommended: AWS**

AWS has the most data centers around the world, which means fast loading for customers everywhere. They are also very reliable and can handle sudden traffic spikes during sales events.

**Services to use:**
- EC2 with auto-scaling
- CloudFront for fast content delivery
- RDS for product and order database

## Decision Matrix
| Business Requirement | Recommended Platform | Reason |
|---|---|---|
| Startup Company | AWS | Free Tier, lots of help online, grows easily |
| Enterprise Organization | Azure | Good security, reliable, enterprise tools |
| Microsoft Environment | Azure | Works natively with Windows and Office |
| AI / Machine Learning | GCP | Best AI tools and research environment |
| Kubernetes | GCP | Created it, best support and performance |
| Global Web App | AWS | Most regions worldwide, proven reliable |