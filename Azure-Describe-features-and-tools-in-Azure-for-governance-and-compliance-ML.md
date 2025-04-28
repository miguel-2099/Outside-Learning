# [Describe features and tools in Azure for governance and compliance](https://learn.microsoft.com/en-us/training/modules/describe-features-tools-azure-for-governance-compliance/)

Unit 1/8 and 2/8:
  - Intro and Describe the purpose of Microsoft Purview:
    - Microsoft Purview is a family of data governance, risk, and compliance solutions. It provides a unified view into your data across on-prem, multicloud, and SaaS environments.
    - Key Features:
      - Automated data discovery.
      - Sensitive data classification.
      - End-to-end data lineage.
    - Solution Areas:
      1. Risk and Compliance: Utilizes MS 365 services like Teams, OneDrive, and Exchange. Helps protect sensitive data, identify data risks, and manage regulatory compliance.
      2. Unified Data Governance: Manages data across Azure, SQL, Hive databases, and other clouds like Amazon S3. Creates an up-to-date map of your data estate, identifies sensitive data, and generates insights.
    - Benefits:
      - Protects sensitive data across various platforms, manages regulatory compliance requirements, and secures data access and management at scale.

Unit 3/8:
  - Describe the purpose of Azure Policy:
    - Azure Policy is a service designed to ensure resources remain compliant with corporate standards by creating, assigning, and managing policies. These policies can audit and enforce rules across resource configurations, preventing noncompliant resources from being created. Policies can be defined individually or grouped into initiatives to track compliance for larger goals. They can be applied at various levels, such as resource, resource group, or subscription, and are inherited by lower-level groupings. Azure Policy includes built-in definitions for areas like storage, networking, computing, security center, and monitoring. It can automatically remediate non-compliant resources, with exceptions flagged as needed. Integration with Azure DevOps allows policies to be applied during pre-deployment and post-deployment phases. An example initiative, "Enable Monitoring in Azure Security Center," includes policies to monitor unencrypted SQL databases, OS vulnerabilities, and missing endpoint protection.
   
Unit 4/8:
  - Describe the purpose of resource locks:
    - Purpose: Prevent accidental deletion or modification of resources. Override Azure RBAC policies to ensure critical resources are protected.
    - Types of Locks:
      - Delete: Users can read and modify, but cannot delete the resource.
      - ReadOnly: Users can read but not delete or update the resource.
    - Application:
      - Locks can be applied to individual resources, resource groups, or entire subscriptions. If a resource group is inherited, all resources will inherit the lock.
    - Management: Manage locks via Azure portal, PowerShell, Azure CLI, or Azure Resource Manager templates.
    - Modification: To modify a locked resource, remove the lock first. Locks apply regardless of RBAC permissions.
   
Unit 5/8: Exercise

Unit 6/8: Describe the purpose of the Service Trust Portal:
  - Purpose: Provide access to content, tools, and resources about Microsoft security, privacy, and compliance practices.
  - Access: Requires signing in with a MS cloud services account and accepting the MS non-disclosure agreement for compliance materials.
  - Features:
    - Services Trust Portal:  Quick access hyperlink to home page.
    - My Library: Save documents for quick access and set up notifications for updates.
    - All Documents: Single landing place for all documents, with the option to pin documents to My Library.
  - Availability: Reports and documents are available for at least 12mo after publishing or until a new version is available. 

Unit 7/8 and 8/8: Module Assessment and Summary
