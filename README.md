# chonky-node-template

<!-- [![Latest Version](https://img.shields.io/npm/v/chonky-node-template/latest.svg)](https://www.npmjs.com/package/chonky-node-template) -->

[![Documentation](https://img.shields.io/badge/docs-yes-brightgreen.svg)](https://github.com/JuroOravec/chonky-node-template/tree/master/docs)
[![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](#-contributing)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://tldrlegal.com/license/mit-license)

<!-- [![Package Size](https://img.shields.io/bundlephobia/min/chonky-node-template)](https://bundlephobia.com/result?p=chonky-node-template) -->
<!-- [![Build Status](https://travis-ci.org/JuroOravec/chonky-node-template.svg?branch=master)](https://travis-ci.org/JuroOravec/chonky-node-template) -->

![Dependencies](https://david-dm.org/JuroOravec/chonky-node-template.svg)
[![Known Vulnerabilities](https://snyk.io/test/github/JuroOravec/chonky-node-template/badge.svg)](https://snyk.io/test/github/JuroOravec/chonky-node-template)
[![Total alerts](https://img.shields.io/lgtm/alerts/g/JuroOravec/chonky-node-template.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/JuroOravec/chonky-node-template/alerts/)

<!-- [![codecov](https://codecov.io/gh/JuroOravec/chonky-node-template/branch/master/graph/badge.svg)](https://codecov.io/gh/JuroOravec/chonky-node-template) -->

<!-- [![Language grade: JavaScript](https://img.shields.io/lgtm/grade/javascript/g/JuroOravec/chonky-node-template.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/JuroOravec/chonky-node-template/context:javascript) -->

<!-- [![Maintainability](https://api.codeclimate.com/v1/badges/97a773f115a7c7961e15/maintainability)](https://codeclimate.com/github/JuroOravec/chonky-node-template/maintainability) -->

---

<!--
One-liner explaining the purpose of the module
-->

Featureful template for an open-source GitHub-based
TypeScript-written Node package.

#### 🏠 [Homepage](https://github.com/JuroOravec/chonky-node-template#readme) | 🗃 [Repository](https://github.com/JuroOravec/chonky-node-template) | 📦 [NPM](https://www.npmjs.com/package/chonky-node-template) | 📚 [Documentation](https://github.com/JuroOravec/chonky-node-template/tree/master/docs) | 🐛 [Issue Tracker](https://github.com/JuroOravec/chonky-node-template/issues)

## 🪑 Table of Content

- [🧰 Features](#-features)
- [🚦 Prerequisites](#-prerequisites)
- [🚀 Usage](#-usage)
  - [Setup](#setup)
  - [Workflow](#workflow)
  - [Scripts](#scripts)
- [🔮 Background](#-background)
- [🤖 API](#-api)
- [⏳ Changelog](#-changelog)
- [🛠 Developing](#-developing)
- [🏗 Roadmap](#-roadmap)
- [🤝 Contributing](#-contributing)
- [🧙 Contributors](#-contributors)
- [⭐ Show your support](#-show-your-support)
- [🐙 Community](#-community) <!-- - [🔗 Related Projects](#-related-projects) -->
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

- Automated pipeline

  - Automated `CHANGELOG.md` updated on PR to master branch
    ([Semantic release](https://semantic-release.gitbook.io/semantic-release/))
  - Release to [NPM](https://www.npmjs.com/)
    and
    [GitHub](https://github.com/)
    on merge to master branch
    ([Semantic release](https://semantic-release.gitbook.io/semantic-release/))
  - Code analysis with
    [CodeCov](https://codecov.io/),
    [CodeClimate](http://codeclimate.com/),
    [LGTM](https://lgtm.com/).
  - Dependency management with
    [DependaBot](https://dependabot.com/).

- Security

  - Security analysis with
    [LGTM](https://lgtm.com/)
    and
    [Snyk](https://snyk.io/).
  - Secrets management.
  - Verified commits from CI / CD enviroment.

- Development

  - Written with [typescript](https://www.typescriptlang.org/)
  - Tests with [jest](https://jestjs.io/)
  - Logging with [debug](https://github.com/visionmedia/debug)

- Effective collaboration

  - Commit standardization and validation with
    [Commitizen](http://commitizen.github.io/cz-cli/),
    [Commitlint](https://commitlint.js.org/)
    and
    [Zappr](https://zappr.opensource.zalan.do/).
  - Formatting standardization with
    [ESLint](https://eslint.org/)
    and
    [prettier](https://prettier.io/)
  - Standardized
    [GitHub issues labels](https://github.com/JuroOravec/chonky-node-template/tree/master/docs/issue_labels.md)
    with automated setup.
  - [TypeDoc](https://typedoc.org/)
    documentation
  - Robust quality guards on pull requests ensured by mulitple bots and tests.

- Community-focused

  - Contributor recognition with
    [AllContributors](https://allcontributors.org/)
    and
    [Sourcer.io's Hall of Fame](https://github.com/sourcerer-io/hall-of-fame).
  - [Spectrum](https://spectrum.chat/)
    community for questions and discussions.
  - Contributing guides.
  - Community files like CONTRIBUTING, CODE_OF_CONDUCT, etc.
  - Detailed README with
    [readme-md-generator](https://github.com/kefranabg/readme-md-generator)
  - Follows initiatives like
    [Make a README](https://www.makeareadme.com/)
    and [Keep a CHANGELOG](https://keepachangelog.com/)

## 🚦 Prerequisites

### Environment

This template works in UNIX enviroment.

### Packages

To run the setup steps, you will need following packages installed:

- [git](https://git-scm.com/)
- [hub](https://hub.github.com/)
- [travis](https://github.com/travis-ci/travis.rb)
- [gpg](https://formulae.brew.sh/formula/gnupg)

### Services / Bots

The template uses following services or bots:

- [GitHub](https://github.com/)
- [Travis CI](https://travis-ci.org/)
- [CodeCov](https://codecov.io/)
- [Zappr](https://zappr.opensource.zalan.do/)
- [AllContributors](https://allcontributors.org/)
- [Snyk](https://snyk.io/)
- [CodeClimate](http://codeclimate.com/)
- [LGTM](https://lgtm.com/)
- [DependaBot](https://dependabot.com/)

## 🚀 Usage

### Setup

Steps to create a new project using this template.

1. Create new directory

   ```bash
   mkdir <project-name> && cd <project-name>
   ```

2. Initialize git and create GitHub repo.

   ```bash
   hub init && hub create
   ```

3. Copy this template into the dir (more on copying git repo w/o `.git`
   [here](https://stackoverflow.com/questions/3946538))

   ```bash
   mkdir temp && cd temp
   git clone https://github.com/JuroOravec/chonky-node-template.git
   mv {chonky-node-template/template/*,chonky-node-template/template/.*} ../
   rm -rf chonky-node-template
   cd ..
   ```

4. Make sure directories like `temp`, `coverage`, `dist`, `docs/typedoc`,
   `node_modules` are all empty

   ```bash
   find ./temp -mindepth 1 -delete
   find ./coverage -mindepth 1 -delete
   find ./dist -mindepth 1 -delete
   find ./docs/typedoc -mindepth 1 -delete
   find ./node_modules -mindepth 1 -delete
   ```

5. Optionally set git aliases defined in `./scripts/git`

   ```bash
   sh scripts/set_git_aliases.sh
   ```

6. `package.json`

   1. Fill in:

      1. Set `name`
      1. Set `description`
      1. Set `homepage`
      1. Set `repository`
      1. Set `bugs`
      1. Set `author.name`
      1. Set `author.email`
      1. Set `keywords`

7. Install dependencies

   ```bash
   npm install
   ```

8. `.env`

   1. Copy `.env.example` and rename it to `.env`

      ```bash
      cp ./.env.example .env
      ```

   2. Fill in the secrets

9. `LICENSE`

   1. Set year

   2. Set author name

10. Create issue labels on GitHub

    1. Create access token for `github-label-sync` named
       `<my-repo>/github-label-sync` and give it access to repo.

    2. Save the token to `.env` under `GITHUB_LABEL_SYNC_TOKEN`

    3. Save the token to secrets management service (e.g. LastPass).

    4. Run label sync wizard and enter required info.

       ```bash
       npm run labels:sync
       ```

11. CodeCov (config)

    1. Go to [CodeCov](https://codecov.io/gh) (or directly to
       `https://codecov.io/gh/<username>/<repo>`), add the new repo and its get
       token.

    2. Set `CODECOV_TOKEN` in `.env`

    3. Save the token to secrets management service (e.g. LastPass).

12. Zappr (`.zappr.yml` config)

    1. Set your username as maintainer in `zappr.yml`.

    2. Go to [Zappr](https://zappr.opensource.zalan.do/) and activate zappr for
       this project.

13. AllContributors (`.all-contributorsrc` config)

    1. Set project name (`projectName`)

    2. Set project owner (`authorGithubUsername`)

14. Snyk

    Taken from
    [this guide](https://blog.travis-ci.com/2017-04-20-continuous-security-snyk-travis-ci/).

    1. Setup Snyk.

       ```bash
       npx snyk wizard
       ```

       > If prompted whether to update the policy file or replace it, choose
       > replace.

       > Snyk commands are already in `package.json`, so when asked if they
       > should be added, say no.

       > If you're prompted to authenticate, run and follow command:
       >
       > ```bash
       > npx snyk auth
       > ```

    `snyk wizard` both patches and tests the dependencies. If later you need to
    do either of them, then:

    - Run `snyk:protect` to patch / update dependencies

      ```sh
      npm run snyk:protect
      ```

    - Run `snyk:test` to test vulnerabilities

      ```sh
      npm run snyk:protect
      ```

15. Travis (config)

    1. Set project name (`projectName`).

    2. Set project owner (`authorGithubUsername`).

16. Travis (bot)

    1. Set up Travis for the repo
       [here](https://travis-ci.org/account/repositories).
       - Make sure that CI builds run on both PR and push (check settings).
       - This must be done before following steps to be able to encrypt tokens.

17. Configure signed commits in Travis CI

    Taken from
    [the semantic-release guide](https://github.com/semantic-release/git/tree/905f113a577c55cd9bb0a37ea3504d9e8ee2dfa2#gpg-signature)

    1. Generate key. This can be done by either filling in a template file and
       passing that or step by step

       - From file:

         <!--  https://lists.gnupg.org/pipermail/gnupg-users/2007-February/030330.html -->

         1. Fill name, email, comment, and passphrase to
            `config/travis-ci/gen-key_template`

         2. Run `gpg --batch --gen-key config/travis-ci/gen-key_template`

         3. Run `rm config/travis-ci/gen-key_template`, or alternatively keep
            the file around a bit longer as we will still need the password later
            on.

       - From command line:

         1. Run GPG

            ```bash
            gpg --full-generate-key
            ```

            - Select `RSA and RSA`.

            - Select size `4096`.

            - Enter yout name, the email associated with your Git hosted
              account.

            - Set a long (e.g. 64) and hard to guess passphrase. Ideally use
              a reliable generator (e.g. keychain). Save the password to
              secrets management service (e.g. LastPass).

            - Set the GPG key comment to include the name of the project, e.g.
              `<my-repo>/travis-ci`

    2. Display the newly created key ID (16-letter sequence).

       ```bash
       gpg --list-secret-keys --keyid-format LONG
       ```

    3. Export the key

       ```bash
       gpg --armor --export XXXXXXXXXXXXXXXX
       ```

       > `XXXXXXXXXXXXXXXX` is the key ID sequence.

    4. Copy the key, beginning with `-----BEGIN PGP PUBLIC KEY BLOCK-----` and
       ending with `-----END PGP PUBLIC KEY BLOCK-----`

    5. Add the GPG key to your GitHub account.

    6. Save the key ID to secrets management service (e.g. LastPass), so you
       know which project the key belongs to (GitHub doesn't allow any
       comments).

    7. Encrypt and add following tokens / passwords to appropriate field in
       `travis.yml`

       ```bash
        travis encrypt GPG_PASSPHRASE=...
        travis encrypt GPG_KEY_ID=XXXXXXXXXXXXXXXX
        travis encrypt GIT_EMAIL=...
        travis encrypt GIT_USERNAME=<UserName>
        travis encrypt "GIT_COMMITTER_NAME=<Your Git Name>"
        travis encrypt GIT_COMMITTER_EMAIL=...
       ```

    8. Export keys:

       ```bash
       gpg --export -a XXXXXXXXXXXXXXXX > git_gpg_keys.asc
       gpg --export-secret-key -a XXXXXXXXXXXXXXXX >> git_gpg_keys.asc
       ```

       Encrypt the file for Travis

       ```bash
       travis encrypt-file git_gpg_keys.asc
       ```

       Paste the response to the appropriate place in `.travis.yml`.

       Finally move the encrypted keys to config direrctory.

       ```bash
       # Save the `git_gpg_keys.asc.enc` to `./config/travis-ci`
       mv git_gpg_keys.asc.enc config/travis-ci/git_gpg_keys.asc.enc
       ```

    9. Cleanup

       ```bash
       rm git_gpg_keys.asc
       ```

       If you haven't removed `config/travis-ci/gen-key_template` before, run

       ```bash
       rm config/travis-ci/gen-key_template
       ```

    > Notes:
    >
    > - Don't forget to update the line that goes like
    >   `- openssl aes-256-cbc...`
    >
    > - When updating the `before_install` script in `.travis.yml`, make
    >   sure that the line which goes like `- echo '/usr/bin/gpg...` that
    >   the command called is `/usr/bin/gpg` and NOT `/usr/bin/gpg2`.
    >
    > - Generate encrypted values with
    >   `travis encrypt MY_ENV_VAR=env_var_value`.
    >   `.travis.yml` already includes fields where the encrypted values
    >   should be pasted (look for `<paste your encrypted...`)

18. Add semantic release tokens to `.travis.yml`

    1. Add encrypted `NPM_TOKEN` to be able to release on NPM
       1. Go to `https://www.npmjs.com/settings/your-username/tokens` and
          generate Read and Publish token
       2. Run `travis encrypt NPM_TOKEN=<your token>` to encrypt the token and add it to
          `.travis.yml`
       3. Save the token to secrets manager so you can find out what the key
          relates to (NPM doesn't offer any way to save a note)
    2. Add encrypted `GH_TOKEN` to be able to release on GitHub
       1. Go to `https://github.com/settings/tokens` and generate new token
          with note `<project-name>/semantic-release` and repo access.
       2. Run `travis encrypt GH_TOKEN=<your token>` to encrypt the token and add it to
          `.travis.yml`

19. Add Snyk token to `.travis.yml`

    1. Add encrypted `SNYK_TOKEN` to be able to test / patch in CI.

       1. Go to `https://snyk.io/account/` and generate a token

       2. Encrypt the token and add it to `.travis.yml`

          ```bash
          travis encrypt SNYK_TOKEN=<your token>
          ```

       3. Add the token to `.env`

20. `CHANGELOG.md`

    1. Make sure it's empty at the beginning.

21. `README.md`

    1. Remove the inital README.md if there's any.

    2. Run README generator (the template uses [readme-md-generator](https://github.com/kefranabg/readme-md-generator)).

       ```bash
       npm run readme:init
       ```

       > Example of init arguments:
       >
       > - HTML - Prefer markdown version for compatibility
       > - Description - Default (one from `package.json`) should be good
       > - Homepage - Default (one from `package.json`) should be good
       > - Demo URL - Add if you have one
       > - Project Docs - `https://github.com/<username>/<repo>/tree/master/docs`
       > - Author Name - Default (one from `package.json`) should be good
       > - GitHub username - your username
       > - Website - Add if you have one
       > - Twitter username - Add if you have one
       > - LinkedIn username - Add if you have one
       > - Patreon username - Add if you have one
       > - License name - MIT
       > - License URL - If MIT, use `https://tldrlegal.com/license/mit-license`
       > - Issues page - `https://github.com/<username>/<repo>/issues`
       > - Contributing guide url - `https://github.com/<username>/<repo>/tree/master/docs/CONTRIBUTING.md`
       > - Install command - `npm install <project-name>`
       > - Usage command - You will want usage to be longer, so for now enter
       >   anything so the field won't be empty and relevant parts will be
       >   rendered
       > - Test command `npm test`

    3. Remove parts that don't apply to your project, e.g.:

       - Logo

       - Multiple ways of reporting relevant NPM versions is available. If
         using beta or next tags, include them, otherwise keep only the
         `@latest` tag.

       - Multiple types of documentation badges are available. If using
         language which
         is supported by Inch CI, use their badge, otherwise use the static
         one.

    4. Remove comments from the markdown, unless stated otherwise.

    5. Fix spacing and gaps.

       - `Homepage | Repository | Documentation | Issue Tracker` should be
         a single line.

       - Table of content if there are any.

       - Gaps between maintainers links.

    6. Update CodeClimate badge

       1. Go to `https://codeclimate.com/github/repos/new` and add the repo.

       2. Go to `https://codeclimate.com/github/<username>/<project-name>/builds`
          and navigate to repo settings > extras > badges.

       3. Copy the ID from the badge image url.

       4. Paste the ID to `Maintainability` badge in README.md

    7. Add contributors

       - With cli:

         ```bash
         npm run contributors:add <username> <contribution type>
         ```

       - With
         [AllContributors GitHub bot](https://allcontributors.org/docs/en/bot/usage)

    8. Update contributors table.

       - With cli:

         ```bash
         npm run contributors:generate
         ```

    9. Update any missing links.

       - Changelog?
       - Code of Conduct link?
       - Open an Issue link?
       - Open a PR link?

    10. Update the remaining content if necessary.

    11. Remove `README_template.md`

        ```bash
        rm README_template.md
        ```

22. Doumentation

    Fill in missing info in docs.

    1. `PULL_REQUEST_TEMPLATE`

       1. Set project name (`projectName`)
       2. Set project owner (`authorGithubUsername`)

    2. `issue_labels.md`

       1. Set project name (`projectName`)
       2. Set project owner (`authorGithubUsername`)

    3. `developing.md`

       1. Set project name (`projectName`)
       2. Set project owner (`authorGithubUsername`)

    4. `CONTRIBUTING.md`

       1. Set project name (`projectName`)
       2. Set project owner (`authorGithubUsername`)

    5. `CODE_OF_CONDUCT.md`

       1. Set project team email (or your email, `authorEmail`)

    6. `logging.md`
       1. Select only those parts of logging strategy that apply.
          Or copy from another repo where it was already modified and
          that is the same type of project as this one.

23. Push the changes to the remote.

    1. Stage all changes

       ```bash
       git add -A
       ```

    2. Commit

       If this is first commit, skip validation by skipping Husky hooks

       ```bash
        HUSKY_SKIP_HOOKS=1 git commit -m "chore: initial commit"
       ```

    3. Push

       If this is first push, set upstream with `git pushu` (one of the
       aliases) set up in step 5.

       ```bash
       git pushu --no-verify
       ```

24. Zappr (bot)

    1. Go to [Zappr](https://zappr.opensource.zalan.do/) and activate
       appropriate checks, e.g.:

       - Approval check
       - Commit message check
       - Specification check

    2. Add the Zappr integration if not active yet.

25. CodeCov (bot)

    1. Add the CodeCov integration if not active yet.

26. CodeClimate (bot)

    1. Go to [CodeClimate](https://codeclimate.com/github/repos/new)
       and add the repo if not done before.

27. AllContributors (bot)

    1. Add the AllContributors integration if not active yet.

28. Hall of Fame Integration

    1. Refresh recognized repos on Sourcerer by going to
       https://sourcerer.io/your-username, and refresh.

    2. Go to Sourcerer's [Hall of Fame](https://sourcerer.io/settings#hof),
       select the repo and add it.

29. DependaBot (bot)

    1. Add the Dependabot integration if not active yet.

    2. If not active you can also activate it
       [here](https://app.dependabot.com/accounts/your-username).

30. LGTM (bot)

    1. Add the [LGTM integration](https://lgtm.com/dashboard) if not active
       yet.

31. Snyk (bot)

    1. Add
       [Snyk integration](https://support.snyk.io/hc/en-us/articles/360004032117-GitHub-integration)
       if not active yet.

32. Protect release branch from accidental modifications:

    1. Go to `https://github.com/<username>/<project-name>/settings/branches`
    2. Add new rule with branch pattern `master`.

33. Create Spectrum community

    1. Login to Spectrum and
       [create new community](https://spectrum.chat/new/community).

    2. Enter the name of the package as the community name (or sensible
       alternative if it is already taken).

    3. Description can be something like
       `Community for the <package-name> NPM package.` + package description

    4. Set community website as link to GitHub,
       e.g. `https://github.com/JuroOravec/instance-manager`

    5. Set community as public and hit create!

    6. Settings:

       - If relevant create appropriate channels

    7. Set to receive notifications from the channel (including the chat).

    8. Go to chat and add intro message, e.g. `Hi there!`.

    9. Pin _Welcome_ post (adapted from Pierre Vanduynslager's welcome post at
       [semantic-release Spectrum community page](https://spectrum.chat/semantic-release/general/welcome-to-the-semantic-release-community~283542eb-27ad-40c1-bd02-a7e4bef2ad16))

       ```txt
       Welcome to the <package-name> community!

       This is the place to discuss `<package-name>` package(s)/project(s) and ask for help.

       When discussing, let's stick to these rules:
       - Be kind, polite and respectful. We expect everyone to follow the [Spectrum’s Code of Conduct](https://github.com/withspectrum/code-of-conduct).
       - Search existing threads for your question to make sure it hasn't already been answered
       - Read the `<package-name>` [documentation](https://github.com/JuroOravec/<package-name>/tree/master/docs).
       - When creating a new thread, make sure to use a clear and unambiguous title so it can be found more easily by others.
       ```

       > Note: If the project is a multi-repo or a collection of projects
       > packages, use the plural form

Congratulations on getting all the way here! :confetti_ball: :tada:

### Workflow

See the [documentation](https://github.com/JuroOravec/chonky-node-template/tree/master/docs) for more on the workflow.

### Scripts

See below some common npm scripts that you will use. For full list, see
`package.json`.

Build distribution:

```bash
npm run build
```

Run tests:

```bash
npm test
```

Run formatters:

```bash
npm run-s format lint
```

Validation (security tests + formatting checks):

```bash
npm run validate
```

TypeDoc documentation:

```bash
# Markdown
npm run typedoc:markdown
# HTML
npm run typedoc:html
```

Add a contributor to README:

```bash
npm run contributors:add <all-contributors args...>
npm run contributors:generate
```

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

A template that came about from working with TypeScript.

## ⏳ Changelog

This projects follows semantic versioning. The
[changelog can be found here](https://github.com/JuroOravec/chonky-node-template/blob/master/CHANGELOG.md).

## 🛠 Developing

If you want to contribute to the project or forked it,
[this guide will get you up and going](https://github.com/JuroOravec/chonky-node-template/blob/master/docs/developing.md).

## 🏗 Roadmap

There is no explicit roadmap for this project. However, there is many ways how
this can be improve or automated, so if you have ideas and the time, please be
sure to share it with us by [opening an issue](#🤝-contributing).

## 🤝 Contributing

Contributions, issues and feature requests are welcome! Thank you ❤️

Feel free to dive in! See [current issues](https://github.com/JuroOravec/chonky-node-template/issues),
[open an issue](https://github.com/JuroOravec/chonky-node-template/issues/new), or [submit PRs](https://github.com/JuroOravec/chonky-node-template/compare).

How to report bugs, feature requests, and how to contribute and what conventions we use is all described in the [contributing guide](https://github.com/JuroOravec/chonky-node-template/tree/master/docs/CONTRIBUTING.md).

When contributing we follow the
[Contributor Covenant](https://contributor-covenant.org/version/1/3/0/).
See our [Code of Conduct](https://github.com/JuroOravec/chonky-node-template/blob/master/docs/CODE_OF_CONDUCT.md).

## 🧙 Contributors

Contributions of any kind welcome. Thanks goes to these wonderful people ❤️

### Recent and Top Contributors

<!-- Hall of Fame uses 8 links (7 users + 1 stats), see https://github.com/sourcerer-io/hall-of-fame#faq -->

[![Hall of Fame Contributor 1](https://sourcerer.io/fame/JuroOravec/JuroOravec/chonky-node-template/images/0)](https://sourcerer.io/fame/JuroOravec/JuroOravec/chonky-node-template/links/0)
[![Hall of Fame Contributor 2](https://sourcerer.io/fame/JuroOravec/JuroOravec/chonky-node-template/images/1)](https://sourcerer.io/fame/JuroOravec/JuroOravec/chonky-node-template/links/1)
[![Hall of Fame Contributor 3](https://sourcerer.io/fame/JuroOravec/JuroOravec/chonky-node-template/images/2)](https://sourcerer.io/fame/JuroOravec/JuroOravec/chonky-node-template/links/2)
[![Hall of Fame Contributor 4](https://sourcerer.io/fame/JuroOravec/JuroOravec/chonky-node-template/images/3)](https://sourcerer.io/fame/JuroOravec/JuroOravec/chonky-node-template/links/3)
[![Hall of Fame Contributor 5](https://sourcerer.io/fame/JuroOravec/JuroOravec/chonky-node-template/images/4)](https://sourcerer.io/fame/JuroOravec/JuroOravec/chonky-node-template/links/4)
[![Hall of Fame Contributor 6](https://sourcerer.io/fame/JuroOravec/JuroOravec/chonky-node-template/images/5)](https://sourcerer.io/fame/JuroOravec/JuroOravec/chonky-node-template/links/5)
[![Hall of Fame Contributor 7](https://sourcerer.io/fame/JuroOravec/JuroOravec/chonky-node-template/images/6)](https://sourcerer.io/fame/JuroOravec/JuroOravec/chonky-node-template/links/6)
[![Hall of Fame Contributor 8](https://sourcerer.io/fame/JuroOravec/JuroOravec/chonky-node-template/images/7)](https://sourcerer.io/fame/JuroOravec/JuroOravec/chonky-node-template/links/7)

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

## 🐙 Community

- [Stack Overflow](https://stackoverflow.com/questions/tagged/chonky-node-template)
- [Quora](https://www.quora.com/search?q=%22chonky-node-template%22)
- [Spectrum community](https://spectrum.chat/chonky-template/node)

<!-- ## 🔗 Related Projects

- e.g. If I make plugin I might want to link to them -->

## 👨‍🔧 Maintainers

👤 **Juro Oravec**

- Twitter: [@JuroOravec](https://twitter.com/JuroOravec)
- GitHub: [@JuroOravec](https://github.com/JuroOravec)
- LinkedIn: [@jurooravec](https://linkedin.com/in/jurooravec)
- Sourcerer: [@JuroOravec](https://sourcerer.io/JuroOravec)

## 📝 License

Copyright © 2020 [Juro Oravec](https://github.com/JuroOravec).

This project is [MIT](https://tldrlegal.com/license/mit-license) licensed.
