# [Describe the benefits of using cloud services](https://learn.microsoft.com/en-us/training/modules/describe-benefits-use-cloud-services/)

Unit 1/7 to 2/7:
  - Intro and Describe the benefits of high availability and scalability in the cloud:
    - High availability: It focuses on ensuring maximum availability, regardless of disruptions or events that may occur. Azure provides uptime guaranteesthrough SLAs (Service-Level Agreements).
    - Scalability: It's the ability to adjust resources to meet demand, so you can add more resources to better handle the increased demand if you suddenly experience peak traffic and systems are overwhelmend. The other benefit of scalability is that you aren't overpaying for services, because the cloud is a consumption-based model, you only pay for what you use.
    - Scalability generally comes in two varieties: vertical and horizontal. Vertical scaling is focused on increasing or decreasing the capabilities of resources. Horizontal scaling is adding or subtracting the number of resources.
      - Vertical scaling: If you are developing an app and you needed more processing power, you could vertically scale up to add more CPUs or RAM to the virtual machine. Conversely, if you realized you had over-specified the needs, you could vertically scale down by lowering the CPU or RAM specifications.
      - Horizontal scaling: If you suddenly experienced a steed jump in demand, your deployed resources could be scaled out automatically or manually. (i.e.: you could add additional virtual machines or containers, scaling out. In the same manner, if there was a significant drop in demand, deployed resources could be scaled in (either automatically or manually), scaling in.)
     
 Unit 3/7:
   - Describe the benefits of reliabilty and predictability in the cloud:
     - Two crucial cloud benefits that help you develop solutions with confidence are reliabilty and predictability.
     - Reliability is the ability of a system to recover from failures and continue to function. It's also one of the pillars of the Microsoft Azure Well-Architected Framework.
     - Predictability in the cloud lets you move forward with confidence. Predictability can be focused on performance predictability or cost predictability. Both performance and cost predictability are heavilty influenced by the MS Azure Well-Architected Framework.
     - Performance: Performance predictabilty focused on predicting the resources needed to deliver a positive experience for customers. Autoscaling, load balancing, and high availability are just some of the cloud concepts that support performance predictabilty. If you suddenly need more resources, autoscaling can deploy additional resources to meet demand, and then scale back when the demand drops. Or if the traffic is heavily focused on one area, load balancing will help redirect some of the overload to less stressed areas.
     - Cost: Cost predictabilty is focused on predicting or forecasting the cost of the cloud spend, you can track and monitor resources in real time to ensure you're using them in the most efficient way, and apply data analysis to find patterns and trends that help better plan resource deployment. You can predict future costs and adjust your resources as needed by operating and using the cloud analytics and information. Even using the Total Cost of Ownership (TCO) or Pricing Calculator to get an estimate of potential cloud spend.

Unit 4/7:
  - Decribe the benefits of security and governance in the cloud:
    - Cloud features support governance and compliance, wether you're deploying infrastructure (IaaS) or software as a service (Saas). Cloud-based auduting helps flag any resource that's out of compliance with your corporate standards and provides mitigation strategies. Depending on your operating model, software patches and updates may also automatically be applied, which helps with both governance and security. Things like set templates help ensure that all your deployed resources 







Describe the benefits of high availability and scalability in the cloud.
Describe the benefits of reliability and predictability in the cloud.
Describe the benefits of security and governance in the cloud.
Describe the benefits of manageability in the cloud.
