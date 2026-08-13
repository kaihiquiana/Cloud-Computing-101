# Cloud Provider Comparison

## Overview

Cloud computing providers offer similar infrastructure capabilities, but each provider uses different service names and provides different features. This comparison examines the core infrastructure services of **Amazon Web Services (AWS)**, **Microsoft Azure**, and **Google Cloud Platform (GCP)**.

The comparison is based on the official documentation provided by each cloud provider.

## Cloud Infrastructure Service Comparison

| Infrastructure Component                 | AWS                                                                                                                | Microsoft Azure                                                                                                                      | Google Cloud Platform                                                                                                          |
| ---------------------------------------- | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ |
| **Compute**                              | **Amazon EC2 (Elastic Compute Cloud)** – provides scalable virtual servers for running applications and workloads. | **Azure Virtual Machines** – provides on-demand and scalable virtual machines with control over the computing environment.           | **Compute Engine** – provides configurable virtual machines running on Google's cloud infrastructure.                          |
| **Storage**                              | **Amazon S3 (Simple Storage Service)** – provides scalable object storage for storing and retrieving data.         | **Azure Blob Storage** – provides scalable object storage for large amounts of unstructured data.                                    | **Cloud Storage** – provides scalable, managed object storage using buckets and objects.                                       |
| **Networking**                           | **Amazon VPC (Virtual Private Cloud)** – provides a logically isolated virtual network for AWS resources.          | **Azure Virtual Network (VNet)** – provides a private network environment for Azure resources and communication with other networks. | **Virtual Private Cloud (VPC)** – provides networking capabilities for Google Cloud resources, including networks and subnets. |
| **Identity and Access Management (IAM)** | **AWS IAM** – manages users, roles, policies, and permissions for AWS resources.                                   | **Microsoft Entra ID + Azure RBAC** – manages identities and controls access to Azure resources through roles and permissions.       | **Google Cloud IAM** – manages access to Google Cloud resources using identities, roles, and permissions.                      |

AWS describes its platform as offering a broad range of cloud products covering compute, storage, networking, security, databases, analytics, AI/ML, developer tools, and other services. AWS documentation currently states that more than 200 services are available.

Azure Virtual Machines provide scalable computing resources, while Azure Storage includes Blob Storage and other storage services. Azure Virtual Network provides private networking for Azure resources, and Microsoft Entra ID provides cloud-based identity and access management.

Google Cloud provides Compute Engine for virtual machines, Cloud Storage for managed object storage, VPC for networking, and Google Cloud IAM for controlling access to resources through roles and permissions.

## Guide Questions

### 1. Which cloud provider offers the broadest range of services? Explain your answer.

**Amazon Web Services (AWS)** offers the broadest range of services among the three providers in this comparison. AWS provides more than 200 cloud services covering areas such as compute, storage, databases, networking, security, analytics, AI/ML, IoT, and developer tools.

### 2. Which cloud platform would you recommend for an organization that primarily uses Microsoft products? Why?

**Microsoft Azure** would be a strong recommendation for an organization that primarily uses Microsoft products. Azure integrates closely with Microsoft's ecosystem, including Microsoft Entra ID, Microsoft 365, Windows Server, and other Microsoft technologies, making identity management and integration easier for organizations already using Microsoft services.

### 3. Which platform is widely recognized for Artificial Intelligence (AI), Machine Learning (ML), and Kubernetes services?

**Google Cloud** is widely recognized for its strengths in AI, machine learning, data analytics, and Kubernetes. Google Cloud provides AI/ML services and **Google Kubernetes Engine (GKE)**, a managed Kubernetes service designed for running containerized applications.

### 4. What similarities did you observe among the three cloud providers?

All three providers offer equivalent fundamental cloud infrastructure services, including virtual machines for compute, scalable storage, virtual networking, and identity and access management. They also provide services designed to support scalability, security, high availability, and flexible resource management, although the service names and specific features differ between providers.

## Conclusion

AWS, Microsoft Azure, and Google Cloud provide comparable foundational cloud infrastructure services while using different service names and management models. Understanding these equivalents allows cloud engineers to transfer their knowledge between platforms and select a provider based on an organization's technical requirements, existing technology ecosystem, and workload needs.
