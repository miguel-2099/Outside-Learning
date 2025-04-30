# [Describe features and tools for managing and deploying Azure resources](https://learn.microsoft.com/en-us/training/modules/describe-features-tools-manage-deploy-azure-resources/)

Unit 1/6 and 2/6:
  - Intro and Describe tools for interacting with Azure (resources):
    1. Azure Portal:
      - Web-based, unified console for managing Azure subscriptions.
      - GUI for building, managing, and monitoring resources.
      - Custom dashboards for organized views.
      - Resilient and continuously available across all Azure datacenters.
    2. Azure Cloud Shell:
      - Browser-based shell tool supporting Azure PowerShell and Azure CLI.
      - No local installation is required; it is authenticated with Azure credentials.
      - Supports both PowerShell and Bash commands.
    3. Azure CLI:
      - Functionally equivalent to Azure PowerShell but uses Bash commands.
      - Handles discrete tasks or complex operations.
      - Installable on Windows, Linux, and Mac platforms.

Unit 3/6:
  - Describe the purpose of Azure Arc:
    - Managing Hybrid and Multi-Cloud Environments with Azure:
      - Azure Arc simplifies governance and management by providing a consistent platform for managing both multicloud environments.
      - Projects non-Azure resources into Azure Resource Manager (RAM) for unified/centralized management.
      - Resource Types Managed: Includes servers, Kubernetes clusters, Azure data services, SQL Server, and virtual machines (preview).
      - Capable of: Managing multi-cloud and hybrid virtual machines, Kubernetes clusters, and databases as if they are running in Azure. Use familiar Azure services and management capabilities across different environments.
      - Support traditional ITOps while introducing environments.
      - Configure custom locations on top of Azure Arc-enabled Kubernetes clusters.

Unit 4/6:
  - Describe Azure Resource Manager and Azure ARM templates:
    -  Azure Resource Manager (ARM):
      - Deployment and Management Service: ARM handles requests from Azure tools, APIs, or SDKs, authenticates and authorizes them, and sends them to the Azure service.
    - Benefits:
      - Declarative Templates: Manage infrastructure through JSON templates.
      - Group Management: Deploy, manage, and monitor resources as a group.
      - Consistent State: Ensure resources are deployed consistently throughout the development lifecycle.
      - Access Control: Integrated RBAC for all services.
      - Tagging: Organize resources and clarify billing.
    - Infrastructure as Code:
      - Concept: Manage infrastructure as code using tools like Azure Cloud Shell, Azure PowerShell, or Azure CLI.
      - ARM Templates: Describe resources in JSON format, ensuring correct creation and connection.
      - Benefits:
        - Declarative Syntax: Define desired state without programming commands.
        - Repeatable Results: Consistent deployment across environments.
        - Orchestration: Deploy interdependent resources in the correct order.
        - Modular Files: Use smaller, reusable components.
        - Extensibility: Include PowerShell or Bash scripts in templates.
      - Bicep:
        - Language: Uses declarative syntax to deploy Azure resources.
        - Benefits:
          - Support for All Resource Types: Immediate support for new Azure services.
          - Simple Syntax: Easier to read and write compared to JSON.
          - Repeatable Results: Consistent deployment across environments.
          - Orchestration: Deploy resources in the correct order.
          - Modularity: Uses modules to simplify development and reuse code.

Unit 5/6: Module Assessment

Unit 6/6: Summary
   






