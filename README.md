<div align="center">
<h1>eslint-plugin-jest-dom</h1>

<p>ESLint plugin to follow best practices and anticipate common mistakes when writing tests with jest-dom.</p>
</div>

---

<!-- prettier-ignore-start -->
[![Build Status][build-badge]][build]
[![Code Coverage][coverage-badge]][coverage]
[![version][version-badge]][package]
[![downloads][downloads-badge]][npmtrends]
[![MIT License][license-badge]][license]
[![All Contributors][all-contributors-badge]](#contributors-)
[![PRs Welcome][prs-badge]][prs]
[![Code of Conduct][coc-badge]][coc]
<!-- prettier-ignore-end -->

## Table of Contents

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [Installation](#installation)
- [Usage](#usage)
- [Recommended Configuration](#recommended-configuration)
- [Supported Rules](#supported-rules)
- [Issues](#issues)
  - [🐛 Bugs](#-bugs)
  - [💡 Feature Requests](#-feature-requests)
- [Contributors ✨](#contributors-)
- [LICENSE](#license)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Installation

This module is distributed via [npm][npm] which is bundled with [node][node] and
should be installed as one of your project's `devDependencies`:

```
npm install --save-dev eslint-plugin-jest-dom
```

This library has a required `peerDependencies` listing for [`ESLint`](https://eslint.org/).

## Usage

Add `jest-dom` to the plugins section of your `.eslintrc.js` configuration file.
You can omit the `eslint-plugin-` prefix:

```javascript
module.exports = {
  plugins: ["jest-dom"],
  rules: {
    // your configuration
  },
};
```

Then configure the rules you want to use under the rules section.

```javascript
module.exports = {
  rules: {
    "jest-dom/prefer-checked": "error",
    "jest-dom/prefer-enabled-disabled": "error",
    "jest-dom/prefer-required": "error",
    "jest-dom/prefer-to-have-attribute": "error",
  },
};
```

## Recommended Configuration

This plugin exports a recommended configuration that enforces good `jest-dom`
practices _(you can find more info about enabled rules in
[Supported Rules section](#supported-rules))_.

To enable this configuration use the `extends` property in your `.eslintrc.js`
config file:

```javascript
module.exports = {
  extends: "plugin:jest-dom/recommended",
  rules: {
    // your configuration
  },
};
```

## Supported Rules

<!-- begin auto-generated rules list -->

💼 Configurations enabled in.\
✅ Set in the `recommended` configuration.\
🔧 Automatically fixable by the [`--fix` CLI option](https://eslint.org/docs/user-guide/command-line-interface#--fix).

| Name                                                                     | Description                                                           | 💼 | 🔧 |
| :----------------------------------------------------------------------- | :-------------------------------------------------------------------- | :- | :- |
| [prefer-checked](docs/rules/prefer-checked.md)                           | prefer toBeChecked over checking attributes                           | ✅  | 🔧 |
| [prefer-empty](docs/rules/prefer-empty.md)                               | Prefer toBeEmpty over checking innerHTML                              | ✅  | 🔧 |
| [prefer-enabled-disabled](docs/rules/prefer-enabled-disabled.md)         | prefer toBeDisabled or toBeEnabled over checking attributes           | ✅  | 🔧 |
| [prefer-focus](docs/rules/prefer-focus.md)                               | prefer toHaveFocus over checking document.activeElement               | ✅  | 🔧 |
| [prefer-in-document](docs/rules/prefer-in-document.md)                   | Prefer .toBeInTheDocument() for asserting the existence of a DOM node | ✅  | 🔧 |
| [prefer-required](docs/rules/prefer-required.md)                         | prefer toBeRequired over checking properties                          | ✅  | 🔧 |
| [prefer-to-have-attribute](docs/rules/prefer-to-have-attribute.md)       | prefer toHaveAttribute over checking  getAttribute/hasAttribute       | ✅  | 🔧 |
| [prefer-to-have-class](docs/rules/prefer-to-have-class.md)               | prefer toHaveClass over checking element className                    | ✅  | 🔧 |
| [prefer-to-have-style](docs/rules/prefer-to-have-style.md)               | prefer toHaveStyle over checking element style                        | ✅  | 🔧 |
| [prefer-to-have-text-content](docs/rules/prefer-to-have-text-content.md) | Prefer toHaveTextContent over checking element.textContent            | ✅  | 🔧 |
| [prefer-to-have-value](docs/rules/prefer-to-have-value.md)               | prefer toHaveValue over checking element.value                        | ✅  | 🔧 |

<!-- end auto-generated rules list -->

## Issues

_Looking to contribute? Look for the [Good First Issue][good-first-issue]
label._

### 🐛 Bugs

Please file an issue for bugs, missing documentation, or unexpected behavior.

[**See Bugs**][bugs]

### 💡 Feature Requests

Please file an issue to suggest new features. Vote on feature requests by adding
a 👍. This helps maintainers prioritize what to work on.

[**See Feature Requests**][requests]

## Contributors ✨

Thanks goes to these people ([emoji key][emojis]):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://github.com/benmonro"><img src="https://avatars3.githubusercontent.com/u/399236?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ben Monro</b></sub></a><br /><a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=benmonro" title="Documentation">📖</a> <a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=benmonro" title="Code">💻</a> <a href="#example-benmonro" title="Examples">💡</a> <a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=benmonro" title="Tests">⚠️</a></td>
    <td align="center"><a href="https://nickmccurdy.com/"><img src="https://avatars0.githubusercontent.com/u/927220?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Nick McCurdy</b></sub></a><br /><a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=nickmccurdy" title="Code">💻</a> <a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=nickmccurdy" title="Documentation">📖</a> <a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=nickmccurdy" title="Tests">⚠️</a></td>
    <td align="center"><a href="https://twitter.com/gnapse"><img src="https://avatars0.githubusercontent.com/u/15199?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ernesto García</b></sub></a><br /><a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=gnapse" title="Documentation">📖</a></td>
    <td align="center"><a href="https://chriscolborne.com"><img src="https://avatars2.githubusercontent.com/u/101371?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Chris Colborne</b></sub></a><br /><a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=zorfling" title="Code">💻</a> <a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=zorfling" title="Tests">⚠️</a></td>
    <td align="center"><a href="https://michaeldeboey.be"><img src="https://avatars3.githubusercontent.com/u/6643991?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Michaël De Boey</b></sub></a><br /><a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=MichaelDeBoey" title="Code">💻</a></td>
    <td align="center"><a href="http://gerritalex.de"><img src="https://avatars1.githubusercontent.com/u/29307652?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Gerrit Alex</b></sub></a><br /><a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=ljosberinn" title="Code">💻</a> <a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=ljosberinn" title="Tests">⚠️</a> <a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=ljosberinn" title="Documentation">📖</a> <a href="https://github.com/testing-library/eslint-plugin-jest-dom/issues?q=author%3Aljosberinn" title="Bug reports">🐛</a></td>
    <td align="center"><a href="http://ololos.space/"><img src="https://avatars1.githubusercontent.com/u/3940079?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Andrey Los</b></sub></a><br /><a href="https://github.com/testing-library/eslint-plugin-jest-dom/issues?q=author%3ARIP21" title="Bug reports">🐛</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://skovy.dev"><img src="https://avatars1.githubusercontent.com/u/5247455?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Spencer Miskoviak</b></sub></a><br /><a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=skovy" title="Code">💻</a> <a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=skovy" title="Tests">⚠️</a></td>
    <td align="center"><a href="https://github.com/atsikov"><img src="https://avatars3.githubusercontent.com/u/1422928?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Aleksei Tsikov</b></sub></a><br /><a href="https://github.com/testing-library/eslint-plugin-jest-dom/issues?q=author%3Aatsikov" title="Bug reports">🐛</a></td>
    <td align="center"><a href="https://mario.dev"><img src="https://avatars1.githubusercontent.com/u/2677072?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Mario Beltrán Alarcón</b></sub></a><br /><a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=Belco90" title="Documentation">📖</a></td>
    <td align="center"><a href="https://codepen.io/ariperkkio/"><img src="https://avatars2.githubusercontent.com/u/14806298?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ari Perkkiö</b></sub></a><br /><a href="https://github.com/testing-library/eslint-plugin-jest-dom/issues?q=author%3AAriPerkkio" title="Bug reports">🐛</a> <a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=AriPerkkio" title="Code">💻</a> <a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=AriPerkkio" title="Tests">⚠️</a></td>
    <td align="center"><a href="http://www.antn.se"><img src="https://avatars0.githubusercontent.com/u/785676?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Anton Niklasson</b></sub></a><br /><a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=AntonNiklasson" title="Code">💻</a> <a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=AntonNiklasson" title="Tests">⚠️</a> <a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=AntonNiklasson" title="Documentation">📖</a></td>
    <td align="center"><a href="http://juzerzarif.com"><img src="https://avatars3.githubusercontent.com/u/22772637?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Juzer Zarif</b></sub></a><br /><a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=juzerzarif" title="Code">💻</a> <a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=juzerzarif" title="Tests">⚠️</a> <a href="https://github.com/testing-library/eslint-plugin-jest-dom/issues?q=author%3Ajuzerzarif" title="Bug reports">🐛</a></td>
    <td align="center"><a href="http://everlong.org/"><img src="https://avatars.githubusercontent.com/u/454175?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Julien Wajsberg</b></sub></a><br /><a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=julienw" title="Code">💻</a> <a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=julienw" title="Tests">⚠️</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/G-Rath"><img src="https://avatars.githubusercontent.com/u/3151613?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Gareth Jones</b></sub></a><br /><a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=G-Rath" title="Tests">⚠️</a> <a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=G-Rath" title="Code">💻</a> <a href="https://github.com/testing-library/eslint-plugin-jest-dom/issues?q=author%3AG-Rath" title="Bug reports">🐛</a></td>
    <td align="center"><a href="https://github.com/huyenltnguyen"><img src="https://avatars.githubusercontent.com/u/25715018?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Huyen Nguyen</b></sub></a><br /><a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=huyenltnguyen" title="Documentation">📖</a></td>
    <td align="center"><a href="https://github.com/mdotwills"><img src="https://avatars.githubusercontent.com/u/5505611?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Matthew</b></sub></a><br /><a href="https://github.com/testing-library/eslint-plugin-jest-dom/issues?q=author%3Amdotwills" title="Bug reports">🐛</a> <a href="https://github.com/testing-library/eslint-plugin-jest-dom/commits?author=mdotwills" title="Code">💻</a></td>
  </tr>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors][all-contributors] specification.
Contributions of any kind welcome!

## LICENSE

MIT

<!-- prettier-ignore-start -->
[npm]: https://www.npmjs.com
[node]: https://nodejs.org
[build-badge]: https://img.shields.io/github/actions/workflow/status/testing-library/eslint-plugin-jest-dom/validate.yml?logo=github&style=flat-square
[build]: https://github.com/testing-library/eslint-plugin-jest-dom/actions?query=workflow%3Avalidate
[coverage-badge]: https://img.shields.io/codecov/c/github/testing-library/eslint-plugin-jest-dom.svg?style=flat-square
[coverage]: https://codecov.io/github/testing-library/eslint-plugin-jest-dom
[version-badge]: https://img.shields.io/npm/v/eslint-plugin-jest-dom.svg?style=flat-square
[package]: https://www.npmjs.com/package/eslint-plugin-jest-dom
[downloads-badge]: https://img.shields.io/npm/dm/eslint-plugin-jest-dom.svg?style=flat-square
[npmtrends]: http://www.npmtrends.com/eslint-plugin-jest-dom
[license-badge]: https://img.shields.io/npm/l/eslint-plugin-jest-dom.svg?style=flat-square
[license]: https://github.com/testing-library/eslint-plugin-jest-dom/blob/main/LICENSE
[prs-badge]: https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square
[prs]: http://makeapullrequest.com
[coc-badge]: https://img.shields.io/badge/code%20of-conduct-ff69b4.svg?style=flat-square
[coc]: https://github.com/testing-library/eslint-plugin-jest-dom/blob/main/other/CODE_OF_CONDUCT.md
[emojis]: https://github.com/all-contributors/all-contributors#emoji-key
[all-contributors]: https://github.com/all-contributors/all-contributors
[all-contributors-badge]: https://img.shields.io/github/all-contributors/testing-library/eslint-plugin-jest-dom
[bugs]: https://github.com/testing-library/eslint-plugin-jest-dom/issues?utf8=%E2%9C%93&q=is%3Aissue+is%3Aopen+sort%3Acreated-desc+label%3Abug
[requests]: https://github.com/testing-library/eslint-plugin-jest-dom/issues?utf8=%E2%9C%93&q=is%3Aissue+is%3Aopen+sort%3Areactions-%2B1-desc+label%3Aenhancement
[good-first-issue]: https://github.com/testing-library/eslint-plugin-jest-dom/issues?utf8=%E2%9C%93&q=is%3Aissue+is%3Aopen+sort%3Areactions-%2B1-desc+label%3Aenhancement+label%3A%22good+first+issue%22
<!-- prettier-ignore-end -->
