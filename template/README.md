![Logo of the project](https://raw.githubusercontent.com/jehna/readme-best-practices/master/sample-logo.png)

# <%= projectName %>

[![Latest Version](https://img.shields.io/npm/v/<%= projectName %>/latest.svg)](https://www.npmjs.com/package/<%= projectName %>)
[![Next Version](https://img.shields.io/npm/v/<%= projectName %>/next.svg)](https://www.npmjs.com/package/<%= projectName %>)
[![Beta Version](https://img.shields.io/npm/v/<%= projectName %>/beta.svg)](https://www.npmjs.com/package/<%= projectName %>)
<% if (projectPrerequisites) { -%>
<% projectPrerequisites.map(({ name, value }) => { -%>
![Prerequisite](https://img.shields.io/badge/<%= name %>-<%= encodeURIComponent(value) %>-blue.svg)
<% }) -%>
<% } -%>
<% if (projectDocumentationUrl) { -%>
[![Documentation](https://img.shields.io/badge/docs-yes-brightgreen.svg)](<%= projectDocumentationUrl %>)
[![Documentation](https://inch-ci.org/github/<%= authorGithubUsername %>/<%= projectName %>.svg?branch=master)](https://inch-ci.org/github/<%= authorGithubUsername %>/<%= projectName %>?branch=master)
<% } -%>
<% if (isGithubRepos) { -%>
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](<%= repositoryUrl %>/graphs/commit-activity)
<% } -%>
[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](#-contributing)
<% if (licenseName) { -%>
[![License: <%= licenseName %>](https://img.shields.io/<%= isGithubRepos ? `github/license/${authorGithubUsername}/${projectName}` : `badge/License-${licenseName}-blue.svg` %>)](<%= licenseUrl ? licenseUrl : '#' %>)
<% } -%>
[![Package Size](https://img.shields.io/bundlephobia/min/<%= projectName%>)](https://bundlephobia.com/result?p=<%= projectName %>)

<% const codeClimateBadgeId = 'eaaa39ef8e79f8d2805a' -%>

[![Build Status](https://travis-ci.org/<%= authorGithubUsername %>/<%= projectName %>.svg?branch=master)](https://travis-ci.org/<%= authorGithubUsername %>/<%= projectName %>)
![Dependencies](https://david-dm.org/<%= authorGithubUsername %>/<%= projectName %>.svg)
[![Known Vulnerabilities](https://snyk.io/test/github/<%= authorGithubUsername %>/<%= projectName %>/badge.svg)](https://snyk.io/test/github/<%= authorGithubUsername %>/<%= projectName %>)
[![codecov](https://codecov.io/gh/<%= authorGithubUsername %>/<%= projectName %>/branch/master/graph/badge.svg)](https://codecov.io/gh/<%= authorGithubUsername %>/<%= projectName %>)
[![Total alerts](https://img.shields.io/lgtm/alerts/g/<%= authorGithubUsername %>/<%= projectName %>.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/<%= authorGithubUsername %>/<%= projectName %>/alerts/)
[![Language grade: JavaScript](https://img.shields.io/lgtm/grade/javascript/g/<%= authorGithubUsername %>/<%= projectName %>.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/<%= authorGithubUsername %>/<%= projectName %>/context:javascript)
[![Maintainability](https://api.codeclimate.com/v1/badges/<%= codeClimateBadgeId %>/maintainability)](https://codeclimate.com/github/<%= authorGithubUsername %>/<%= projectName %>/maintainability)

---

<% if (projectDescription) { -%>

<!--
One-liner explaining the purpose of the module
-->

<%= projectDescription %>

<% } -%>

#### <% -%>

<% if (projectHomepage) { -%>

🏠 [Homepage](<%= projectHomepage %>) | <% -%>

<% } -%>

🗃 [Repository](https://github.com/<%= authorGithubUsername %>/<%= projectName %>) |
📦 [NPM](https://www.npmjs.com/package/<%= projectName %>) <% -%>

<% if (projectDocumentationUrl) { -%>

| 📚 [Documentation](<%= projectDocumentationUrl %>) <% -%>

<% } -%>

<% if (issuesUrl) { -%>

| 🐛 [Issue Tracker](<%= issuesUrl %>) <% -%>

<% } -%>

## 🪑 Table of Content

- [🧰 Features](#-features) <% if (projectDemoUrl) { -%>
- [✨ Demo](#-demo) <% } -%> <% if (projectPrerequisites && projectPrerequisites.length) { -%>
- [🚦 Prerequisites](#-prerequisites) <% } %>
- [👶 Install](#-install)
- [🚀 Usage](#-usage)
- [🔮 Background](#-background)
- [🤖 API](#-api)
- [⏳ Changelog](#-changelog)
- [🛠 Developing](#-developing)
- [🏗 Roadmap](#-roadmap)
- [🤝 Contributing](#-contributing)
- [🧙 Contributors](#-contributors)
- [⭐ Show your support](#-show-your-support)
- [🐙 Community](#-community)
- [🔗 Related Projects](#-related-projects)
- [👨‍🔧 Maintainers](#-maintainers)
- [📝 License](#-license)

## 🧰 Features

<!--
A brief description of your project, what it is used for and how does life get
awesome when someone starts to use it.

- Note and briefly describe any key concepts (technical, philosophical, or both) important to the user’s understanding.
- Link to any supplementary blog posts or project main pages.
- State if it is out-of-the-box user-friendly, so it’s clear to the user.
- List its most useful/innovative/noteworthy features.
- State its goals/what problem(s) it solves.
-->

What's all the bells and whistles this project can perform?

- What's the main functionality
- You can also do another thing
- If you get really randy, you can even do this

<% if (projectDemoUrl) { -%>

<!--
- If possible, include screenshots and demo videos.
-->

## ✨ [Demo](<%= projectDemoUrl %>)

<% } -%>

<% if (projectPrerequisites && projectPrerequisites.length) { -%>

## 🚦 Prerequisites

<% projectPrerequisites.map(({ name, value }) => { -%>

- <%= name %> <%= value -%>

<% }) -%>

<% } -%>

<% if (installCommand) { -%>

## 👶 Install

<!--
- Getting it
- Installing It
- Configuring It
- Running it
-->

```sh
<%= installCommand %>
```

<% } -%>

<% if (usage) { -%>

## 🚀 Usage

<!-- Clear, _runnable_ example of usage -->

```sh
<%= usage %>
```

### Typing

This project is written in TypeScript and the typings are included in the distribution.

### Debugging

This project uses [debug](https://www.npmjs.com/package/debug). To show debug logs, activate debug for `<%= projectName%>`.

CLI example:

```sh
DEBUG=<%= projectName%> node path/to/my/<%= projectName%>-project
```

<% } -%>

## 🔮 Background

<!-- Core Technical Concepts/Inspiration

- Potentially unfamiliar terms link to informative sources
- Why does it exist?
- Frame your project for the potential user.
- Compare/contrast your project with other, similar projects so the user knows how it is different from those projects.
- Highlight the technical concepts that your project demonstrates or supports. Keep it very brief.
- Keep it useful.
- Performs [cognitive funneling](https://github.com/noffle/art-of-readme#cognitive-funneling)
- Caveats and limitations mentioned up-front

-->

## 🤖 API

TypeDoc documentation can be [found here](https://github.com/<%= authorGithubUsername %>/<%= projectName %>/blob/master/docs/typedoc/README.md).

## ⏳ Changelog

This projects follows semantic versioning. The
[changelog can be found here](https://github.com/<%= authorGithubUsername %>/<%= projectName %>/blob/master/CHANGELOG.md).

## 🛠 Developing

If you want to contribute to the project or forked it,
[this guide will get you up and going](https://github.com/<%= authorGithubUsername %>/<%= projectName %>/blob/master/docs/developing.md).

## 🏗 Roadmap

- Next steps
- Features planned
- Known bugs (shortlist)

OR

This package is considered feature-complete. However, if you have ideas how it
could be improved, please be sure to share it with us by [opening an issue](#🤝-contributing).

## 🤝 Contributing

Contributions, issues and feature requests are welcome! Thank you ❤️

<% if (issuesUrl) { -%>

Feel free to dive in! See [current issues](<%= issuesUrl %>),
[open an issue](<%= issuesUrl %>/new), or [submit PRs](https://github.com/<%= authorGithubUsername %>/<%= projectName %>/compare).

<% } -%>

<%= contributingUrl ? `How to report bugs, feature requests, and how to contribute and what conventions we use is all described in the [contributing guide](${contributingUrl}).` : '' %>

When contributing we follow the
[Contributor Covenant](https://contributor-covenant.org/version/1/3/0/).
See our [Code of Conduct](https://github.com/<%= authorGithubUsername %>/<%= projectName %>/blob/master/docs/CODE_OF_CONDUCT.md).

## 🧙 Contributors

Contributions of any kind welcome. Thanks goes to these wonderful people ❤️

### Recent and Top Contributors

<!-- Hall of Fame uses 8 links (7 users + 1 stats), see https://github.com/sourcerer-io/hall-of-fame#faq -->

<% const hallOfFameLinksNum = 8; %>
<% const sourcererUsername = 'JuroOravec'; %>

<% Array(8).fill().forEach((v, index) => { -%>
[![Hall of Fame Contributor <%= index + 1 %>](https://sourcerer.io/fame/<%= sourcererUsername %>/<%= authorGithubUsername %>/<%= projectName %>/images/<%= index %>)](https://sourcerer.io/fame/<%= sourcererUsername %>/<%= authorGithubUsername %>/<%= projectName %>/links/<%= index %>)
<% }) %>

<!-- markdownlint-disable -->

<sub><em>Generated using [Hall of Fame](https://github.com/sourcerer-io/hall-of-fame#readme).</em></sub>

<!-- markdownlint-enable -->

### All Contributors

Contribution type [emoji legend](https://allcontributors.org/docs/en/emoji-key)

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->

_No additional contributors. Be the first one!_

<!-- ALL-CONTRIBUTORS-LIST:END -->

<!-- markdownlint-disable -->

<sub><em>This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification.</em></sub>

<!-- markdownlint-enable -->

## ⭐ Show your support

Give a ⭐️if this project helped you!

<% if (authorPatreonUsername) { -%>

<a href="https://www.patreon.com/<%= authorPatreonUsername %>">
  <img src="https://c5.patreon.com/external/logo/become_a_patron_button@2x.png" width="160">
</a>

<% } -%>

## 🐙 Community

- [Stack Overflow](https://stackoverflow.com/questions/tagged/<%= projectName %>)
- [Quora](https://www.quora.com/search?q=%22<%= projectName %>%22)
- [Spectrum community](https://spectrum.chat/<%= projectName %>)

## 🔗 Related Projects

- e.g. If I make plugin I might want to link to them

<% if (authorName || authorTwitterUsername || authorGithubUsername) { -%>

## 👨‍🔧 Maintainers

<% if (authorName) { %>

👤 **<%= authorName %>**

<% } %>

<% if (authorWebsite) { -%>

- Website: <%= authorWebsite -%>

<% } -%>

<% if (authorTwitterUsername) { -%>

- Twitter: [@<%= authorTwitterUsername %>](https://twitter.com/<%= authorTwitterUsername %>) <% -%>

<% } -%>

<% if (authorGithubUsername) { -%>

- GitHub: [@<%= authorGithubUsername %>](https://github.com/<%= authorGithubUsername %>) <% -%>

<% } -%>

<% if (authorLinkedInUsername) { -%>

- LinkedIn: [@<%= authorLinkedInUsername %>](https://linkedin.com/in/<%= authorLinkedInUsername %>) <% -%>

<% } -%>

- Sourcerer: [@<%= authorGithubUsername %>](https://sourcerer.io/<%= authorGithubUsername%>)

<% } %>

<% if (licenseName && licenseUrl) { -%>

## 📝 License

<% if (authorName && authorGithubUsername) { -%>

Copyright © <%= currentYear %> [<%= authorName %>](https://github.com/<%= authorGithubUsername %>).

<% } -%>

This project is [<%= licenseName %>](<%= licenseUrl %>) licensed.

<% } -%>
