# Non-functional requirements

### Usability

* Tools should be accessible to non-technical users
* Web content or software must meet WCAG 3.0 AA standards for accessibility
* Development needs to include i18n standards for internationalization

### Scalability

* To establish the legitimacy of the proposals, there must be sufficient participation. We expect tools would need to support at least:
  * 250,000 concurrent users if built for ada holders or GA submitters
  * 10,000 concurrent users if built for DReps
  * 2,000 concurrent users if built for SPOs

### Performance

* Responsiveness of the tool. Front page load time must be no longer than 2 seconds for users accessing the website using an LTE mobile connection

### IP rights

* The work must be open source with an open source license that permits the assets to be changed, redistributed, and used commercially (suggested: Apache 2.0 for code and CC BY 4.0 for other documents and assets)
* Any third party dependencies must not hinder the assets from being changed, redistributed, and used commercially
* The assets created for this proposal are universally accessible on a public repository by the time the project has completed
* Any code created for this proposal must migrate into Intersect’s repositories if requested by Intersect.

## Open-source requirements

* Intersect’s Open Source Committee is defining its open source best practices. In the meantime, the examples below (sourced from Intersect member, IOG) can be referenced:
  * [Cardano Engineering Handbook](https://github.com/input-output-hk/cardano-engineering-handbook/tree/main)
  * Guidance related to [open source policy can be referenced here](https://github.com/input-output-hk/cardano-engineering-handbook/tree/main/policy)

Guidance related to expected [best practices can be referenced here](https://github.com/input-output-hk/cardano-engineering-handbook/tree/main/practices)

## For Tools being proposed for direct integration into the existing Voltaire governance tooling system

Some proposed solutions may be appropriate for direct integration into the Voltaire governance tooling system. Adding a new space for ada holders to communicate with their DRep, for example.  For these tools, additional requirements apply:

* The tool should be built using a compatible tech stack where applicable, make use of the existing [design system](https://www.figma.com/file/8MJHuaTfHGLnuicZuXquA6/Voltaire-Design-System?type=design\&node-id=47%3A2\&mode=design\&t=z0giIZJfHLnZyDIy-1), and be developed (or transferable) into the open repos that will be made available ahead of development.
* The ultimate objective is for these tools to appear to the user as one solid application with an end-to-end experience of all the steps needed to participate in Cardano governance. Tools will share the same look & feel but will consist of micro-frontends with the actual code for each tool or service maintained in separate folders or repos.
* [This short video ](https://www.loom.com/share/36f328c87ea147c18221d90b2019ad97?sid=b308d27f-c94f-4377-9f4b-54e47494f70f)shows what is currently implemented in the Voltaire governance tooling system and how to apply the existing [design system](https://www.figma.com/file/8MJHuaTfHGLnuicZuXquA6/Voltaire-Design-System?type=design\&node-id=47%3A2\&mode=design\&t=z0giIZJfHLnZyDIy-1). A front-end library documented in Storybook with key-built components will also be provided.

### Technical requirements for front end (to ensure integration)

* NextJS / React
* Material UI
* (optional if applicable) Axios

### Deployment and environment requirements

* Run separate development and testing environments for the duration of development.
* Other guidance related to deployment environment requirements will be provided.
