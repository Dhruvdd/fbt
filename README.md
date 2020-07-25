<p>
  <a href="https://travis-ci.com/facebook/fbt">
    <img src="https://img.shields.io/travis/com/facebook/fbt?logo=travis" alt="Travis CI" />
  </a>

  <a href="https://twitter.com/fbt_js">
    <img src="https://img.shields.io/twitter/follow/fbt_js.svg?style=social" align="right" alt="Twitter Follow" />
  </a>

  <a href="https://discord.gg/cQvXZr5">
    <img src="https://img.shields.io/discord/102860784329052160.svg" align="right" alt="Discord Chat" />
  </a>

  <a href="https://www.facebook.com/groups/498204277369868">
    <img src="https://img.shields.io/badge/Facebook-Group-blue" align="right" alt="Facebook Group" />
  </a>
</p>

<h1 align="center">
  <img src="https://facebook.github.io/fbt/img/fbt.png" height="150" width="150" alt="FBT"/>
</h1>

FBT is an internationalization framework for JavaScript designed to be not just powerful and flexible, but also simple and intuitive. It helps with the following:
Organizing your source text for translation
Composing grammatically correct translatable UI
Eliminating verbose boilerplate for generating UI
Examples
See our demo here See our React Native demo here
Requirements
Node.js
Yarn
Babel
Building the FBT library
git clone git@github.com:facebook/fbt.git
cd FBT
yarn install

NOTE: if you make changes to the FBT runtime that you'd like to test in the demo-app, be sure to run this command to rebuild the JS code:
yarn build-runtime

Using FBT
See how to use the source directly with Babel and Webpack in our demo-app.
How FBT works
FBT works by transforming your <fbt> and FBT(...) constructs via Babel plugins. These plugins serve to extract strings from source and lookup translated payloads generated at build-time. FBT creates tables of all possible variations for the given fbt phrase and accesses this at runtime.
Full documentation
https://facebook.github.io/fbt
Join the FBT community
Website
Facebook group
Discord #fbt channel in react flux
Twitter
See the CONTRIBUTING file for how to help out.
Changelog
See CHANGELOG.
List of npm modules published from this repo:
fbt (client-side)
See package.json config
babel-plugin-fbt (server-side)
See package.json config
babel-plugin-fbt-runtime (server-side)
See package.json config
fb-babel-plugin-utils (server-side, used by babel-plugin-fbt-runtime)
See package.json config
How to release a new npm version
# Go to the module's folder (where package.json is located)
cd fbt-runtime/
# or
# cd packages/babel-plugin-fbt/
# cd packages/babel-plugin-runtime/

# publishes to npm and push new git tag to Github
yarn publish_to_npm_latest

License
FBT is MIT licensed, as found in the LICENSE file.

