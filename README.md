# npmtest-cssify

#### basic test coverage for  cssify (v1.0.3)  [![npm package](https://img.shields.io/npm/v/npmtest-cssify.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-cssify) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-cssify.svg)](https://travis-ci.org/npmtest/node-npmtest-cssify)

#### A simple Browserify transform for adding required styles to the browser.

[![NPM](https://nodei.co/npm/cssify.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/cssify)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-cssify/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-cssify/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-cssify/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-cssify/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-cssify/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-cssify/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-cssify/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-cssify/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-cssify/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-cssify/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-cssify/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-cssify/build/test-report.html](https://npmtest.github.io/node-npmtest-cssify/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-cssify/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-cssify/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-cssify/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-cssify/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-cssify/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-cssify/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-cssify/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-cssify/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "cssify",
    "version": "1.0.3",
    "description": "A simple Browserify transform for adding required styles to the browser.",
    "main": "./lib/index.js",
    "scripts": {
        "pretest": "standard",
        "test:browser": "browserify -t [ . --no-auto-inject ] -t browserify-istanbul test/browser | browser-run | node test/extract-coverage.js | tap-difflet",
        "test:node": "istanbul cover --report json --print none ./node_modules/.bin/tape 'test/**/*.spec.js' | tap-difflet",
        "test": "mkdir -p coverage && npm run test:node && npm run test:browser && istanbul report"
    },
    "repository": "https://github.com/davidguttman/cssify",
    "keywords": [
        "browserify",
        "css",
        "transform",
        "browserify-transform",
        "dom",
        "browser"
    ],
    "browserify": "./lib/browser.js",
    "author": "David Guttman",
    "license": "BSD",
    "engines": {
        "node": ">= 0.12.0"
    },
    "dependencies": {
        "css-modules-loader-core": "^1.0.0",
        "lodash.assign": "^3.2.0",
        "resolve": "^1.1.6",
        "string-hash": "^1.1.0",
        "stringify-object": "^2.3.1",
        "through2": "^2.0.0"
    },
    "devDependencies": {
        "browser-run": "^3.0.3",
        "browserify": "^12.0.1",
        "browserify-istanbul": "^0.2.1",
        "concat-stream": "^1.5.1",
        "istanbul": "^0.4.0",
        "standard": "^5.3.1",
        "tap-difflet": "^0.4.0",
        "tape": "^4.2.2",
        "tape-catch": "^1.0.4"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
