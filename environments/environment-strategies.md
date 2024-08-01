# Environment Strategies
Microsoft structures its Power Platform environments into three broader categories that cover seven use cases, reflecting varying degrees of risk and control: 
  - **Personal productivity** - This is for someone who just wants to build an app or flow for themselves. For example, they aren't collaborating with others.
  - **Team collaboration** – This is for users who are building tooling, automation, and processes for their team. For this scenario, Microsoft encourages the use of Dataverse for Teams environments. Lifecycle, access management, and data labeling are controlled at the Microsoft 365 group-level so we don't have to spend the time managing these users from a Power Platform governance perspective. This level of use is the next step up in the risk spectrum.
  - **Enterprise development/production-level used by all employees** – These are people building tooling or solutions used more broadly across the company. These environments may store the most sensitive data, use more powerful connectors, and require more governance. This is considered the highest risk and most effort is spent on governance. ALM is required, with preproduction work happening in sandbox environments and only managed solutions are allowed within production environments. Many environment groups and rules are used to manage and control these environments.

## Communicate your environment strategy to your organization

You implement your tenant environment strategy more successfully if your Power Platform users understand and are aligned with what you're trying to achieve. If you simply activate your strategy without any communication, users see the changes as restrictions and look for ways to work around them.

As part of developing or evolving your strategy, decide how you inform users of key elements of the strategy that affect their use of Power Platform. **They don't need all the technical details of your strategy, only the essentials that help ensure that they remain productive, such as:**

- The purpose of the default environment
- Where they should build new low-code assets
- How they should use their personal developer environment
- How to request custom environments for specific business units or projects
- How to share what they build with others
- The responsibilities of a maker; for example:
    - Keep the tenant clean. Delete your environments, apps, and flows if they're no longer needed. Use test environments if experimenting.
    - Share wisely. Watch out for oversharing of your environments, apps, flows, and shared connections.
    - Protect organization data. Avoid moving data from highly confidential or confidential data sources to unprotected storage.
- When your strategy changes, share how the changes affect your users so that they know what to do differently

Another effective approach to communicating with your users is establishing an internal Power Platform hub. The hub can be a place for people to collaborate on projects, share ideas, and discover new ways to apply technology to achieve more. The hub could be where you share more detailed information on your environment strategy that's relevant to your users. [Learn how to create an internal Power Platform hub](https://learn.microsoft.com/en-us/power-platform/guidance/adoption/wiki-community).


## Considerations - New environments

As part of developing your strategy, consider when you create environments to support a workload. Your evaluation must balance the benefits of isolation that an environment provides&mdash;for example, being able to lock down particular environments more than others is helpful from a security perspective&mdash;with the disadvantages, such as that isolation creates friction for users who try to share data across apps.

When you're evaluating whether an app or an automation belongs in its own environment.  When multiple apps are developed in a single environment, you risk creating cross-app dependencies.

Testing multiple apps in the same environment makes sense if they run together in production. In fact, if you don't test with the apps that will be running in production, you risk not discovering compatibility problems.

When you evaluate the production environment for an app, keep the following considerations in mind:

- Each environment (besides trial and developer environments) **consumes 1 GB to initially provision**.
- **Is the app compatible with existing apps in the environment?** For example, two apps that both use the Dataverse Contact table for different purposes might not be compatible. Are the apps compatible from a DLP policy perspective?
- **Are there special compliance or regulatory requirements for separation of data?** For example, does the sensitivity of the data require it to be isolated? Is there a requirement that data can't be included with other data?
- **Is the data highly confidential or sensitive? Would exfiltration cause monetary or reputational damage to the organization?** Isolating in a separate environment can allow for more control over security.
- **Does the app need data from other apps and need to be collocated with them?** For example, two apps that both use your Customer table should be hosted together. Separating them would create redundant, data copies and create problems with maintaining the data.
- **Will new admins be needed, or will the existing admins be sufficient?** If the new app requires more admins, are they compatible with the existing admins because all of them will have admin permissions on all apps in the environment.
- **What's the life expectancy of the app?** If the app or automation is temporary or short-lived, it might not be a good idea to install it in an environment with more permanent apps.
- **Will users have difficulty having to use multiple environments for different apps?** This can affect everything from finding an app on their mobile device to self-service reporting that has to pull data from multiple environments.

## Scenario 1: Standardized (Developer, Sandbox, and Production) Environments at each MSC and Subordinate Unit
![Baseline-environments](/media/baseline-environments.png)

## References
  - [https://learn.microsoft.com/en-us/power-platform/guidance/white-papers/environment-strategy](https://learn.microsoft.com/en-us/power-platform/guidance/white-papers/environment-strategy)

