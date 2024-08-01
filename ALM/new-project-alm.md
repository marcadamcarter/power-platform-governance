# Scenario 0: ALM for a new project
If you're new to Power Apps and creating your first app, follow the
tasks described in this article to successfully deploy a functioning application to your production environment using a healthy application lifecycle management (ALM) strategy.

| Task  | Description |
|-------|-------------|
| 1. Plan and implement your environment strategy.| Determining the environments you'll need and establishing an appropriate governance model is a critical first step. At a minimum, you should have two environments: dev and production. However, we recommend that you have three environments: dev, test, and production. |
| 2. Create a solution and publisher.| Start with a blank solution, and create a custom publisher for that solution.|
| 3. Set up your DevOps project.  | Set up a DevOps project in which you'll later add several pipelines to perform required processing like export and deployment of your solution. |
| 4. Create your export from development pipeline in DevOps. | Create a DevOps pipeline to export your completed unmanaged solution to a managed solution.|
| 5. Configure and build your app.  | Create your app within the solution you created.|
| 6. Add any additional customizations to that solution.  | Add additional components as needed. Choose from a vast selection of components, such as flows, AI models, export to data lake configuration, web resources, plug-ins, and even other apps.|
| 7. Create a deployment pipeline in DevOps. | Create a DevOps pipeline to deploy your managed solution to one or more target production environments.|
| 8. Grant access to the app.  | Assign licensing and assign security roles to share applications with users.|

### See also
[Scenario 1: Citizen development (app and flow makers)](citizen-dev-alm.md)

## References
  - [https://learn.microsoft.com/en-us/power-platform/alm/new-project-alm](https://learn.microsoft.com/en-us/power-platform/alm/new-project-alm)
