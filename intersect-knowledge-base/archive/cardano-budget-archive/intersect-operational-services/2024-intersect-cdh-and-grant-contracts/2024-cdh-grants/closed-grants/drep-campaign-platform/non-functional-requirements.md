# Non-functional requirements

{% include "../../../../../../../.gitbook/includes/this-page-has-been-archived.md" %}

### Usability

* The DRep campaign platform should be accessible to non-technical users
* Proposal discussions should be transparent and easy to engage with
* Meet WCAG 3.0 AA accessibility standards
* Support for i18n/localization

### Scalability

* There must be enough participation to establish the legitimacy of the DRep campaign process. The tool would need to support at least 250,000 concurrent users.

### Performance

* Tool responsiveness: front page must load within 2 seconds for users accessing the website using an LTE mobile connection

### IP rights

* The code must be open source, with an open source license that permits the assets to be changed, redistributed, and used commercially (suggested: Apache 2.0 for code and CC BY 4.0 for other documents and assets)
* Any third party dependencies must not hinder or prevent the assets from being changed, redistributed, and used commercially
* The assets created for this proposal will be universally accessible on a public repository by the time the project is complete
* The assets created for this proposal must migrate into Intersect’s repositories if requested by Intersect

### Open source requirements

* While this instance is unique to the ways of working to Intersect member, IOG, open source best practice can be referenced from here: [Cardano Engineering Handbook](https://github.com/input-output-hk/cardano-engineering-handbook/tree/main)
* Guidance related to [open source policy can be referenced here](https://github.com/input-output-hk/cardano-engineering-handbook/tree/main/policy)
* Guidance related to expected [best practices can be referenced here](https://github.com/input-output-hk/cardano-engineering-handbook/tree/main/practices)

### Technical specification recommendations for FE (to support integration)

* NextJS / React
* Material UI
* i18next (or equivalent. New version support i18n without additional plugin)
