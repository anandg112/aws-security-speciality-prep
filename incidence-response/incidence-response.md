## Incidence Response  
**Note: AWS does not allow port scanning or pen testing of your resources without permission**

**Incident** - An unplanned interruption or degradation of an IT service  
1. Incident Response Framework
* Preparation – Proactive steps to take action before the incident  
  * Be proactive
    *  Risk management – Determine where the different levels of risks are
    * Principle of least privilege – No unnecessary permissions
    * Architect for failure - high availability and fault tolerance always
    * Train for the real thing – Test and simulate; a real incident is a horrible place to learn lesson
    *	Clear ownership and governance – Tag all resources so no time is wasted finding who or what group to contact
    * Data classification – tagging data stores with classification can quickly identify spillage  
  **AWS services involved – IAM, VPC, EC2, EFS, RDS**  

  * Limit the blast radius
**Careful planning can reduce the “blast radius” of any attack. The idea here is to segment/section off resources from each other. Best practices are:**
    * Organizations – we can add accounts under our main account
    * Benefits: 
      * If there is a breach, it will not affect multiple accounts
      * Service Control policies can be set so “child” accounts can be limited
      * Using multiple Regions and VPCs can have a similar effect (ONLY network-level protection)  
**AWS Services – Organizations, VPCs**

  * Log Everything 
Logging is the best way to collect information about our environments. Logs are also the beginning of being able to monitor a lot of resources. We can search the logs for information or automate responses based on patterns and alarms. Some of the best practices are: