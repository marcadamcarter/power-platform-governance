# Purpose 
The US Army is digitally transforming its IT workspace and modernizing its productivity suite to increase business productivity, collaboration, efficiency, and accessibility. To achieve these goals, the Army is using Microsoft Office 365 (O365) Government cloud services and integrating those services with the Army network through the O365 DoD Impact Level 5 (IL5) tenant which is known as Army 365. IL5 (Impact Level 5) is a DoD cloud and has specific security and access requirements referenced in the Department of Defense Cloud Computing Security Requirements Guide (Cloud SRG).  
This document describes recommended AMC governance practices and provides guidance related to technical and operational topics to ensure the operation and management of the Microsoft Power Platform in the Army Enterprise environment. All users should become familiar with the concepts described in more detail in Microsoft’s official Power Platform Admin and Governance Whitepaper. Please note that some capabilities may not be available in Army 365. 
AMC intends for organization members to adhere to Army regulation, governance provided by Headquarters Department of Army (HQDA), and by more specific requirements identified in this document. Adherence to standardized governance facilitates the integration of Information Technology solutions across the A365 environment. 

## Reference Documentation 
1.	NETCOM Draft SharePoint Online Governance 
2.	Power Platform Admin and Governance Whitepaper 
3.	https://learn.microsoft.com/  

# AMC A365 SharePoint Online 
Organizations should use SharePoint Online for cross-team/cross-organization co-authoring and collaboration, sharing to multiple groups, and for providing access to finalized documents. Use SharePoint Online to store long term records with accordance with current Army Records Management Programs authorized under Army Regulation 25-400-2.  

# AMC A365 MS Teams 
MS Teams should be the primary tool for AMC users to simultaneously co-author documents and collaborate on projects within their internal staffs or working groups. Teams are primarily used for internal communication with immediate co-workers. The A365 group associated with a MS Team is also used to provide access to content within SharePoint Online. When an AMC user establishes a team, the team owner should only add those members with a need to know. MS Teams is not intended for long term storage of files or records. 

# OneDrive 
Users should utilize OneDrive for personal productivity and storing personal work-related files that do not primarily require collaboration or sharing. Maintaining and working with files from OneDrive allows access to those items with most any Windows based Army desktop connected to the NIPRnet. 

# Power Platform Vision  
Take advantage of data where data lives to rapidly advance local capabilities and increase velocity across the operational spectrum. Leverage the Power Platform to feed AMC's data production and consumption model. Prioritize licensing based on data consumption demand, utility and over all mission impact. 

# Help Desk Ticket Submission 
Service responsibility exists at several different levels and with many different organizations within the A365 platform. To ensure the most efficient response and handling of issues, use the following service request procedures. 

## One Drive 
Work with the organization’s lowest level Information Technology (IT) Team to resolve issues prior to submitting tickets to directly to NETCOM.  
  - Proceed to: https://www.aesmp.army.mil 
  - Select “Something is Broken” 
  - Complete all fields and provide URLs/Web Addresses and issue details as accurate and succinct as possible 

## MS Teams 
Work with the organization’s lowest level Information Technology (IT) Team to resolve issues prior to submitting tickets to directly to NETCOM. When organizations exhaust all efforts for remediation at the lowest IT level, submit an AESMP incident ticket. 
  -	Proceed to: https://www.aesmp.army.mil 
  -	Select “Something is Broken” 
  -	Complete all fields and provide URLs/Web Addresses and issue details as accurate and succinct as possible  

## MS SharePoint Online  
Organizations must seek to resolve issues at the lowest level. When organizations exhaust all efforts for remediation at the lowest level, it is appropriate to seek assistance from the next higher command’s SharePoint Team. For issues where remediation must occur at the tenant level, the Army Materiel Command’s appointed Major Command Level Administrator (MCLA) must facilitate an AESMP incident entered by the affected organization.  

#### Entering Tickets for Support from the Army Materiel Command Enterprise Portal Team (AEP)  
  -	Initiate a request with the AEP using any of the following methods 
    - Email the AEP Team: USAMC-HQAMC_AEP_SharePointTeam@army.mil 
    - Email the AEP NIPR Help Desk: usarmy.redstone.usamc.mbx.aep-helpdesknipr@mail.mil  
    - Assign an AESMP ticket directly to the AEP Assignment Group in the AESMP Service Management System: AMC HQ GITOC - Web Application 
    - Email the AMC GITOC and request assignment to the AMC AEP Team: usarmy.redstone.usamc.mbx.gitoc@army.mil  
      - GITOC requests must include the following in the body of the email in the same format: 
        - User Name  
        - MSC/ORG/Command  
        - Phone 
        - Email 
        - DoD ID 
        - ISSUE 
      - Call the AMC GITOC and request assignment to the AMC AEP Team:  
        - Hours: M-F 0600-1800 
        - (256)-450-8888, Option 1  

### Entering Tenant Level Tickets 
  - The affected organization must notify and receive approval from the AMC MCLA for elevating an issue to NETCOM 
  - Initiate a ticket with the AEP using one of the steps listed under Entering Tickets for Support from the AEP 
  - The AEP Team will forward or create the affected organization’s AESMP ticket with the date and time of AMC MCLA approval and AMC MCLA contact information to NETCOM 
  - NETCOM verifies ticket association to the AMC MCLA appointees registered with NETCOM  

### Examples of When to Enter Tenant Level Tickets with the AMC MCLA 
  - When a site collection cannot be added to the Hub (i.e. permissions issue with Command Hub Administrators (CHA) or Deputy Command Hub Administrators that needs addressed by the NETCOM team) 
  - When a site collection requires renaming 
  - When a Power Apps Premium Capacity Environment (PCE) needs created 

## Power Platform 
For technical issues not related to entitlements, licensing, or development methods; work with the organization’s lowest level Information Technology (IT) Team to resolve issues prior to submitting tickets to directly to NETCOM. When organizations exhaust all efforts for remediation at the lowest IT level, submit an AESMP incident ticket. 
  - Proceed to: https://www.aesmp.army.mil 
  - Select “Something is Broken”  

Complete all fields and provide URLs/Web Addresses and issue details as accurate and succinct as possible.  

# AMC A365 Naming Conventions  
Naming conventions of sites and all custom created solutions should allow for an immediate recognition of the owning organization. Due to the centralization of Army organizations to the A365 platform, naming conventions are crucial to efficiently determine ownership of content, enable support, and facilitate transition of permissions in the event of group or team ownership changes. Microsoft 365 Security Groups are visible to organizations throughout the Microsoft 365 environment. Avoid generic names when creating teams, groups, and sites. 

## Microsoft SharePoint Online Sites 
SharePoint Online sites provisioned to AMC organizations will adhere to the following naming convention.  
Naming Convention Example: AMC-(Command)-(SubCommand)_DescriptiveName  
## Microsoft Teams 
Team/Group owners should create teams or groups through Outlook and then create the associated MS 
Team from the Microsoft 365 security group to avoid a later need to submit an Army Enterprise Service Management Platform (AESMP) ticket to enable the group email address. Creating a Microsoft Team does not automatically enable use of the connected email address. Microsoft Teams automatically creates a connected Microsoft 365 security group when a user creates a Microsoft Team. Users must rename any existing teams to conform to AMC naming conventions. AMC requires that users adhere to the following naming convention when creating or renaming a team within Microsoft Teams. NonPrivate MS Teams shall have “Public” appended to the descriptive name to help avoid privacy breach incidents. Omit sub-command or sub-office where applicable. Avoid using spaces and special characters within the entire name except for hyphen ( - ) and underscore ( _ ).  

### Naming Convention Example: 
  - AMC_(Command)-(SubCommand)_(PrimaryOfficeSymbol)-(SubOfficeSymbol)_DescriptiveName 
  - AMC_(Command)-(SubCommand)_(PrimaryOfficeSymbol)-
(SubOfficeSymbol)_DescriptiveNamePublic 

### Renaming a Microsoft Team: 
Renaming a team within Microsoft Teams will automatically rename the connected Microsoft 365 Security Group. Renaming a team within Microsoft Teams will not rename the Microsoft team connected email. 
  - Renaming the Microsoft team connected email requires submission of a ticket to the Army Enterprise Service Management Platform (AESMP): https://www.aesmp.army.mil/ 

### Microsoft 365 Power Platform Solutions 
AMC requires that users adhere to the following naming convention when creating or renaming a Power App solution, Power BI solution, or a Power Automate flow. Omit sub-command or sub-office where applicable.  

Naming Convention Example:  
- AMC_(Command)-(SubCommand)_(PrimaryOfficeSymbol)-(SubOfficeSymbol)_DescriptiveName 

### Power Platform Security Enabled A365 Groups 
Managing and accessing premium capacity services requires the use of Security enabled A365 groups. 
Omit sub-command or sub-office where applicable.  
  - For PCE administrative groups:  
    - AMC_HQ_PowerPlatform_(Command)_Makers 
  - For PCE user groups: 
    - AMC_HQ_PowerPlatform_(Command)_Users 
  - For specific purpose groups: 
    - AMC_HQ_PowerPlatform_(Command)_(Description) 

### Power Platform Premium Capacity Environments 
Each MSC has a basic PCE set of Developer, Test, and Production provisioned through AMC HQ requests to NETCOM.  
  - For developer environments: 
    - AMC_(Command)_(SubCommand)_Dev 
  - For test environments:  
    - AMC_(Command)_(SubCommand)_Test 
  - For production environments: o AMC_(Command)_(SubCommand)_Production 
  - For unique environments: 
    - AMC_(Command)_(SubCommand)_(UniqueEnvironmentDescription) 

# AMC Innovation Factory 

## AMC Innovation Factory Change Advisory Board 
AMC HQ will establish and maintain an AMC Army 365 Innovation Factory Change Advisory Board (CAB) weekly working group with downtrace units to nest within NETCOMs quarterly battle rhythm. The AMC working group should include appointed representatives from the AMC HQ Knowledge Management Office, AMC HQ Records Management Office, AMC Major Command Level Administrator (MCLA), appointed AMC Command Hub Administrators (CHAs), appointed AMC Deputy Command Hub Administrators (DCHAs), and AMC G-6 Chief Information Officers (CIOs) or CIO designated representatives.  

Topics during weekly meetings should cover:  
  - Completed governance changes 
  - Requests for governance changes 
  - Socialization and nomination of solutions for the AMC Innovation Factory 
  - Technical discussions and requests for assistance  

Major changes to governance within this document will only occur collaborative decision of the AMC Army 365 Innovation Factory Change Advisory Board. Changes to AR Policies, Guidance, Regulations that affect established policies and procedures within this document should trigger a review for directed updates to this document during the next soonest AMC Army 365 Innovation Factory CAB meeting.  

The AMC HQ Enterprise Services Branch will make grammatical or technical corrections to this document as needed.  

### AMC Innovation Factory Solution Registration 
Solutions can consist of any single Power Platform capability or a complex mixture of Power Apps, Power BI, and Power Automate etc. Registration of solutions within the AMC Innovation Factory Solution Registration tool applies to meeting any of the following conditions: 
  - The solution assists with Command & Control (C2) 
  - The solution aids with contested logistics efforts 
  - The solution enhances leadership visibility 
  - The solution enhances "support operations" 
  - The solution increases efficiencies (fiscal, labor, or both) 
  - The solution automates an Army process at the AMC Major Subordinate Command (MSC) level or across commands  

#### To register a Solution 
  - Proceed to: https://armyeitaas.sharepointmil.us/sites/HQAMC/SitePages/AMC_HQ_AMIO_AIFSR.aspx  
  - Locate the AMC Innovation Factory Solution Registration (AIFSR) application on the page 
  - Select “Register a Solution” and follow the data entry prompts 

#### Adoption of Enterprise Solutions 
![AMC Innovation Factory - App Example](media/AMC-app%20example.png)  
1.	Each AMC MSC is provisioned MSC CIO managed development, test, and production Power Apps Premium Environments.  The environments enable MSC citizen developers to build Power Apps that drive outcomes within their MSC and sub-ordinate organizations. 
2.	The AMC Innovation Factory Center of Excellence is an executive-sponsored IPT with the mission to scale innovative ideas and solutions from the MSCs and subordinate organizations into enterprise solutions that impact multiple AMC organizations.  This outcome focused organization has representatives from every AMC MSC and aligns people and technology 
resources toward solutions.  An Innovation Factory Power App, developed and sustained by the AMC G-6, supports the overarching Innovation Factory process. 
3.	The Innovation Factory Center of Excellence aligns resources to solutions, choosing the right technology stack for the solution and aligning engineering support to the outcome. 
4.	Azure DevOps, or a like source code/project management solution, enables the inner-source movement within AMC.  The platform supports transparent project management, the ability to manage work items (requirements, user stories, issues), user feature requests, and integrates documentation.  For advanced Power Platform developers and professional development projects, the platform supports modern software development practices like continuous integration/delivery, software supply chain management, DevSecOps, and Continuous ATO. 

# Premium Capacity Environments 

## License Requests 

