# [Describe Azure management and governance](https://learn.microsoft.com/en-us/training/paths/describe-azure-management-governance/)

Unit 1/9 and 2/9:
  - Intro and Factors that can affect costs in Azure:
    - Operational expense (OpEx) of renting infrastructure as you need it, whether it's compute, storage, networking, and so on:
    - They are:
      - Resource Type:  Different types of resources, like storage accounts and virtual machines, have varying costs based on settings and regions. Measured instances that track resource usage and generate a usage record that is used to calculate bills.
      - Consumption: Pay-as-you-go model: Pay for resources used during a billing cycle. Reserved resources: Commit to a set amount of resources in advance for discounts.
      - Maintenance: Regularly maintain and organize resources to control costs. Deprovision unnecessary resources to avoid extra charges.
      - Geography: Costs vary by region due to differences in power, labor, taxes, and fees. Network traffic costs differ based on geographical zones.
      - Subscription type: Different subscription types offer various usage allowances and free access to certain products.
      - Azure Marketplace: Purchase third-party solutions and services, which may include additional costs for vendor services.

Unit 3/9:
  - Comparing pricing calculator and total cost of ownership (TCO): 
    - The calculators help understand potential Azure expenses. Both are accessible from the internet, and both calculators allow you to build out a configuration. However, the two calculators have very different purposes:
      - [Pricing calculator](https://learn.microsoft.com/en-us/training/wwl-azure/describe-cost-management-azure/media/price-calculator-0a750ac3.png): It's designed to give you an estimated cost for provisioning resources in Azure. You can get an estimate for individual resources, build out a solution, or use an example scenario to see an estimate of the Azure spend. The pricing calculator's focus is on provisioned resources in Azure. (The Pricing calculator is for information purposes only. The prices are only an estimate. Nothing is provisioned when you add resources to the pricing calculator, and you won't be charged for any services you select.)
        - With the pricing calculator, you can estimate the cost of any provisioned resources, including compute, storage, and associated network costs. You can even account for different storage options like storage type, access tier, and redundancy.
       - [TCO Calculator](https://learn.microsoft.com/en-us/training/wwl-azure/describe-cost-management-azure/media/total-cost-ownership-657fe344.png): The TCO calculator is designed to help you compare the costs of running an on-prem infrastructure compared to an Azure Cloud infrastructure. With it, you enter the current infrastructure configuration, including servers, database, storage, and outbound network traffic. Also, you can add in assumptions like power and IT labor costs, and are presented with an estimation of the cost difference to run the same environment in your current datacenter or Azure. The TCO calculator then compares the anticipated costs for your current environment with an Azure environment supporting the same infrastructure requirements.

Unit 4/9:
  - Estimate workload costs by using the pricing calculator:
    - Define Requirements: Identify the necessary Azure services, such as Virtual Machines, Application Gateway, and SQL Database.
    - Configuration Details: Set specific values for each service, including region, operating system, instance type, and storage.
    - Review and Save: Review the total estimated cost, and share it with your team.

Unit 5/9: Exercise - Compare workload costs using the TCO calculator

Unit 6/9: 
  - Describe the MS Cost Management Tool:
    - The Azure Cost Management helps you monitor and manage your Azure spending. It provides tools for cost analysis, alerts, and budgeting.
  - Cost Analysis:
    - Visualise costs: View costs by billing cycle, region, resource, etc.
    - Identify Trends: Understand spending patterns and forecast future costs.
  - Cost Alerts (types):
    - Budget Alerts: Notify when spending exceeds defined limits.
    - Credit Alerts: Inform when Azure credit is consumed (for Enterprise Agreements).
    - Department Spending Quota Alerts: Alert when departamental spending reaches set thresholds.
  - Budgets:
    - Set Spending Limits: Define budgets based on subscription, resource group, or service type.
    - Automate Management: Trigger actions like suspending resources when budget conditions are met.
  - Support:
    - Help Available: Explore existing questions or ask new ones on MS Q&A for issues related to this module. 

Unit 5/5: 
  - Describe the purpose of tags:
    - Organization Strategy: As cloud usage grows, organizing resources effectively is crucial for understanding usage and managing costs.
    - Resource Tags:
      - Resource Management: Locate and manage resources by workloads, enviroments, business units, and owners.
      - Cost Management: Group resources for cost reporting, budget tracking, and cost forecasting.
      - Operations Management: Group resources by their criticality to business operations, aiding in SLA formulation (service-level agreements).
      - Security: Classify data by security levels, such as public or confidential.
      - Governance and Compliance: Identify resources that meet governance or regulatory requirements.
      - Workload Optimization and Automation: Visualize resources in complex deployments and automate tasks using tools like Azure DevOps.
      - Managing Tags: Tags can be added, modified, or deleted using various tools like PowerShell, Azure CLI, and Azure portal. Azure policy can enforce tagging rules and conventions.
      - Tagging Structure: Tags consist of a name and value, and examples include AppName, CostCenter, Owner, Environment, and Impact.

Unit 8/9: Module Assessment

Unit 9/9: Summary










