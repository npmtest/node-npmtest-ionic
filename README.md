# test coverage for  [ionic (v2.2.2-201704172341-201704172341)](http://ionicframework.com/)  [![npm package](https://img.shields.io/npm/v/npmtest-ionic.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-ionic) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-ionic.svg)](https://travis-ci.org/npmtest/node-npmtest-ionic)
#### A tool for creating and developing Ionic Framework mobile apps.

[![NPM](https://nodei.co/npm/ionic.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/ionic)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-ionic/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-ionic/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-ionic/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-ionic/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-ionic/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-ionic/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-ionic/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-ionic/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-ionic/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-ionic/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-ionic/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-ionic/build/test-report.html](https://npmtest.github.io/node-npmtest-ionic/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-ionic/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-ionic/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-ionic/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-ionic/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-ionic/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-ionic/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-ionic/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-ionic/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "ionic",
    "version": "2.2.2-201704172341-201704172341",
    "preferGlobal": true,
    "description": "A tool for creating and developing Ionic Framework mobile apps.",
    "homepage": "http://ionicframework.com/",
    "bin": {
        "ionic": "bin/ionic"
    },
    "scripts": {
        "changelog": "conventional-changelog -i CHANGELOG.md -s -p angular",
        "gh-release": "node scripts/release",
        "coveralls": "istanbul cover node_modules/jasmine-node/bin/jasmine-node --captureExceptions spec/ && cat coverage/lcov.info | node_modules/coveralls/bin/coveralls.js && rm -rf coverage",
        "e2e": "jasmine-node --captureExceptions ./e2e",
        "jasmine": "jasmine-node --captureExceptions  ./spec",
        "lint": "eslint .",
        "test": "istanbul cover node_modules/jasmine-node/bin/jasmine-node --captureExceptions spec/",
        "publish:nightly": "node ./scripts/publish-nightly.js"
    },
    "keywords": [
        "ionic",
        "ionic framework",
        "ionicframework",
        "mobile",
        "app",
        "hybrid",
        "cordova",
        "native",
        "phonegap"
    ],
    "repository": {
        "type": "git",
        "url": "git+https://github.com/driftyco/ionic-cli.git"
    },
    "contributors": [
        {
            "name": "Max Lynch",
            "url": "https://twitter.com/maxlynch"
        },
        {
            "name": "Peter Collins",
            "url": "https://twitter.com/SomethingNew2_0"
        },
        {
            "name": "Adam Bradley",
            "url": "https://twitter.com/adamdbradley"
        },
        {
            "name": "Josh Bavari",
            "url": "https://twitter.com/jbavari"
        },
        {
            "name": "Tim Lancina",
            "url": "https://twitter.com/timlancina"
        },
        {
            "name": "Josh Thomas",
            "url": "https://twitter.com/jthoms1"
        }
    ],
    "license": "MIT",
    "dependencies": {
        "@ionic/app-generators": "0.0.3",
        "chalk": "^1.1.3",
        "cli-table": "0.3.1",
        "cross-spawn": "^5.0.1",
        "expand-tilde": "1.2.0",
        "form-data": "0.1.4",
        "gulp": "3.8.8",
        "gulp-util": "3.0.7",
        "inquirer": "0.11.2",
        "ionic-app-lib": "2.2.1",
        "moment": "2.11.1",
        "open": "0.0.5",
        "optimist": "0.6.0",
        "pretty-hrtime": "1.0.2",
        "progress": "1.1.7",
        "prompt": "0.2.12",
        "q": "1.0.1",
        "request": "2.74.0",
        "semver": "4.3.6",
        "serve-static": "1.7.1",
        "shelljs": "0.2.6",
        "underscore": "1.7.0",
        "unzip": "0.1.9"
    },
    "devDependencies": {
        "conventional-changelog-cli": "1.1.1",
        "coveralls": "^2.2.0",
        "eslint": "^3.8.1",
        "eslint-plugin-no-use-extend-native": "^0.3.11",
        "github": "0.2.4",
        "istanbul": "^0.4.4",
        "jasmine-node": "1.14.5",
        "mock-require": "1.3.0",
        "rewire": "2.5.1"
    },
    "gitHead": "ebde0f5507a020a0f1b83061baf71e047a378801",
    "bugs": {
        "url": "https://github.com/driftyco/ionic-cli/issues"
    },
    "bundleDependencies": [
        "cli-table",
        "chalk",
        "cross-spawn",
        "expand-tilde",
        "form-data",
        "gulp",
        "gulp-util",
        "inquirer",
        "ionic-app-lib",
        "moment",
        "open",
        "optimist",
        "pretty-hrtime",
        "progress",
        "prompt",
        "q",
        "request",
        "semver",
        "serve-static",
        "shelljs",
        "underscore",
        "unzip"
    ],
    "dist": {
        "shasum": "3890117c43f2cf6719a3b9063c928420d1762f41",
        "tarball": "https://registry.npmjs.org/ionic/-/ionic-2.2.2.tgz"
    },
    "maintainers": [
        {
            "name": "brandyscarney"
        },
        {
            "name": "drifty"
        },
        {
            "name": "drygh"
        },
        {
            "name": "dwieeb"
        },
        {
            "name": "ericb"
        },
        {
            "name": "jthoms1"
        },
        {
            "name": "tlancina"
        }
    ],
    "directories": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
