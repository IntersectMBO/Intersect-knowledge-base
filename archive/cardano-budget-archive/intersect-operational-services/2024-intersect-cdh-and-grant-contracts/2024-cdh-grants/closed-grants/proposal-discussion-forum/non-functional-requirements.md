# Non-functional requirements

{% include "../../../../../../../.gitbook/includes/this-page-has-been-archived.md" %}

## Minimum non-functional requirements

The Proposal Discussion Forum will be a pillar of the Voltaire governance tooling system. This means that it should be built using a compatible tech stack where applicable, make use of the existing design elements (design library to be provided), and be developed (or transferable) into the open repos that will be made available ahead of development.

The ultimate objective is for these tools to appear to the user as one solid application with an end-to-end experience of all the steps needed to participate in Cardano governance. Tools will share the same look & feel, but will consist of micro-frontends with the actual code for each tool or service maintained in separate folders or repos.

Context can be found in [this initial visualization](https://www.figma.com/file/239JKpjintphf2Go5NPipp/Proposal-discussion-Forum?type=design\&node-id=0%3A1\&mode=design\&t=anh7vIBCkE3MxzUD-1), which gives initial ideas of how to use the [design system](https://www.figma.com/file/8MJHuaTfHGLnuicZuXquA6/Voltaire-Design-System?type=design\&node-id=47%3A2\&mode=design\&t=z0giIZJfHLnZyDIy-1) and how to integrate with the existing functions. [This short video ](https://www.loom.com/share/36f328c87ea147c18221d90b2019ad97?sid=b308d27f-c94f-4377-9f4b-54e47494f70f)shows what is currently implemented in the Voltaire governance tooling system.

### Usability

* The proposal discussion forum should be accessible to non-technical users
* Proposal discussions should be transparent and easy to engage
* Meet WCAG 3.0 AA standards for accessibility
* Development needs to include i18n standards for internationalization

### Scalability

* In order to establish the legitimacy of the proposals, there must be sufficient participation so we expect this tool would need to support at least 250,000 concurrent users

### Performance

* Responsiveness of the tool: Front page load time must be no more than 2 seconds for users that access the website using an LTE mobile connection

### Open source requirements

* Guidance related to open source requirements will be provided
* Guidance related to expected best practices to follow will be provided

### Technical specification requirements for FE (to ensure integration)

* NextJS / React
* Material UI
* (optional if applicable) Axios

### IP rights

* The code must be open source with an open source license that permits the assets to be changed, redistributed, and used commercially (suggested: Apache 2.0 for code and CC BY 4.0 for other documents and assets)
* Any third party dependencies must not hinder the assets from being changed, redistributed and used commercially
* The assets created for this proposal are universally accessible on a public repository by the time the project has completed
* The assets created for this proposal must migrate into Intersect’s repositories if requested by Intersect

### Deployment and environment requirements

* Run separate development and testing environments for the duration of development
* Other guidance related to deployment, environments requirements will be provided
