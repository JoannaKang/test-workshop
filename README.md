# Testing Workshop

[![slides-badge][slides-badge]][slides]
[![chat-badge][chat-badge]][chat]
[![Build Status][build-badge]][build]
[![Dependencies][dependencyci-badge]][dependencyci]
[![MIT License][license-badge]][LICENSE]
[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors)

[![PRs Welcome][prs-badge]][prs]
[![Donate][donate-badge]][donate]
[![Code of Conduct][coc-badge]][coc]
[![Watch on GitHub][github-watch-badge]][github-watch]
[![Star on GitHub][github-star-badge]][github-star]
[![Tweet][twitter-badge]][twitter]

👋 hi there! My name is [Kent C. Dodds](https://kentcdodds.com)! This is a workshop repo to teach you about testing
JavaScript applications. We'll cover:

1. Unit Testing with [Jest](http://facebook.github.io/jest)
2. Integration Testing with [Jest](http://facebook.github.io/jest)
3. End to End (E2E) Testing with [Cypress](https://www.cypress.io/)

We'll mention other forms of testing, but these are the types we'll focus on and learn in this workshop. We'll learn
about the benefits (and tradeoffs) of [TDD](https://en.wikipedia.org/wiki/Test-driven_development). We'll learn how to
configure the tools and why, when, where, and what to test.

## Thank You

Big thanks to the [RealWorld](https://github.com/gothinkster/realworld) project from
[GoThinkster](https://github.com/gothinkster). This project is a copy of
[the Node implementation](https://github.com/gothinkster/node-express-realworld-example-app) and
[the React implementation](https://github.com/GoThinkster/react-redux-realworld-example-app) of the RealWorld project.

## Project

### System Requirements

- [git][git] v2.10.2 or greater
- [NodeJS][node] v6.9.5 or greater
- [yarn][yarn] v0.20.3 or greater (or [npm][npm] v4.2.0 or greater)
- [MongoDB][mongo] v3.4.2 or greater

### Setup

After you've made sure to have the correct things (and versions) installed, you should be able to just run a few
commands to get set up:

```
git clone https://github.com/kentcdodds/testing-workshop.git
cd testing-workshop
npm run setup
```

This may take a few minutes. If you get any errors, please read the error output and see whether there's any
instructions to fix things and try again. If you're still getting errors or need any help at all, then please
[file an issue][issue].

### Running the app

To get the app up and running (and really see if it worked), run:

```
npm start
```

This _should_ start `mongod`, the `api` server, and the `client` server in individual terminal tabs/windows. **This is
experimental** and if it doesn't work for you please [report it][issue].

*If it doesn't work for you, you can start each of these individually yourself:*

```
npm start mongo
```

```
npm start api
```

```
npm start client
```

With this, your browser should open up automatically to `http://localhost:8080` (if it doesn't, just open that yourself)
and you should be able to start messing around with the app.

If this fails at any point for you, please [report it][issue].

### Windows

If you're running on windows, you may have trouble with the `start` script and I'd love to know how to improve it.
You may also have trouble with `npm start mongo`. If that's the case, open up `package-scripts.js` and make sure that
`mongodBin` is set to the right value based on the path to your mongo installation.

### Structure

This project has a bit of a unique setup. Normally you'll have just a single `package.json` at the root of your
repository, but to simplify setup I've included both the `api` and `client` projects in a single repository. The root
of the project has a `package.json` as does `api`, and `client`. Most of our time working on tooling and running tests
will be in one of these sub-directories (with the exception of the E2E tests).

[issue]: https://github.com/kentcdodds/testing-workshop/issues/new

# LICENSE

The original projects are licensed as noted in their respective `package.json` files. The rest of this project is MIT
licensed.

## Contributors

Thanks goes to these wonderful people ([emoji key](https://github.com/kentcdodds/all-contributors#emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
| [<img src="https://avatars.githubusercontent.com/u/8601733?v=3" width="100px;"/><br /><sub>Thinkster</sub>](https://thinkster.io)<br />[💻](https://github.com/kentcdodds/testing-workshop/commits?author=gothinkster) | [<img src="https://avatars.githubusercontent.com/u/1500684?v=3" width="100px;"/><br /><sub>Kent C. Dodds</sub>](https://kentcdodds.com)<br />[💻](https://github.com/kentcdodds/testing-workshop/commits?author=kentcdodds) [📖](https://github.com/kentcdodds/testing-workshop/commits?author=kentcdodds) 🚇 [⚠️](https://github.com/kentcdodds/testing-workshop/commits?author=kentcdodds) |
| :---: | :---: |
<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/kentcdodds/all-contributors) specification. Contributions of any kind welcome!

[npm]: https://www.npmjs.com/
[yarn]: https://yarnpkg.com/
[node]: https://nodejs.org
[git]: https://git-scm.com/
[mongo]: https://www.mongodb.com/
[slides]: http://kcd.im/testing-intro-slides
[slides-badge]: https://cdn.rawgit.com/kentcdodds/custom-badges/2/badges/slides.svg
[chat]: https://gitter.im/kentcdodds/testing-workshop
[chat-badge]: https://img.shields.io/gitter/room/kentcdodds/testing-workshop.js.svg?style=flat-square
[build-badge]: https://img.shields.io/travis/kentcdodds/testing-workshop.svg?style=flat-square
[build]: https://travis-ci.org/kentcdodds/testing-workshop
[dependencyci-badge]: https://dependencyci.com/github/kentcdodds/testing-workshop/badge?style=flat-square
[dependencyci]: https://dependencyci.com/github/kentcdodds/testing-workshop
[license-badge]: https://img.shields.io/badge/license-MIT%20License-blue.svg?style=flat-square
[license]: https://github.com/kentcdodds/testing-workshop/blob/master/LICENSE
[prs-badge]: https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square
[prs]: http://makeapullrequest.com
[donate-badge]: https://img.shields.io/badge/$-support-green.svg?style=flat-square
[donate]: http://kcd.im/donate
[coc-badge]: https://img.shields.io/badge/code%20of-conduct-ff69b4.svg?style=flat-square
[coc]: https://github.com/kentcdodds/testing-workshop/blob/master/other/CODE_OF_CONDUCT.md
[github-watch-badge]: https://img.shields.io/github/watchers/kentcdodds/testing-workshop.svg?style=social
[github-watch]: https://github.com/kentcdodds/testing-workshop/watchers
[github-star-badge]: https://img.shields.io/github/stars/kentcdodds/testing-workshop.svg?style=social
[github-star]: https://github.com/kentcdodds/testing-workshop/stargazers
[twitter]: https://twitter.com/intent/tweet?text=Check%20out%20testing-workshop%20by%20@kentcdodds%20https://github.com/kentcdodds/testing-workshop%20%F0%9F%91%8D
[twitter-badge]: https://img.shields.io/twitter/url/https/github.com/kentcdodds/testing-workshop.svg?style=social
[emojis]: https://github.com/kentcdodds/all-contributors#emoji-key
[all-contributors]: https://github.com/kentcdodds/all-contributors