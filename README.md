# npmtest-optimize-js

#### basic test coverage for  [optimize-js (v1.0.3)](https://github.com/nolanlawson/optimize-js#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-optimize-js.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-optimize-js) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-optimize-js.svg)](https://travis-ci.org/npmtest/node-npmtest-optimize-js)

#### Optimize initial JavaScript execution/parsing by wrapping eager functions

[![NPM](https://nodei.co/npm/optimize-js.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/optimize-js)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-optimize-js/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-optimize-js/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-optimize-js/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-optimize-js/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-optimize-js/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-optimize-js/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-optimize-js/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-optimize-js/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-optimize-js/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-optimize-js/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-optimize-js/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-optimize-js/build/test-report.html](https://npmtest.github.io/node-npmtest-optimize-js/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-optimize-js/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-optimize-js/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-optimize-js/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-optimize-js/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-optimize-js/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-optimize-js/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-optimize-js/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-optimize-js/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "optimize-js",
    "version": "1.0.3",
    "description": "Optimize initial JavaScript execution/parsing by wrapping eager functions",
    "main": "lib/index.js",
    "scripts": {
        "test": "standard && mocha --timeout 60000 test/test.js",
        "benchmark": "npm run build-benchmark && hs -p 9090 benchmarks",
        "build-benchmark": "sh bin/build-benchmark.sh",
        "publish-benchmark": "sh bin/publish-benchmark.sh",
        "coverage": "istanbul cover ./node_modules/mocha/bin/_mocha test/test.js && istanbul check-coverage --lines 100 --function 100 --statements 100 --branches 100"
    },
    "bin": {
        "optimize-js": "lib/bin.js"
    },
    "keywords": [
        "optimize",
        "optimise",
        "js"
    ],
    "author": "Nolan Lawson <nolan@nolanlawson.com>",
    "license": "Apache-2.0",
    "dependencies": {
        "acorn": "^3.3.0",
        "concat-stream": "^1.5.1",
        "estree-walker": "^0.3.0",
        "magic-string": "^0.16.0",
        "yargs": "^4.8.1"
    },
    "devDependencies": {
        "assert": "^1.4.1",
        "denodeify": "^1.2.1",
        "http-server": "^0.9.0",
        "istanbul": "^0.4.5",
        "mocha": "^3.0.2",
        "standard": "^7.1.2",
        "uglify-js": "^2.7.0"
    },
    "files": [
        "lib"
    ],
    "standard": {
        "ignore": [
            "test/cases/**",
            "benchmarks/**"
        ]
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/nolanlawson/optimize-js.git"
    },
    "bugs": {
        "url": "https://github.com/nolanlawson/optimize-js/issues"
    },
    "homepage": "https://github.com/nolanlawson/optimize-js#readme"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
