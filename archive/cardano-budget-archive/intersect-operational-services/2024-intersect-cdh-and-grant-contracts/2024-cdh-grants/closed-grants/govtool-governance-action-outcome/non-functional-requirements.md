# Non Functional Requirements

{% include "../../../../../../../.gitbook/includes/this-page-has-been-archived.md" %}

### Usability

* This section should be accessible to non-technical users
* This section should be transparent and easy to engage
* Meet WCAG 3.0 AA standards for accessibility
* Development needs to include i18n standards for internationalization

### Scalability

* We expect this tool would need to support at least 250,000 concurrent users

### Performance

* Responsiveness of the tool: Front page load time must be no more than 2 seconds for users that access the website using an LTE mobile connection

### Open source requirements

* Key open source requirements:
  * The section needs to follow the same apache 2.0 of the overall govtool
  * The applicant accepts to create full documentation to allow open contribution
* Use the following boilerplate:
  * [https://github.com/IntersectMBO/web-app-boilerplate-template](https://github.com/IntersectMBO/web-app-boilerplate-template)

### Technical specification requirements for FE and BE (to ensure integration)

* NodeJS backend
* NextJS frontend
* “Voltaire” Design System based on material UI
* (optional if applicable) Axios

### IP rights

* The code must be open source with an open source license that permits the assets to be changed, redistributed, and used commercially (suggested: Apache 2.0 for code and CC BY 4.0 for other documents and assets)
* Any third party dependencies must not hinder the assets from being changed, redistributed and used commercially
* The assets created for this proposal are universally accessible on a public repository by the time the project has completed
* The assets created for this proposal must migrate into Intersect’s repositories if requested by Intersect

### Deployment and environment requirements

* Other guidance related to deployment, environments requirements will be provided to ensure integration with GovTool
