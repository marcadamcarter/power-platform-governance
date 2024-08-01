# Scenario 5: Supporting team development
Supporting team development consists of multiple apps and development team members in a structured release management process. Team development includes the following: 

-   **Conflict and merge resolution** It's important to consider which pieces will merge well and which should only be worked on by a single developer at a time, such as forms or site maps. More information: [Understand how managed solutions are merged](https://learn.microsoft.com/en-us/power-platform/alm/how-managed-solutions-merged)

-   **Branching strategy** Your branching strategy should make sure that you can
    service an existing release while working on the next version.

-   **Environment strategy** Developer isolation, and an environment strategy that
    supports it, is critical when multiple developers work on the same
    application. Environments should be short-lived and spun up on demand from
    the latest build. Each developer should have their own development environment
    in which only the required unmanaged solution is installed, and all dependent
    solutions are installed as managed.

-   **Power Apps component library** Components are reusable building blocks for canvas apps so that app makers can create custom controls to use inside an app, or across apps using the component library. More information: [Component library](https://learn.microsoft.com/en-us/powerapps/maker/canvas-apps/component-library) 

### See also
[Scenario 6: Embrace your citizen developers in the ALM process](embrace-citizen-devs.md)

## References
  - [https://learn.microsoft.com/en-us/power-platform/alm/team-development-alm](https://learn.microsoft.com/en-us/power-platform/alm/team-development-alm)