### Update Identification Card Online (IDCO) 
Entitlement Managers (EMs) and any user seeking any A365 entitlements must ensure their information is entered and correct within the IDCO system according to your closest Chain of Command (CoC). AMC currently has 10,000 Premium Maker Licenses available to distribute proportionately across the Command with the remaining 140,000 licenses needed for end users to use and consume premium capacity solutions. Careful management of the distribution of these licenses is crucial to the success of AMC’s innovation strategy. 
  - Proceed to: https://idco.dmdc.osd.mil/idco/ 
  - Use the “My Profile” feature to update user information o Duty Sub Organization o Duty Installation Location o Office Symbol 

### Identifying Organization Entitlement Managers 
Use the following procedure to identify an organization’s EM 
  - Proceed to: https://portal.apps.deas.mil/ 
  - Use the Login link to perform a Common Access Card login 
  - Select “My Self-Service” from the navigation menu 
    - Select “My GM/EM Contacts” 
    - Enter the user’s duty location within the “Duty Location” field to filter the GM/EM contacts to that location  
    - Verify the display name of a GM/EM contains the user’s command name 

### Contact the Organization Entitlement Manager 
Each organization’s Entitlement Manager can issue A365 entitlements from a pool of licenses provisioned by the Group Manager (GM). 
  - Provide the type of license required 
  - Provide the Command business need 

## Security Enabled A365 Groups 
Managing and accessing premium capacity services requires the use of Security enabled A365 groups. The Security Enabled Flag is only applied through the Microsoft Entra ID Azure tool that is only accessible by NETCOM Tenant and Global Administrators. 
  - Create an A365 group using Outlook and adhering to AMC naming conventions 
  - Submit an AESMP ticket by proceeding to: https://www.aesmp.army.mil/ 
  - Select “Request Something” 
  - Select “Army 365” as the “Business Service” 
  - Select “M365 Group” as the “Category” 
  - Select “M365 Group” – Other as the “Subcategory” 
  - Provide the exact group names in the “Comment” field along with a statement of “Please add the Security Enabled flag to the listed M365 groups” 

## Requesting Environments 
The requesting organization must provide a security enabled A365 group for the PCE administrators when requesting an environment and maker licenses must be assigned to every member of the provided PCE administrator group. The default set of PCEs provided will consist of Developer, Test, and 
Production environments. Additional environments require justification to both the Command Premium Capacity Manager and Major Command Level Administrator (MCLA).  
  - Environments must have approval from the requesting organization’s Chief Information Officer with justification in memorandum 
  - Initiate a request by emailing the AMC MCLA Team: army365-mcla-amc@army.mil  
    - The request must include: 
      - CIO Environment request approval  
      - Provide the desired premium capacity environment (PCE) name within the request. Environments must match the AMC naming convention replacing or omitting sub-command where applicable. Additional, unique, environments will have a succinct but descriptive name that clearly associates the environment to the purpose or solution 
      - Estimated storage capacity needed 
      - The security enabled PCE administrator group 
      - The security enabled PCE user group 

## Managing Environments 
Dataverse security is another area that has a steep learning curve. Be prepared to spend time reading up on Microsoft Learn and other resources and then develop your security plan before starting to add business units, teams, and roles to your Premium Environment. 
  - Familiarize administrators with Dataverse Security: https://learn.microsoft.com/en-us/powerplatform/admin/wp-security  
  - The AMC PCE is for Command Apps that solve AMC problems and move AMC towards achieving innovative goals 
    - Solutions should not consume Premium Capacity if the core focus does not contribute to the conditions listed for solution registration  
  - Consider that AMC Premium Capacity storage is pooled at the Army tenant level with other MACOMs and other AMC Major Subordinate Commands 
    - It is incumbent upon AMC organizations to be conservative and good stewards with data consumption 
    - Delete deprecated solutions and Dataverse tables where applicable to release capacity back to the AMC environments 
    - Select minimum capacities for environments as AMC PCE Administrators can increase  those capacities when necessary 
    - Do not create excessive numbers of tables compared to the actual need of a requirement 
    - Do not build solutions in an AMC PCE that are better suited to leverage MS Teams Dataverse capacity 
    - Do not build solutions in an AMC PCE that are better suited to leverage SharePoint lists and libraries for unique, local, singular staff processes 

## Developer Environments 
The developer environment is where solutions are initially built by an organization and checked for feasibility of use. Not all solutions will proceed past the developer stage. Administrators should release those resources upon determination of adoption accordingly. 

## Test Environments 
The test environment is where developers should test changes and refined versions of developed solutions while only interacting with non-production data and invited test users. 

## Production Environments 
The production environments are for fully developed and refined solutions that will connect to, consume, or manipulate live production data. The solutions and data are available to real world Army processes and impact Army operations. 