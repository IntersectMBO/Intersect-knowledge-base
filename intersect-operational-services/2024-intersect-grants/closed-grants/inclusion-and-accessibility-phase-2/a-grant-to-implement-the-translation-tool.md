# A Grant to implement the translation tool

{% hint style="info" %}
This grant Part 1 is now closed&#x20;
{% endhint %}

## Context

Govtool and Constitutional Committee Portal frontend are built on top of NextJS stack which has full I18n support since version 10. The i18n routing support is currently meant to complement existing i18n library solutions like react-intl, react-i18next, lingui, rosetta, next-intl, next-translate, next-multilingual, tolgee, inlang and others by streamlining the routes and locale parsing.\
\
The internationalization (and translations) work by providing the list of locales, the default locale and domain-specific locales, and the tech stack will automatically handle the routing.

The frontend stack itself is already configured as explained above. Now we need the community contributors to work on the translations and internationalization files holding key-value pairs of strings used across the interface. The default en-UK version will be provided.\
\
In order to provide the right tooling to community contributors to work on the translations, we need to implement a Translation Management system. Translized, Smartling, Localize or similar OR we can leverage from newer AI tooling.\
\
Solutions like Poedit offer online translations tools which can be integrated into our frontends so that users themselves can suggest better translations maintaining the context of written word in different languages.

## Functional Requirements

The successful applicant will be required to deploy Poedit, the localisation management system, and configure it to support GovTool translations and localisations to selected languages. The successful applicant will integrate Poedit with the Intersect GitHub account to more easily manage the localization of language files hosted on GitHub. Initially, the successful applicant will be required to use Automatic Translation feature which will allow us to use machine translation engines from Google, Microsoft and DeepL.\
\
Once configured, the tool will be used by contributors to work on the translations in selected languages.

## Budget

This grant is for 5,000 ADA.
