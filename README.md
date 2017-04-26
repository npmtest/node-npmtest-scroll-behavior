# npmtest-scroll-behavior

#### basic test coverage for  [scroll-behavior (v0.9.3)](https://github.com/taion/scroll-behavior#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-scroll-behavior.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-scroll-behavior) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-scroll-behavior.svg)](https://travis-ci.org/npmtest/node-npmtest-scroll-behavior)

#### Pluggable browser scroll management

[![NPM](https://nodei.co/npm/scroll-behavior.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/scroll-behavior)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-scroll-behavior/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-scroll-behavior/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-scroll-behavior/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-scroll-behavior/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-scroll-behavior/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-scroll-behavior/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-scroll-behavior/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-scroll-behavior/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-scroll-behavior/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-scroll-behavior/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-scroll-behavior/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-scroll-behavior/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-scroll-behavior/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-scroll-behavior/build/test-report.html](https://npmtest.github.io/node-npmtest-scroll-behavior/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-scroll-behavior/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-scroll-behavior/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-scroll-behavior/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-scroll-behavior/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-scroll-behavior/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-scroll-behavior/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-scroll-behavior/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-scroll-behavior/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jimmy Jia"
    },
    "bugs": {
        "url": "https://github.com/taion/scroll-behavior/issues"
    },
    "dependencies": {
        "dom-helpers": "^3.0.0",
        "invariant": "^2.2.1"
    },
    "description": "Pluggable browser scroll management",
    "devDependencies": {
        "babel-cli": "^6.18.0",
        "babel-core": "^6.18.2",
        "babel-eslint": "^7.1.0",
        "babel-loader": "^6.2.7",
        "babel-plugin-add-module-exports": "^0.2.1",
        "babel-plugin-dev-expression": "^0.2.1",
        "babel-plugin-istanbul": "^2.0.3",
        "babel-polyfill": "^6.16.0",
        "babel-preset-latest": "^6.16.0",
        "babel-preset-stage-2": "^6.18.0",
        "chai": "^3.5.0",
        "codecov": "^1.0.1",
        "cross-env": "^3.1.3",
        "dirty-chai": "^1.2.2",
        "eslint": "^3.9.1",
        "eslint-config-4catalyzer": "^0.1.3",
        "eslint-plugin-import": "^1.16.0",
        "history": "^2.1.2",
        "karma": "^1.3.0",
        "karma-chrome-launcher": "^2.0.0",
        "karma-coverage": "^1.1.1",
        "karma-firefox-launcher": "^1.0.0",
        "karma-mocha": "^1.2.0",
        "karma-mocha-reporter": "^2.2.0",
        "karma-sinon-chai": "^1.2.4",
        "karma-sourcemap-loader": "^0.3.7",
        "karma-webpack": "^1.8.0",
        "mocha": "^3.1.2",
        "rimraf": "^2.5.4",
        "sinon": "^1.17.6",
        "sinon-chai": "^2.8.0",
        "webpack": "^1.13.3"
    },
    "directories": {},
    "dist": {
        "shasum": "e48bcc8af364f3f07176e8dbca3968bd5e71557b",
        "tarball": "https://registry.npmjs.org/scroll-behavior/-/scroll-behavior-0.9.3.tgz"
    },
    "files": [
        "lib"
    ],
    "gitHead": "e3a852d3b8ee96ddeed531ef4ffc358a4cbcef21",
    "homepage": "https://github.com/taion/scroll-behavior#readme",
    "keywords": [
        "scroll"
    ],
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "taion"
        }
    ],
    "name": "scroll-behavior",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/taion/scroll-behavior.git"
    },
    "scripts": {
        "build": "rimraf lib && babel src -d lib",
        "lint": "eslint src test *.js",
        "prepublish": "npm run build",
        "tdd": "cross-env NODE_ENV=test karma start",
        "test": "npm run lint && npm run testonly",
        "testonly": "npm run tdd -- --single-run"
    },
    "version": "0.9.3",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
