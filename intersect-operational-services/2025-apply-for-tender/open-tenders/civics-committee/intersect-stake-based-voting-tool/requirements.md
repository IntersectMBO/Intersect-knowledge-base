# Requirements

### Functional requirements

* CIP-30 for wallet connectivity

### Non-functional requirements

#### Usability

* This section should be accessible to non-technical users
* This section should be transparent and easy to engage
* Meet WCAG 3.0 AA standards for accessibility
* Development needs to include i18n standards for internationalization

#### **Scalability**

* We expect this tool would need to support at least 250,000 concurrent users

#### Performance

* Responsiveness of the tool: Front page load time must be no more than 2 seconds for users that access the website using an LTE mobile connection

#### Open source requirements

Key open source requirements

1. The section needs to follow the same apache 2.0 of the overall govtool
2. The applicant accepts to create full documentation to allow open contribution

#### IP rights

* The code must be open source with an open source license that permits the assets to be changed, redistributed, and used commercially (suggested: Apache 2.0 for code and CC BY 4.0 for other documents and assets)
* Any third party dependencies must not hinder the assets from being changed, redistributed and used commercially
* The assets created for this proposal are universally accessible on a public repository by the time the project has completed
* The assets created for this proposal must migrate into Intersect’s repositories if requested by Intersect

### Optional functions

* Admin dashboard to create voting events and set up the criteria
* Admin dashboard to track the voting events with key metrics such as participation based on stake&#x20;
* [Post results on-chain automatically](https://github.com/cardano-foundation/cf-cardano-ballot/blob/main/backend-services/voting-admin-app/EVENT_REGISTRATION.md)
* Be handled on a side chain
* The snapshot should be limited to voters who delegated to a DRep
* Support for multi-language
* If possible, use the style used in the design system used for Govtool
