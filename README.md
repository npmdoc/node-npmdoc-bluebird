# npmdoc-bluebird

#### api documentation for  [bluebird (v3.5.0)](https://github.com/petkaantonov/bluebird)  [![npm package](https://img.shields.io/npm/v/npmdoc-bluebird.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-bluebird) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-bluebird.svg)](https://travis-ci.org/npmdoc/node-npmdoc-bluebird)

#### Full featured Promises/A+ implementation with exceptionally good performance

[![NPM](https://nodei.co/npm/bluebird.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/bluebird)

- [https://npmdoc.github.io/node-npmdoc-bluebird/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-bluebird/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-bluebird/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-bluebird/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-bluebird/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-bluebird/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Petka Antonov",
        "url": "http://github.com/petkaantonov/"
    },
    "browser": "./js/browser/bluebird.js",
    "bugs": {
        "url": "http://github.com/petkaantonov/bluebird/issues"
    },
    "dependencies": {},
    "description": "Full featured Promises/A+ implementation with exceptionally good performance",
    "devDependencies": {
        "acorn": "~0.6.0",
        "baconjs": "^0.7.43",
        "bluebird": "^2.9.2",
        "body-parser": "^1.10.2",
        "browserify": "^8.1.1",
        "cli-table": "~0.3.1",
        "co": "^4.2.0",
        "cross-spawn": "^0.2.3",
        "glob": "^4.3.2",
        "grunt-saucelabs": "~8.4.1",
        "highland": "^2.3.0",
        "istanbul": "^0.3.5",
        "jshint": "^2.6.0",
        "jshint-stylish": "~0.2.0",
        "kefir": "^2.4.1",
        "mkdirp": "~0.5.0",
        "mocha": "~2.1",
        "open": "~0.0.5",
        "optimist": "~0.6.1",
        "rimraf": "~2.2.6",
        "rx": "^2.3.25",
        "serve-static": "^1.7.1",
        "sinon": "~1.7.3",
        "uglify-js": "~2.4.16"
    },
    "directories": {},
    "dist": {
        "shasum": "791420d7f551eea2897453a8a77653f96606d67c",
        "tarball": "https://registry.npmjs.org/bluebird/-/bluebird-3.5.0.tgz"
    },
    "files": [
        "js/browser",
        "js/release",
        "LICENSE"
    ],
    "gitHead": "0b281e6caeec9c30b8de9a409b8ff1723f973f59",
    "homepage": "https://github.com/petkaantonov/bluebird",
    "keywords": [
        "promise",
        "performance",
        "promises",
        "promises-a",
        "promises-aplus",
        "async",
        "await",
        "deferred",
        "deferreds",
        "future",
        "flow control",
        "dsl",
        "fluent interface"
    ],
    "license": "MIT",
    "main": "./js/release/bluebird.js",
    "maintainers": [
        {
            "name": "esailija"
        }
    ],
    "name": "bluebird",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/petkaantonov/bluebird.git"
    },
    "scripts": {
        "generate-browser-core": "node tools/build.js --features=core --no-debug --release --zalgo --browser --minify && mv js/browser/bluebird.js js/browser/bluebird.core.js && mv js/browser/bluebird.min.js js/browser/bluebird.core.min.js",
        "generate-browser-full": "node tools/build.js --no-clean --no-debug --release --browser --minify",
        "istanbul": "istanbul",
        "lint": "node scripts/jshint.js",
        "prepublish": "npm run generate-browser-core && npm run generate-browser-full",
        "test": "node tools/test.js"
    },
    "version": "3.5.0",
    "webpack": "./js/release/bluebird.js"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
