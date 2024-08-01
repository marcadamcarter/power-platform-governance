# Environments
Power Platform environments are spaces where you can store, manage, and share your organization's business data, apps, chatbots, and flows. Each environment type serves a specific purpose, helping organizations manage their applications and data effectively. Below are the different types of Power Platform environments:  

[See Environment Strategies](/environments/environment-strategies.md)

|Type|Creator|Dataverse Instance|Security|
|----|-------|------------------|--------|
|**Default**|Auto-created|Mandatory|Limited control. All licensed users have the environment maker role.|
|**Production**|Licensed user, subject to tenant-level settings|Mandatory|Full control.|
|**Sandbox**|Licensed user, subject to tenant-level settings|Optional|Full control. If used for testing, only user access is needed. Developers require environment maker access to create resources.|
|**Developer**|Licensed User|Optional|Limited control. Security groups can't be assigned to developer environments.|
|**Dataverse for Teams (D4T)**|Auto-created|Mandatory|Limited control. Admins have limited settings available for Teams environments. No customizations of security role or assignments are available. Teams members are automatically mapped to their Teams membership type - owners, members, and guests - with a corresponding security role assigned by the system.|  

## Default Environment:
   - **Description**: Automatically created for each tenant and shared by all users.
   - **Use Case**: Ideal for personal productivity apps and initial exploration of Power Platform capabilities.  

## Production Environment:
   - **Description**: Used for deploying live applications that are used by end-users.
   - **Use Case**: Suitable for business-critical applications that require high availability and reliability.

## Sandbox Environment:
   - **Description**: A non-production environment used for development and testing.
   - **Use Case**: Allows developers to test new features and updates without affecting the production environment.

## Developer Environment:
   - **Description**: Personal environment for individual developers. Intended only for use by the owner and **cannot be shared with other users**.
   - **Use Case**: Ideal for building and testing apps in isolation before moving them to a shared environment. Development environments should be single-purpose, disposable, and easily recreated.  

## Trial Environment:
   - **Description**: |**Trial**|Licensed user, subject to tenant-level settings|Optional|Full control.|
   - **Use Case**: Useful for evaluating Power Platform capabilities before committing to a full license.

## Dataverse for Teams Environment:
   - **Description**: Integrated with Microsoft Teams, providing a lightweight Dataverse experience.  Dataverse for Teams environments are automatically created for a Team when you create an app in Teams using Power Apps for the first time or install a Power Apps app from the app catalog.
   - **Use Case**: Suitable for building low-code apps and automations within Teams¹²³.  

## Changing Environment Type
You may decide that your customization work developed and tested on a sandbox environment is now ready to go live. If you’ve placed your sandbox environment in administration mode, only users with System Administrator or System Customizer security roles are able to sign in to that environment. Once you change the environment type to production, all your users within your organization can access your environment. When you configure or edit an environment, you can change the environment from:  
- Production to sandbox  
- Sandbox to production  

## White papers
  - [Develop a tenant environment strategy to adopt Power Platform at scale (microsoft.com)](https://learn.microsoft.com/en-us/power-platform/guidance/white-papers/environment-strategy)
  - [Enterprise security with Power Platform (microsoft.com)](https://learn.microsoft.com/en-us/power-platform/guidance/white-papers/enterprise-security)
## References
  - [https://learn.microsoft.com/en-us/power-platform/admin/switch-environment](https://learn.microsoft.com/en-us/power-platform/admin/switch-environment)
  - [https://learn.microsoft.com/en-us/power-platform/admin/environments-overview#power-platform-environment-types](https://learn.microsoft.com/en-us/power-platform/admin/environments-overview#power-platform-environment-types)
