# api-documentation for  [bluebird (v3.5.0)](https://github.com/petkaantonov/bluebird)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-bluebird.svg)](https://travis-ci.org/npmdoc/node-npmdoc-bluebird)
#### Full featured Promises/A+ implementation with exceptionally good performance

[![NPM](https://nodei.co/npm/bluebird.png?downloads=true)](https://www.npmjs.com/package/bluebird)

# html version

- [https://npmdoc.github.io/node-npmdoc-bluebird/build..beta..travis-ci.org/apidoc.html](https://npmdoc.github.io/node-npmdoc-bluebird/build..beta..travis-ci.org/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-bluebird/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-bluebird_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-bluebird/build..beta..travis-ci.org/apidoc.html)

# package listing

![package-listing](https://npmdoc.github.io/node-npmdoc-bluebird/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Petka Antonov",
        "email": "petka_antonov@hotmail.com",
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
            "name": "esailija",
            "email": "petka_antonov@hotmail.com"
        }
    ],
    "name": "bluebird",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module bluebird](#apidoc.module.bluebird)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>AggregateError (message)](#apidoc.element.bluebird.AggregateError)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>CancellationError (message)](#apidoc.element.bluebird.CancellationError)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>OperationalError (message)](#apidoc.element.bluebird.OperationalError)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>Promise (executor)](#apidoc.element.bluebird.Promise)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>PromiseInspection (promise)](#apidoc.element.bluebird.PromiseInspection)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>RangeError ()](#apidoc.element.bluebird.RangeError)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>RejectionError (message)](#apidoc.element.bluebird.RejectionError)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>TimeoutError (message)](#apidoc.element.bluebird.TimeoutError)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>TypeError ()](#apidoc.element.bluebird.TypeError)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>_SomePromiseArray (values)](#apidoc.element.bluebird._SomePromiseArray)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>_peekContext ()](#apidoc.element.bluebird._peekContext)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>all (promises)](#apidoc.element.bluebird.all)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>any (promises)](#apidoc.element.bluebird.any)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>attempt (fn)](#apidoc.element.bluebird.attempt)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>bind (thisArg, value)](#apidoc.element.bluebird.bind)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>cast (obj)](#apidoc.element.bluebird.cast)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>config (opts)](#apidoc.element.bluebird.config)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>coroutine (generatorFunction, options)](#apidoc.element.bluebird.coroutine)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>defer ()](#apidoc.element.bluebird.defer)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>delay (ms, value)](#apidoc.element.bluebird.delay)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>each (promises, fn)](#apidoc.element.bluebird.each)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>filter (promises, fn, options)](#apidoc.element.bluebird.filter)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>fromCallback (fn)](#apidoc.element.bluebird.fromCallback)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>fromNode (fn)](#apidoc.element.bluebird.fromNode)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>fulfilled (obj)](#apidoc.element.bluebird.fulfilled)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>getNewLibraryCopy ()](#apidoc.element.bluebird.getNewLibraryCopy)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>hasLongStackTraces ()](#apidoc.element.bluebird.hasLongStackTraces)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>is (val)](#apidoc.element.bluebird.is)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>join ()](#apidoc.element.bluebird.join)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>longStackTraces ()](#apidoc.element.bluebird.longStackTraces)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>map (promises, fn, options, _filter)](#apidoc.element.bluebird.map)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>mapSeries (promises, fn)](#apidoc.element.bluebird.mapSeries)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>method (fn)](#apidoc.element.bluebird.method)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>noConflict ()](#apidoc.element.bluebird.noConflict)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>onPossiblyUnhandledRejection (fn)](#apidoc.element.bluebird.onPossiblyUnhandledRejection)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>onUnhandledRejectionHandled (fn)](#apidoc.element.bluebird.onUnhandledRejectionHandled)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>pending ()](#apidoc.element.bluebird.pending)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>promisify (fn, options)](#apidoc.element.bluebird.promisify)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>promisifyAll (target, options)](#apidoc.element.bluebird.promisifyAll)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>props (promises)](#apidoc.element.bluebird.props)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>race (promises)](#apidoc.element.bluebird.race)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>reduce (promises, fn, initialValue, _each)](#apidoc.element.bluebird.reduce)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>reject (reason)](#apidoc.element.bluebird.reject)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>rejected (reason)](#apidoc.element.bluebird.rejected)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>resolve (obj)](#apidoc.element.bluebird.resolve)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>setScheduler (fn)](#apidoc.element.bluebird.setScheduler)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>settle (promises)](#apidoc.element.bluebird.settle)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>some (promises, howMany)](#apidoc.element.bluebird.some)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>spawn (generatorFunction)](#apidoc.element.bluebird.spawn)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>try (fn)](#apidoc.element.bluebird.try)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>using ()](#apidoc.element.bluebird.using)
1.  object <span class="apidocSignatureSpan">bluebird.</span>AggregateError.prototype
1.  object <span class="apidocSignatureSpan">bluebird.</span>CancellationError.prototype
1.  object <span class="apidocSignatureSpan">bluebird.</span>OperationalError.prototype
1.  object <span class="apidocSignatureSpan">bluebird.</span>PromiseInspection.prototype
1.  object <span class="apidocSignatureSpan">bluebird.</span>TimeoutError.prototype
1.  object <span class="apidocSignatureSpan">bluebird.</span>_SomePromiseArray.prototype
1.  string <span class="apidocSignatureSpan">bluebird.</span>version

#### [module bluebird.AggregateError](#apidoc.module.bluebird.AggregateError)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>AggregateError (message)](#apidoc.element.bluebird.AggregateError.AggregateError)

#### [module bluebird.AggregateError.prototype](#apidoc.module.bluebird.AggregateError.prototype)
1.  boolean <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>isOperational
1.  [function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>constructor (message)](#apidoc.element.bluebird.AggregateError.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>every ()](#apidoc.element.bluebird.AggregateError.prototype.every)
1.  [function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>filter ()](#apidoc.element.bluebird.AggregateError.prototype.filter)
1.  [function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>forEach ()](#apidoc.element.bluebird.AggregateError.prototype.forEach)
1.  [function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>indexOf ()](#apidoc.element.bluebird.AggregateError.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>join ()](#apidoc.element.bluebird.AggregateError.prototype.join)
1.  [function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>lastIndexOf ()](#apidoc.element.bluebird.AggregateError.prototype.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>map ()](#apidoc.element.bluebird.AggregateError.prototype.map)
1.  [function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>pop ()](#apidoc.element.bluebird.AggregateError.prototype.pop)
1.  [function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>push ()](#apidoc.element.bluebird.AggregateError.prototype.push)
1.  [function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>reduce ()](#apidoc.element.bluebird.AggregateError.prototype.reduce)
1.  [function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>reduceRight ()](#apidoc.element.bluebird.AggregateError.prototype.reduceRight)
1.  [function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>reverse ()](#apidoc.element.bluebird.AggregateError.prototype.reverse)
1.  [function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>shift ()](#apidoc.element.bluebird.AggregateError.prototype.shift)
1.  [function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>slice ()](#apidoc.element.bluebird.AggregateError.prototype.slice)
1.  [function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>some ()](#apidoc.element.bluebird.AggregateError.prototype.some)
1.  [function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>sort ()](#apidoc.element.bluebird.AggregateError.prototype.sort)
1.  [function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>toString ()](#apidoc.element.bluebird.AggregateError.prototype.toString)
1.  [function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>unshift ()](#apidoc.element.bluebird.AggregateError.prototype.unshift)
1.  number <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>length

#### [module bluebird.CancellationError](#apidoc.module.bluebird.CancellationError)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>CancellationError (message)](#apidoc.element.bluebird.CancellationError.CancellationError)

#### [module bluebird.CancellationError.prototype](#apidoc.module.bluebird.CancellationError.prototype)
1.  [function <span class="apidocSignatureSpan">bluebird.CancellationError.prototype.</span>constructor (message)](#apidoc.element.bluebird.CancellationError.prototype.constructor)

#### [module bluebird.OperationalError](#apidoc.module.bluebird.OperationalError)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>OperationalError (message)](#apidoc.element.bluebird.OperationalError.OperationalError)

#### [module bluebird.OperationalError.prototype](#apidoc.module.bluebird.OperationalError.prototype)
1.  [function <span class="apidocSignatureSpan">bluebird.OperationalError.prototype.</span>constructor (message)](#apidoc.element.bluebird.OperationalError.prototype.constructor)

#### [module bluebird.PromiseInspection](#apidoc.module.bluebird.PromiseInspection)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>PromiseInspection (promise)](#apidoc.element.bluebird.PromiseInspection.PromiseInspection)

#### [module bluebird.PromiseInspection.prototype](#apidoc.module.bluebird.PromiseInspection.prototype)
1.  [function <span class="apidocSignatureSpan">bluebird.PromiseInspection.prototype.</span>_settledValue ()](#apidoc.element.bluebird.PromiseInspection.prototype._settledValue)
1.  [function <span class="apidocSignatureSpan">bluebird.PromiseInspection.prototype.</span>error ()](#apidoc.element.bluebird.PromiseInspection.prototype.error)
1.  [function <span class="apidocSignatureSpan">bluebird.PromiseInspection.prototype.</span>isCancelled ()](#apidoc.element.bluebird.PromiseInspection.prototype.isCancelled)
1.  [function <span class="apidocSignatureSpan">bluebird.PromiseInspection.prototype.</span>isFulfilled ()](#apidoc.element.bluebird.PromiseInspection.prototype.isFulfilled)
1.  [function <span class="apidocSignatureSpan">bluebird.PromiseInspection.prototype.</span>isPending ()](#apidoc.element.bluebird.PromiseInspection.prototype.isPending)
1.  [function <span class="apidocSignatureSpan">bluebird.PromiseInspection.prototype.</span>isRejected ()](#apidoc.element.bluebird.PromiseInspection.prototype.isRejected)
1.  [function <span class="apidocSignatureSpan">bluebird.PromiseInspection.prototype.</span>isResolved ()](#apidoc.element.bluebird.PromiseInspection.prototype.isResolved)
1.  [function <span class="apidocSignatureSpan">bluebird.PromiseInspection.prototype.</span>reason ()](#apidoc.element.bluebird.PromiseInspection.prototype.reason)
1.  [function <span class="apidocSignatureSpan">bluebird.PromiseInspection.prototype.</span>value ()](#apidoc.element.bluebird.PromiseInspection.prototype.value)

#### [module bluebird.TimeoutError](#apidoc.module.bluebird.TimeoutError)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>TimeoutError (message)](#apidoc.element.bluebird.TimeoutError.TimeoutError)

#### [module bluebird.TimeoutError.prototype](#apidoc.module.bluebird.TimeoutError.prototype)
1.  [function <span class="apidocSignatureSpan">bluebird.TimeoutError.prototype.</span>constructor (message)](#apidoc.element.bluebird.TimeoutError.prototype.constructor)

#### [module bluebird._SomePromiseArray](#apidoc.module.bluebird._SomePromiseArray)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>_SomePromiseArray (values)](#apidoc.element.bluebird._SomePromiseArray._SomePromiseArray)

#### [module bluebird._SomePromiseArray.prototype](#apidoc.module.bluebird._SomePromiseArray.prototype)
1.  [function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_addFulfilled (value)](#apidoc.element.bluebird._SomePromiseArray.prototype._addFulfilled)
1.  [function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_addRejected (reason)](#apidoc.element.bluebird._SomePromiseArray.prototype._addRejected)
1.  [function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_canPossiblyFulfill ()](#apidoc.element.bluebird._SomePromiseArray.prototype._canPossiblyFulfill)
1.  [function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_checkOutcome ()](#apidoc.element.bluebird._SomePromiseArray.prototype._checkOutcome)
1.  [function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_fulfilled ()](#apidoc.element.bluebird._SomePromiseArray.prototype._fulfilled)
1.  [function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_getRangeError (count)](#apidoc.element.bluebird._SomePromiseArray.prototype._getRangeError)
1.  [function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_init ()](#apidoc.element.bluebird._SomePromiseArray.prototype._init)
1.  [function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_promiseCancelled ()](#apidoc.element.bluebird._SomePromiseArray.prototype._promiseCancelled)
1.  [function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_promiseFulfilled (value)](#apidoc.element.bluebird._SomePromiseArray.prototype._promiseFulfilled)
1.  [function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_promiseRejected (reason)](#apidoc.element.bluebird._SomePromiseArray.prototype._promiseRejected)
1.  [function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_rejected ()](#apidoc.element.bluebird._SomePromiseArray.prototype._rejected)
1.  [function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_resolveEmptyArray ()](#apidoc.element.bluebird._SomePromiseArray.prototype._resolveEmptyArray)
1.  [function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>constructor (values)](#apidoc.element.bluebird._SomePromiseArray.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>howMany ()](#apidoc.element.bluebird._SomePromiseArray.prototype.howMany)
1.  [function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>init ()](#apidoc.element.bluebird._SomePromiseArray.prototype.init)
1.  [function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>setHowMany (count)](#apidoc.element.bluebird._SomePromiseArray.prototype.setHowMany)
1.  [function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>setUnwrap ()](#apidoc.element.bluebird._SomePromiseArray.prototype.setUnwrap)

#### [module bluebird.coroutine](#apidoc.module.bluebird.coroutine)
1.  [function <span class="apidocSignatureSpan">bluebird.</span>coroutine (generatorFunction, options)](#apidoc.element.bluebird.coroutine.coroutine)
1.  [function <span class="apidocSignatureSpan">bluebird.coroutine.</span>addYieldHandler (fn)](#apidoc.element.bluebird.coroutine.addYieldHandler)



# <a name="apidoc.module.bluebird"></a>[module bluebird](#apidoc.module.bluebird)

#### <a name="apidoc.element.bluebird.AggregateError"></a>[function <span class="apidocSignatureSpan">bluebird.</span>AggregateError (message)](#apidoc.element.bluebird.AggregateError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.CancellationError"></a>[function <span class="apidocSignatureSpan">bluebird.</span>CancellationError (message)](#apidoc.element.bluebird.CancellationError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.OperationalError"></a>[function <span class="apidocSignatureSpan">bluebird.</span>OperationalError (message)](#apidoc.element.bluebird.OperationalError)
- description and source-code
```javascript
function OperationalError(message) {
    if (!(this instanceof OperationalError))
        return new OperationalError(message);
    notEnumerableProp(this, "name", "OperationalError");
    notEnumerableProp(this, "message", message);
    this.cause = message;
    this["isOperational"] = true;

    if (message instanceof Error) {
        notEnumerableProp(this, "message", message.message);
        notEnumerableProp(this, "stack", message.stack);
    } else if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.Promise"></a>[function <span class="apidocSignatureSpan">bluebird.</span>Promise (executor)](#apidoc.element.bluebird.Promise)
- description and source-code
```javascript
function Promise(executor) {
    if (executor !== INTERNAL) {
        check(this, executor);
    }
    this._bitField = 0;
    this._fulfillmentHandler0 = undefined;
    this._rejectionHandler0 = undefined;
    this._promise0 = undefined;
    this._receiver0 = undefined;
    this._resolveFromExecutor(executor);
    this._promiseCreated();
    this._fireEvent("promiseCreated", this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.PromiseInspection"></a>[function <span class="apidocSignatureSpan">bluebird.</span>PromiseInspection (promise)](#apidoc.element.bluebird.PromiseInspection)
- description and source-code
```javascript
function PromiseInspection(promise) {
    if (promise !== undefined) {
        promise = promise._target();
        this._bitField = promise._bitField;
        this._settledValueField = promise._isFateSealed()
            ? promise._settledValue() : undefined;
    }
    else {
        this._bitField = 0;
        this._settledValueField = undefined;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.RangeError"></a>[function <span class="apidocSignatureSpan">bluebird.</span>RangeError ()](#apidoc.element.bluebird.RangeError)
- description and source-code
```javascript
function RangeError() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.RejectionError"></a>[function <span class="apidocSignatureSpan">bluebird.</span>RejectionError (message)](#apidoc.element.bluebird.RejectionError)
- description and source-code
```javascript
function OperationalError(message) {
    if (!(this instanceof OperationalError))
        return new OperationalError(message);
    notEnumerableProp(this, "name", "OperationalError");
    notEnumerableProp(this, "message", message);
    this.cause = message;
    this["isOperational"] = true;

    if (message instanceof Error) {
        notEnumerableProp(this, "message", message.message);
        notEnumerableProp(this, "stack", message.stack);
    } else if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    }

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.TimeoutError"></a>[function <span class="apidocSignatureSpan">bluebird.</span>TimeoutError (message)](#apidoc.element.bluebird.TimeoutError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.TypeError"></a>[function <span class="apidocSignatureSpan">bluebird.</span>TypeError ()](#apidoc.element.bluebird.TypeError)
- description and source-code
```javascript
function TypeError() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird._SomePromiseArray"></a>[function <span class="apidocSignatureSpan">bluebird.</span>_SomePromiseArray (values)](#apidoc.element.bluebird._SomePromiseArray)
- description and source-code
```javascript
function SomePromiseArray(values) {
    this.constructor$(values);
    this._howMany = 0;
    this._unwrap = false;
    this._initialized = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird._peekContext"></a>[function <span class="apidocSignatureSpan">bluebird.</span>_peekContext ()](#apidoc.element.bluebird._peekContext)
- description and source-code
```javascript
_peekContext = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.all"></a>[function <span class="apidocSignatureSpan">bluebird.</span>all (promises)](#apidoc.element.bluebird.all)
- description and source-code
```javascript
all = function (promises) {
    return new PromiseArray(promises).promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.any"></a>[function <span class="apidocSignatureSpan">bluebird.</span>any (promises)](#apidoc.element.bluebird.any)
- description and source-code
```javascript
any = function (promises) {
    return any(promises);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.attempt"></a>[function <span class="apidocSignatureSpan">bluebird.</span>attempt (fn)](#apidoc.element.bluebird.attempt)
- description and source-code
```javascript
attempt = function (fn) {
    if (typeof fn !== "function") {
        return apiRejection("expecting a function but got " + util.classString(fn));
    }
    var ret = new Promise(INTERNAL);
    ret._captureStackTrace();
    ret._pushContext();
    var value;
    if (arguments.length > 1) {
        debug.deprecated("calling Promise.try with more than 1 argument");
        var arg = arguments[1];
        var ctx = arguments[2];
        value = util.isArray(arg) ? tryCatch(fn).apply(ctx, arg)
                                  : tryCatch(fn).call(ctx, arg);
    } else {
        value = tryCatch(fn)();
    }
    var promiseCreated = ret._popContext();
    debug.checkForgottenReturns(
        value, promiseCreated, "Promise.try", ret);
    ret._resolveFromSyncValue(value);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.bind"></a>[function <span class="apidocSignatureSpan">bluebird.</span>bind (thisArg, value)](#apidoc.element.bluebird.bind)
- description and source-code
```javascript
bind = function (thisArg, value) {
    return Promise.resolve(value).bind(thisArg);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.cast"></a>[function <span class="apidocSignatureSpan">bluebird.</span>cast (obj)](#apidoc.element.bluebird.cast)
- description and source-code
```javascript
cast = function (obj) {
    var ret = tryConvertToPromise(obj);
    if (!(ret instanceof Promise)) {
        ret = new Promise(INTERNAL);
        ret._captureStackTrace();
        ret._setFulfilled();
        ret._rejectionHandler0 = obj;
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.config"></a>[function <span class="apidocSignatureSpan">bluebird.</span>config (opts)](#apidoc.element.bluebird.config)
- description and source-code
```javascript
config = function (opts) {
    opts = Object(opts);
    if ("longStackTraces" in opts) {
        if (opts.longStackTraces) {
            Promise.longStackTraces();
        } else if (!opts.longStackTraces && Promise.hasLongStackTraces()) {
            disableLongStackTraces();
        }
    }
    if ("warnings" in opts) {
        var warningsOption = opts.warnings;
        config.warnings = !!warningsOption;
        wForgottenReturn = config.warnings;

        if (util.isObject(warningsOption)) {
            if ("wForgottenReturn" in warningsOption) {
                wForgottenReturn = !!warningsOption.wForgottenReturn;
            }
        }
    }
    if ("cancellation" in opts && opts.cancellation && !config.cancellation) {
        if (async.haveItemsQueued()) {
            throw new Error(
                "cannot enable cancellation after promises are in use");
        }
        Promise.prototype._clearCancellationData =
            cancellationClearCancellationData;
        Promise.prototype._propagateFrom = cancellationPropagateFrom;
        Promise.prototype._onCancel = cancellationOnCancel;
        Promise.prototype._setOnCancel = cancellationSetOnCancel;
        Promise.prototype._attachCancellationCallback =
            cancellationAttachCancellationCallback;
        Promise.prototype._execute = cancellationExecute;
        propagateFromFunction = cancellationPropagateFrom;
        config.cancellation = true;
    }
    if ("monitoring" in opts) {
        if (opts.monitoring && !config.monitoring) {
            config.monitoring = true;
            Promise.prototype._fireEvent = activeFireEvent;
        } else if (!opts.monitoring && config.monitoring) {
            config.monitoring = false;
            Promise.prototype._fireEvent = defaultFireEvent;
        }
    }
    return Promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.coroutine"></a>[function <span class="apidocSignatureSpan">bluebird.</span>coroutine (generatorFunction, options)](#apidoc.element.bluebird.coroutine)
- description and source-code
```javascript
coroutine = function (generatorFunction, options) {
    if (typeof generatorFunction !== "function") {
        throw new TypeError("generatorFunction must be a function\u000a\u000a    See http://goo.gl/MqrFmX\u000a");
    }
    var yieldHandler = Object(options).yieldHandler;
    var PromiseSpawn$ = PromiseSpawn;
    var stack = new Error().stack;
    return function () {
        var generator = generatorFunction.apply(this, arguments);
        var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                      stack);
        var ret = spawn.promise();
        spawn._generator = generator;
        spawn._promiseFulfilled(undefined);
        return ret;
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.defer"></a>[function <span class="apidocSignatureSpan">bluebird.</span>defer ()](#apidoc.element.bluebird.defer)
- description and source-code
```javascript
defer = function () {
    debug.deprecated("Promise.defer", "new Promise");
    var promise = new Promise(INTERNAL);
    return {
        promise: promise,
        resolve: deferResolve,
        reject: deferReject
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.delay"></a>[function <span class="apidocSignatureSpan">bluebird.</span>delay (ms, value)](#apidoc.element.bluebird.delay)
- description and source-code
```javascript
delay = function (ms, value) {
    var ret;
    var handle;
    if (value !== undefined) {
        ret = Promise.resolve(value)
                ._then(afterValue, null, null, ms, undefined);
        if (debug.cancellation() && value instanceof Promise) {
            ret._setOnCancel(value);
        }
    } else {
        ret = new Promise(INTERNAL);
        handle = setTimeout(function() { ret._fulfill(); }, +ms);
        if (debug.cancellation()) {
            ret._setOnCancel(new HandleWrapper(handle));
        }
        ret._captureStackTrace();
    }
    ret._setAsyncGuaranteed();
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.each"></a>[function <span class="apidocSignatureSpan">bluebird.</span>each (promises, fn)](#apidoc.element.bluebird.each)
- description and source-code
```javascript
each = function (promises, fn) {
    return PromiseReduce(promises, fn, INTERNAL, 0)
              ._then(promiseAllThis, undefined, undefined, promises, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.filter"></a>[function <span class="apidocSignatureSpan">bluebird.</span>filter (promises, fn, options)](#apidoc.element.bluebird.filter)
- description and source-code
```javascript
filter = function (promises, fn, options) {
    return PromiseMap(promises, fn, options, INTERNAL);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.fromCallback"></a>[function <span class="apidocSignatureSpan">bluebird.</span>fromCallback (fn)](#apidoc.element.bluebird.fromCallback)
- description and source-code
```javascript
fromCallback = function (fn) {
    var ret = new Promise(INTERNAL);
    ret._captureStackTrace();
    var multiArgs = arguments.length > 1 ? !!Object(arguments[1]).multiArgs
                                         : false;
    var result = tryCatch(fn)(nodebackForPromise(ret, multiArgs));
    if (result === errorObj) {
        ret._rejectCallback(result.e, true);
    }
    if (!ret._isFateSealed()) ret._setAsyncGuaranteed();
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.fromNode"></a>[function <span class="apidocSignatureSpan">bluebird.</span>fromNode (fn)](#apidoc.element.bluebird.fromNode)
- description and source-code
```javascript
fromNode = function (fn) {
    var ret = new Promise(INTERNAL);
    ret._captureStackTrace();
    var multiArgs = arguments.length > 1 ? !!Object(arguments[1]).multiArgs
                                         : false;
    var result = tryCatch(fn)(nodebackForPromise(ret, multiArgs));
    if (result === errorObj) {
        ret._rejectCallback(result.e, true);
    }
    if (!ret._isFateSealed()) ret._setAsyncGuaranteed();
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.fulfilled"></a>[function <span class="apidocSignatureSpan">bluebird.</span>fulfilled (obj)](#apidoc.element.bluebird.fulfilled)
- description and source-code
```javascript
fulfilled = function (obj) {
    var ret = tryConvertToPromise(obj);
    if (!(ret instanceof Promise)) {
        ret = new Promise(INTERNAL);
        ret._captureStackTrace();
        ret._setFulfilled();
        ret._rejectionHandler0 = obj;
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.getNewLibraryCopy"></a>[function <span class="apidocSignatureSpan">bluebird.</span>getNewLibraryCopy ()](#apidoc.element.bluebird.getNewLibraryCopy)
- description and source-code
```javascript
getNewLibraryCopy = function () {
var makeSelfResolutionError = function () {
    return new TypeError("circular promise resolution chain\u000a\u000a    See http://goo.gl/MqrFmX\u000a");
};
var reflectHandler = function() {
    return new Promise.PromiseInspection(this._target());
};
var apiRejection = function(msg) {
    return Promise.reject(new TypeError(msg));
};
function Proxyable() {}
var UNDEFINED_BINDING = {};
var util = require("./util");

var getDomain;
if (util.isNode) {
    getDomain = function() {
        var ret = process.domain;
        if (ret === undefined) ret = null;
        return ret;
    };
} else {
    getDomain = function() {
        return null;
    };
}
util.notEnumerableProp(Promise, "_getDomain", getDomain);

var es5 = require("./es5");
var Async = require("./async");
var async = new Async();
es5.defineProperty(Promise, "_async", {value: async});
var errors = require("./errors");
var TypeError = Promise.TypeError = errors.TypeError;
Promise.RangeError = errors.RangeError;
var CancellationError = Promise.CancellationError = errors.CancellationError;
Promise.TimeoutError = errors.TimeoutError;
Promise.OperationalError = errors.OperationalError;
Promise.RejectionError = errors.OperationalError;
Promise.AggregateError = errors.AggregateError;
var INTERNAL = function(){};
var APPLY = {};
var NEXT_FILTER = {};
var tryConvertToPromise = require("./thenables")(Promise, INTERNAL);
var PromiseArray =
    require("./promise_array")(Promise, INTERNAL,
                               tryConvertToPromise, apiRejection, Proxyable);
var Context = require("./context")(Promise);
<span class="apidocCodeCommentSpan"> /*jshint unused:false*/
</span>var createContext = Context.create;
var debug = require("./debuggability")(Promise, Context);
var CapturedTrace = debug.CapturedTrace;
var PassThroughHandlerContext =
    require("./finally")(Promise, tryConvertToPromise, NEXT_FILTER);
var catchFilter = require("./catch_filter")(NEXT_FILTER);
var nodebackForPromise = require("./nodeback");
var errorObj = util.errorObj;
var tryCatch = util.tryCatch;
function check(self, executor) {
    if (self == null || self.constructor !== Promise) {
        throw new TypeError("the promise constructor cannot be invoked directly\u000a\u000a    See http://goo.gl/MqrFmX\u000a");
    }
    if (typeof executor !== "function") {
        throw new TypeError("expecting a function but got " + util.classString(executor));
    }

}

function Promise(executor) {
    if (executor !== INTERNAL) {
        check(this, executor);
    }
    this._bitField = 0;
    this._fulfillmentHandler0 = undefined;
    this._rejectionHandler0 = undefined;
    this._promise0 = undefined;
    this._receiver0 = undefined;
    this._resolveFromExecutor(executor);
    this._promiseCreated();
    this._fireEvent("promiseCreated", this);
}

Promise.prototype.toString = function () {
    return "[object Promise]";
};

Promise.prototype.caught = Promise.prototype["catch"] = function (fn) {
    var len = arguments.length;
    if (len > 1) {
        var catchInstances = new Array(len - 1),
            j = 0, i;
        for (i = 0; i < len - 1; ++i) {
            var item = arguments[i];
            if (util.isObject(item)) {
                catchInstances[j++] = item;
            } else {
                return apiRejection("Catch statement predicate: " +
                    "expecting an object but got " + util.classString(item));
            }
        }
        catchInstances.length = j;
        fn = arguments[i];
        return this.then(undefined, catchFilter(catchInstances, fn, this));
    }
    return this.then(undefined, fn);
};

Promise.prototype.reflect = function () {
    return this._then(reflectHandler,
        reflectHandler, undefined, this, undefined);
};

Promise.prototype.then = function (didFulfill, didReject) {
    if (debug.warnings() && arguments.length > 0 &&
        typeof didFulfill !== "function" &&
        typeof didReject !== "function") {
        var msg = ".then() only accepts functions but was passed: " +
                util.classString(didFulfill);
        if (arguments.length > 1) {
            msg += ", ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.hasLongStackTraces"></a>[function <span class="apidocSignatureSpan">bluebird.</span>hasLongStackTraces ()](#apidoc.element.bluebird.hasLongStackTraces)
- description and source-code
```javascript
hasLongStackTraces = function () {
    return config.longStackTraces && longStackTracesIsSupported();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.is"></a>[function <span class="apidocSignatureSpan">bluebird.</span>is (val)](#apidoc.element.bluebird.is)
- description and source-code
```javascript
is = function (val) {
    return val instanceof Promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.join"></a>[function <span class="apidocSignatureSpan">bluebird.</span>join ()](#apidoc.element.bluebird.join)
- description and source-code
```javascript
join = function () {
    var last = arguments.length - 1;
    var fn;
    if (last > 0 && typeof arguments[last] === "function") {
        fn = arguments[last];
        if (!false) {
            if (last <= 8 && canEvaluate) {
                var ret = new Promise(INTERNAL);
                ret._captureStackTrace();
                var HolderClass = holderClasses[last - 1];
                var holder = new HolderClass(fn);
                var callbacks = thenCallbacks;

                for (var i = 0; i < last; ++i) {
                    var maybePromise = tryConvertToPromise(arguments[i], ret);
                    if (maybePromise instanceof Promise) {
                        maybePromise = maybePromise._target();
                        var bitField = maybePromise._bitField;
                        ;
                        if (((bitField & 50397184) === 0)) {
                            maybePromise._then(callbacks[i], reject,
                                               undefined, ret, holder);
                            promiseSetters[i](maybePromise, holder);
                            holder.asyncNeeded = false;
                        } else if (((bitField & 33554432) !== 0)) {
                            callbacks[i].call(ret,
                                              maybePromise._value(), holder);
                        } else if (((bitField & 16777216) !== 0)) {
                            ret._reject(maybePromise._reason());
                        } else {
                            ret._cancel();
                        }
                    } else {
                        callbacks[i].call(ret, maybePromise, holder);
                    }
                }

                if (!ret._isFateSealed()) {
                    if (holder.asyncNeeded) {
                        var domain = getDomain();
                        if (domain !== null) {
                            holder.fn = util.domainBind(domain, holder.fn);
                        }
                    }
                    ret._setAsyncGuaranteed();
                    ret._setOnCancel(holder);
                }
                return ret;
            }
        }
    }
    var $_len = arguments.length;var args = new Array($_len); for(var $_i = 0; $_i < $_len; ++$_i) {args[$_i] = arguments[$_i];};
    if (fn) args.pop();
    var ret = new PromiseArray(args).promise();
    return fn !== undefined ? ret.spread(fn) : ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.longStackTraces"></a>[function <span class="apidocSignatureSpan">bluebird.</span>longStackTraces ()](#apidoc.element.bluebird.longStackTraces)
- description and source-code
```javascript
longStackTraces = function () {
    if (async.haveItemsQueued() && !config.longStackTraces) {
        throw new Error("cannot enable long stack traces after promises have been created\u000a\u000a    See http://goo.gl/MqrFmX\u000a");
    }
    if (!config.longStackTraces && longStackTracesIsSupported()) {
        var Promise_captureStackTrace = Promise.prototype._captureStackTrace;
        var Promise_attachExtraTrace = Promise.prototype._attachExtraTrace;
        config.longStackTraces = true;
        disableLongStackTraces = function() {
            if (async.haveItemsQueued() && !config.longStackTraces) {
                throw new Error("cannot enable long stack traces after promises have been created\u000a\u000a    See http://goo.
gl/MqrFmX\u000a");
            }
            Promise.prototype._captureStackTrace = Promise_captureStackTrace;
            Promise.prototype._attachExtraTrace = Promise_attachExtraTrace;
            Context.deactivateLongStackTraces();
            async.enableTrampoline();
            config.longStackTraces = false;
        };
        Promise.prototype._captureStackTrace = longStackTracesCaptureStackTrace;
        Promise.prototype._attachExtraTrace = longStackTracesAttachExtraTrace;
        Context.activateLongStackTraces();
        async.disableTrampolineIfNecessary();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.map"></a>[function <span class="apidocSignatureSpan">bluebird.</span>map (promises, fn, options, _filter)](#apidoc.element.bluebird.map)
- description and source-code
```javascript
map = function (promises, fn, options, _filter) {
    return map(promises, fn, options, _filter);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.mapSeries"></a>[function <span class="apidocSignatureSpan">bluebird.</span>mapSeries (promises, fn)](#apidoc.element.bluebird.mapSeries)
- description and source-code
```javascript
function PromiseMapSeries(promises, fn) {
    return PromiseReduce(promises, fn, INTERNAL, INTERNAL);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.method"></a>[function <span class="apidocSignatureSpan">bluebird.</span>method (fn)](#apidoc.element.bluebird.method)
- description and source-code
```javascript
method = function (fn) {
    if (typeof fn !== "function") {
        throw new Promise.TypeError("expecting a function but got " + util.classString(fn));
    }
    return function () {
        var ret = new Promise(INTERNAL);
        ret._captureStackTrace();
        ret._pushContext();
        var value = tryCatch(fn).apply(this, arguments);
        var promiseCreated = ret._popContext();
        debug.checkForgottenReturns(
            value, promiseCreated, "Promise.method", ret);
        ret._resolveFromSyncValue(value);
        return ret;
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.noConflict"></a>[function <span class="apidocSignatureSpan">bluebird.</span>noConflict ()](#apidoc.element.bluebird.noConflict)
- description and source-code
```javascript
function noConflict() {
    try { if (Promise === bluebird) Promise = old; }
    catch (e) {}
    return bluebird;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.onPossiblyUnhandledRejection"></a>[function <span class="apidocSignatureSpan">bluebird.</span>onPossiblyUnhandledRejection (fn)](#apidoc.element.bluebird.onPossiblyUnhandledRejection)
- description and source-code
```javascript
onPossiblyUnhandledRejection = function (fn) {
    var domain = getDomain();
    possiblyUnhandledRejection =
        typeof fn === "function" ? (domain === null ?
                                            fn : util.domainBind(domain, fn))
                                 : undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.onUnhandledRejectionHandled"></a>[function <span class="apidocSignatureSpan">bluebird.</span>onUnhandledRejectionHandled (fn)](#apidoc.element.bluebird.onUnhandledRejectionHandled)
- description and source-code
```javascript
onUnhandledRejectionHandled = function (fn) {
    var domain = getDomain();
    unhandledRejectionHandled =
        typeof fn === "function" ? (domain === null ?
                                            fn : util.domainBind(domain, fn))
                                 : undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.pending"></a>[function <span class="apidocSignatureSpan">bluebird.</span>pending ()](#apidoc.element.bluebird.pending)
- description and source-code
```javascript
pending = function () {
    debug.deprecated("Promise.defer", "new Promise");
    var promise = new Promise(INTERNAL);
    return {
        promise: promise,
        resolve: deferResolve,
        reject: deferReject
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.promisify"></a>[function <span class="apidocSignatureSpan">bluebird.</span>promisify (fn, options)](#apidoc.element.bluebird.promisify)
- description and source-code
```javascript
promisify = function (fn, options) {
    if (typeof fn !== "function") {
        throw new TypeError("expecting a function but got " + util.classString(fn));
    }
    if (isPromisified(fn)) {
        return fn;
    }
    options = Object(options);
    var receiver = options.context === undefined ? THIS : options.context;
    var multiArgs = !!options.multiArgs;
    var ret = promisify(fn, receiver, multiArgs);
    util.copyDescriptors(fn, ret, propsFilter);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.promisifyAll"></a>[function <span class="apidocSignatureSpan">bluebird.</span>promisifyAll (target, options)](#apidoc.element.bluebird.promisifyAll)
- description and source-code
```javascript
promisifyAll = function (target, options) {
    if (typeof target !== "function" && typeof target !== "object") {
        throw new TypeError("the target of promisifyAll must be an object or a function\u000a\u000a    See http://goo.gl/MqrFmX\
u000a");
    }
    options = Object(options);
    var multiArgs = !!options.multiArgs;
    var suffix = options.suffix;
    if (typeof suffix !== "string") suffix = defaultSuffix;
    var filter = options.filter;
    if (typeof filter !== "function") filter = defaultFilter;
    var promisifier = options.promisifier;
    if (typeof promisifier !== "function") promisifier = makeNodePromisified;

    if (!util.isIdentifier(suffix)) {
        throw new RangeError("suffix must be a valid identifier\u000a\u000a    See http://goo.gl/MqrFmX\u000a");
    }

    var keys = util.inheritedDataKeys(target);
    for (var i = 0; i < keys.length; ++i) {
        var value = target[keys[i]];
        if (keys[i] !== "constructor" &&
            util.isClass(value)) {
            promisifyAll(value.prototype, suffix, filter, promisifier,
                multiArgs);
            promisifyAll(value, suffix, filter, promisifier, multiArgs);
        }
    }

    return promisifyAll(target, suffix, filter, promisifier, multiArgs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.props"></a>[function <span class="apidocSignatureSpan">bluebird.</span>props (promises)](#apidoc.element.bluebird.props)
- description and source-code
```javascript
props = function (promises) {
    return props(promises);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.race"></a>[function <span class="apidocSignatureSpan">bluebird.</span>race (promises)](#apidoc.element.bluebird.race)
- description and source-code
```javascript
race = function (promises) {
    return race(promises, undefined);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.reduce"></a>[function <span class="apidocSignatureSpan">bluebird.</span>reduce (promises, fn, initialValue, _each)](#apidoc.element.bluebird.reduce)
- description and source-code
```javascript
reduce = function (promises, fn, initialValue, _each) {
    return reduce(promises, fn, initialValue, _each);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.reject"></a>[function <span class="apidocSignatureSpan">bluebird.</span>reject (reason)](#apidoc.element.bluebird.reject)
- description and source-code
```javascript
reject = function (reason) {
    var ret = new Promise(INTERNAL);
    ret._captureStackTrace();
    ret._rejectCallback(reason, true);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.rejected"></a>[function <span class="apidocSignatureSpan">bluebird.</span>rejected (reason)](#apidoc.element.bluebird.rejected)
- description and source-code
```javascript
rejected = function (reason) {
    var ret = new Promise(INTERNAL);
    ret._captureStackTrace();
    ret._rejectCallback(reason, true);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.resolve"></a>[function <span class="apidocSignatureSpan">bluebird.</span>resolve (obj)](#apidoc.element.bluebird.resolve)
- description and source-code
```javascript
resolve = function (obj) {
    var ret = tryConvertToPromise(obj);
    if (!(ret instanceof Promise)) {
        ret = new Promise(INTERNAL);
        ret._captureStackTrace();
        ret._setFulfilled();
        ret._rejectionHandler0 = obj;
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.setScheduler"></a>[function <span class="apidocSignatureSpan">bluebird.</span>setScheduler (fn)](#apidoc.element.bluebird.setScheduler)
- description and source-code
```javascript
setScheduler = function (fn) {
    if (typeof fn !== "function") {
        throw new TypeError("expecting a function but got " + util.classString(fn));
    }
    return async.setScheduler(fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.settle"></a>[function <span class="apidocSignatureSpan">bluebird.</span>settle (promises)](#apidoc.element.bluebird.settle)
- description and source-code
```javascript
settle = function (promises) {
    debug.deprecated(".settle()", ".reflect()");
    return new SettledPromiseArray(promises).promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.some"></a>[function <span class="apidocSignatureSpan">bluebird.</span>some (promises, howMany)](#apidoc.element.bluebird.some)
- description and source-code
```javascript
some = function (promises, howMany) {
    return some(promises, howMany);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.spawn"></a>[function <span class="apidocSignatureSpan">bluebird.</span>spawn (generatorFunction)](#apidoc.element.bluebird.spawn)
- description and source-code
```javascript
spawn = function (generatorFunction) {
    debug.deprecated("Promise.spawn()", "Promise.coroutine()");
    if (typeof generatorFunction !== "function") {
        return apiRejection("generatorFunction must be a function\u000a\u000a    See http://goo.gl/MqrFmX\u000a");
    }
    var spawn = new PromiseSpawn(generatorFunction, this);
    var ret = spawn.promise();
    spawn._run(Promise.spawn);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.try"></a>[function <span class="apidocSignatureSpan">bluebird.</span>try (fn)](#apidoc.element.bluebird.try)
- description and source-code
```javascript
try = function (fn) {
    if (typeof fn !== "function") {
        return apiRejection("expecting a function but got " + util.classString(fn));
    }
    var ret = new Promise(INTERNAL);
    ret._captureStackTrace();
    ret._pushContext();
    var value;
    if (arguments.length > 1) {
        debug.deprecated("calling Promise.try with more than 1 argument");
        var arg = arguments[1];
        var ctx = arguments[2];
        value = util.isArray(arg) ? tryCatch(fn).apply(ctx, arg)
                                  : tryCatch(fn).call(ctx, arg);
    } else {
        value = tryCatch(fn)();
    }
    var promiseCreated = ret._popContext();
    debug.checkForgottenReturns(
        value, promiseCreated, "Promise.try", ret);
    ret._resolveFromSyncValue(value);
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.using"></a>[function <span class="apidocSignatureSpan">bluebird.</span>using ()](#apidoc.element.bluebird.using)
- description and source-code
```javascript
using = function () {
    var len = arguments.length;
    if (len < 2) return apiRejection(
                    "you must pass at least 2 arguments to Promise.using");
    var fn = arguments[len - 1];
    if (typeof fn !== "function") {
        return apiRejection("expecting a function but got " + util.classString(fn));
    }
    var input;
    var spreadArgs = true;
    if (len === 2 && Array.isArray(arguments[0])) {
        input = arguments[0];
        len = input.length;
        spreadArgs = false;
    } else {
        input = arguments;
        len--;
    }
    var resources = new ResourceList(len);
    for (var i = 0; i < len; ++i) {
        var resource = input[i];
        if (Disposer.isDisposer(resource)) {
            var disposer = resource;
            resource = resource.promise();
            resource._setDisposable(disposer);
        } else {
            var maybePromise = tryConvertToPromise(resource);
            if (maybePromise instanceof Promise) {
                resource =
                    maybePromise._then(maybeUnwrapDisposer, null, null, {
                        resources: resources,
                        index: i
                }, undefined);
            }
        }
        resources[i] = resource;
    }

    var reflectedResources = new Array(resources.length);
    for (var i = 0; i < reflectedResources.length; ++i) {
        reflectedResources[i] = Promise.resolve(resources[i]).reflect();
    }

    var resultPromise = Promise.all(reflectedResources)
        .then(function(inspections) {
            for (var i = 0; i < inspections.length; ++i) {
                var inspection = inspections[i];
                if (inspection.isRejected()) {
                    errorObj.e = inspection.error();
                    return errorObj;
                } else if (!inspection.isFulfilled()) {
                    resultPromise.cancel();
                    return;
                }
                inspections[i] = inspection.value();
            }
            promise._pushContext();

            fn = tryCatch(fn);
            var ret = spreadArgs
                ? fn.apply(undefined, inspections) : fn(inspections);
            var promiseCreated = promise._popContext();
            debug.checkForgottenReturns(
                ret, promiseCreated, "Promise.using", promise);
            return ret;
        });

    var promise = resultPromise.lastly(function() {
        var inspection = new Promise.PromiseInspection(resultPromise);
        return dispose(resources, inspection);
    });
    resources.promise = promise;
    promise._setOnCancel(resources);
    return promise;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bluebird.AggregateError"></a>[module bluebird.AggregateError](#apidoc.module.bluebird.AggregateError)

#### <a name="apidoc.element.bluebird.AggregateError.AggregateError"></a>[function <span class="apidocSignatureSpan">bluebird.</span>AggregateError (message)](#apidoc.element.bluebird.AggregateError.AggregateError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bluebird.AggregateError.prototype"></a>[module bluebird.AggregateError.prototype](#apidoc.module.bluebird.AggregateError.prototype)

#### <a name="apidoc.element.bluebird.AggregateError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>constructor (message)](#apidoc.element.bluebird.AggregateError.prototype.constructor)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.AggregateError.prototype.every"></a>[function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>every ()](#apidoc.element.bluebird.AggregateError.prototype.every)
- description and source-code
```javascript
function every() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.AggregateError.prototype.filter"></a>[function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>filter ()](#apidoc.element.bluebird.AggregateError.prototype.filter)
- description and source-code
```javascript
function filter() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.AggregateError.prototype.forEach"></a>[function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>forEach ()](#apidoc.element.bluebird.AggregateError.prototype.forEach)
- description and source-code
```javascript
function forEach() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.AggregateError.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>indexOf ()](#apidoc.element.bluebird.AggregateError.prototype.indexOf)
- description and source-code
```javascript
function indexOf() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.AggregateError.prototype.join"></a>[function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>join ()](#apidoc.element.bluebird.AggregateError.prototype.join)
- description and source-code
```javascript
function join() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.AggregateError.prototype.lastIndexOf"></a>[function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>lastIndexOf ()](#apidoc.element.bluebird.AggregateError.prototype.lastIndexOf)
- description and source-code
```javascript
function lastIndexOf() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.AggregateError.prototype.map"></a>[function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>map ()](#apidoc.element.bluebird.AggregateError.prototype.map)
- description and source-code
```javascript
function map() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.AggregateError.prototype.pop"></a>[function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>pop ()](#apidoc.element.bluebird.AggregateError.prototype.pop)
- description and source-code
```javascript
function pop() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.AggregateError.prototype.push"></a>[function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>push ()](#apidoc.element.bluebird.AggregateError.prototype.push)
- description and source-code
```javascript
function push() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.AggregateError.prototype.reduce"></a>[function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>reduce ()](#apidoc.element.bluebird.AggregateError.prototype.reduce)
- description and source-code
```javascript
function reduce() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.AggregateError.prototype.reduceRight"></a>[function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>reduceRight ()](#apidoc.element.bluebird.AggregateError.prototype.reduceRight)
- description and source-code
```javascript
function reduceRight() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.AggregateError.prototype.reverse"></a>[function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>reverse ()](#apidoc.element.bluebird.AggregateError.prototype.reverse)
- description and source-code
```javascript
function reverse() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.AggregateError.prototype.shift"></a>[function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>shift ()](#apidoc.element.bluebird.AggregateError.prototype.shift)
- description and source-code
```javascript
function shift() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.AggregateError.prototype.slice"></a>[function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>slice ()](#apidoc.element.bluebird.AggregateError.prototype.slice)
- description and source-code
```javascript
function slice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.AggregateError.prototype.some"></a>[function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>some ()](#apidoc.element.bluebird.AggregateError.prototype.some)
- description and source-code
```javascript
function some() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.AggregateError.prototype.sort"></a>[function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>sort ()](#apidoc.element.bluebird.AggregateError.prototype.sort)
- description and source-code
```javascript
function sort() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.AggregateError.prototype.toString"></a>[function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>toString ()](#apidoc.element.bluebird.AggregateError.prototype.toString)
- description and source-code
```javascript
toString = function () {
    var indent = Array(level * 4 + 1).join(" ");
    var ret = "\n" + indent + "AggregateError of:" + "\n";
    level++;
    indent = Array(level * 4 + 1).join(" ");
    for (var i = 0; i < this.length; ++i) {
        var str = this[i] === this ? "[Circular AggregateError]" : this[i] + "";
        var lines = str.split("\n");
        for (var j = 0; j < lines.length; ++j) {
            lines[j] = indent + lines[j];
        }
        str = lines.join("\n");
        ret += str + "\n";
    }
    level--;
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.AggregateError.prototype.unshift"></a>[function <span class="apidocSignatureSpan">bluebird.AggregateError.prototype.</span>unshift ()](#apidoc.element.bluebird.AggregateError.prototype.unshift)
- description and source-code
```javascript
function unshift() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bluebird.CancellationError"></a>[module bluebird.CancellationError](#apidoc.module.bluebird.CancellationError)

#### <a name="apidoc.element.bluebird.CancellationError.CancellationError"></a>[function <span class="apidocSignatureSpan">bluebird.</span>CancellationError (message)](#apidoc.element.bluebird.CancellationError.CancellationError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bluebird.CancellationError.prototype"></a>[module bluebird.CancellationError.prototype](#apidoc.module.bluebird.CancellationError.prototype)

#### <a name="apidoc.element.bluebird.CancellationError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">bluebird.CancellationError.prototype.</span>constructor (message)](#apidoc.element.bluebird.CancellationError.prototype.constructor)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bluebird.OperationalError"></a>[module bluebird.OperationalError](#apidoc.module.bluebird.OperationalError)

#### <a name="apidoc.element.bluebird.OperationalError.OperationalError"></a>[function <span class="apidocSignatureSpan">bluebird.</span>OperationalError (message)](#apidoc.element.bluebird.OperationalError.OperationalError)
- description and source-code
```javascript
function OperationalError(message) {
    if (!(this instanceof OperationalError))
        return new OperationalError(message);
    notEnumerableProp(this, "name", "OperationalError");
    notEnumerableProp(this, "message", message);
    this.cause = message;
    this["isOperational"] = true;

    if (message instanceof Error) {
        notEnumerableProp(this, "message", message.message);
        notEnumerableProp(this, "stack", message.stack);
    } else if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    }

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bluebird.OperationalError.prototype"></a>[module bluebird.OperationalError.prototype](#apidoc.module.bluebird.OperationalError.prototype)

#### <a name="apidoc.element.bluebird.OperationalError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">bluebird.OperationalError.prototype.</span>constructor (message)](#apidoc.element.bluebird.OperationalError.prototype.constructor)
- description and source-code
```javascript
function OperationalError(message) {
    if (!(this instanceof OperationalError))
        return new OperationalError(message);
    notEnumerableProp(this, "name", "OperationalError");
    notEnumerableProp(this, "message", message);
    this.cause = message;
    this["isOperational"] = true;

    if (message instanceof Error) {
        notEnumerableProp(this, "message", message.message);
        notEnumerableProp(this, "stack", message.stack);
    } else if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    }

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bluebird.PromiseInspection"></a>[module bluebird.PromiseInspection](#apidoc.module.bluebird.PromiseInspection)

#### <a name="apidoc.element.bluebird.PromiseInspection.PromiseInspection"></a>[function <span class="apidocSignatureSpan">bluebird.</span>PromiseInspection (promise)](#apidoc.element.bluebird.PromiseInspection.PromiseInspection)
- description and source-code
```javascript
function PromiseInspection(promise) {
    if (promise !== undefined) {
        promise = promise._target();
        this._bitField = promise._bitField;
        this._settledValueField = promise._isFateSealed()
            ? promise._settledValue() : undefined;
    }
    else {
        this._bitField = 0;
        this._settledValueField = undefined;
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bluebird.PromiseInspection.prototype"></a>[module bluebird.PromiseInspection.prototype](#apidoc.module.bluebird.PromiseInspection.prototype)

#### <a name="apidoc.element.bluebird.PromiseInspection.prototype._settledValue"></a>[function <span class="apidocSignatureSpan">bluebird.PromiseInspection.prototype.</span>_settledValue ()](#apidoc.element.bluebird.PromiseInspection.prototype._settledValue)
- description and source-code
```javascript
_settledValue = function () {
    return this._settledValueField;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.PromiseInspection.prototype.error"></a>[function <span class="apidocSignatureSpan">bluebird.PromiseInspection.prototype.</span>error ()](#apidoc.element.bluebird.PromiseInspection.prototype.error)
- description and source-code
```javascript
error = function () {
    if (!this.isRejected()) {
        throw new TypeError("cannot get rejection reason of a non-rejected promise\u000a\u000a    See http://goo.gl/MqrFmX\u000a
");
    }
    return this._settledValue();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.PromiseInspection.prototype.isCancelled"></a>[function <span class="apidocSignatureSpan">bluebird.PromiseInspection.prototype.</span>isCancelled ()](#apidoc.element.bluebird.PromiseInspection.prototype.isCancelled)
- description and source-code
```javascript
isCancelled = function () {
    return (this._bitField & 8454144) !== 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.PromiseInspection.prototype.isFulfilled"></a>[function <span class="apidocSignatureSpan">bluebird.PromiseInspection.prototype.</span>isFulfilled ()](#apidoc.element.bluebird.PromiseInspection.prototype.isFulfilled)
- description and source-code
```javascript
isFulfilled = function () {
    return (this._bitField & 33554432) !== 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.PromiseInspection.prototype.isPending"></a>[function <span class="apidocSignatureSpan">bluebird.PromiseInspection.prototype.</span>isPending ()](#apidoc.element.bluebird.PromiseInspection.prototype.isPending)
- description and source-code
```javascript
isPending = function () {
    return (this._bitField & 50397184) === 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.PromiseInspection.prototype.isRejected"></a>[function <span class="apidocSignatureSpan">bluebird.PromiseInspection.prototype.</span>isRejected ()](#apidoc.element.bluebird.PromiseInspection.prototype.isRejected)
- description and source-code
```javascript
isRejected = function () {
    return (this._bitField & 16777216) !== 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.PromiseInspection.prototype.isResolved"></a>[function <span class="apidocSignatureSpan">bluebird.PromiseInspection.prototype.</span>isResolved ()](#apidoc.element.bluebird.PromiseInspection.prototype.isResolved)
- description and source-code
```javascript
isResolved = function () {
    return (this._bitField & 50331648) !== 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.PromiseInspection.prototype.reason"></a>[function <span class="apidocSignatureSpan">bluebird.PromiseInspection.prototype.</span>reason ()](#apidoc.element.bluebird.PromiseInspection.prototype.reason)
- description and source-code
```javascript
reason = function () {
    if (!this.isRejected()) {
        throw new TypeError("cannot get rejection reason of a non-rejected promise\u000a\u000a    See http://goo.gl/MqrFmX\u000a
");
    }
    return this._settledValue();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.PromiseInspection.prototype.value"></a>[function <span class="apidocSignatureSpan">bluebird.PromiseInspection.prototype.</span>value ()](#apidoc.element.bluebird.PromiseInspection.prototype.value)
- description and source-code
```javascript
value = function () {
    if (!this.isFulfilled()) {
        throw new TypeError("cannot get fulfillment value of a non-fulfilled promise\u000a\u000a    See http://goo.gl/MqrFmX\u000a
");
    }
    return this._settledValue();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bluebird.TimeoutError"></a>[module bluebird.TimeoutError](#apidoc.module.bluebird.TimeoutError)

#### <a name="apidoc.element.bluebird.TimeoutError.TimeoutError"></a>[function <span class="apidocSignatureSpan">bluebird.</span>TimeoutError (message)](#apidoc.element.bluebird.TimeoutError.TimeoutError)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bluebird.TimeoutError.prototype"></a>[module bluebird.TimeoutError.prototype](#apidoc.module.bluebird.TimeoutError.prototype)

#### <a name="apidoc.element.bluebird.TimeoutError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">bluebird.TimeoutError.prototype.</span>constructor (message)](#apidoc.element.bluebird.TimeoutError.prototype.constructor)
- description and source-code
```javascript
function SubError(message) {
    if (!(this instanceof SubError)) return new SubError(message);
    notEnumerableProp(this, "message",
        typeof message === "string" ? message : defaultMessage);
    notEnumerableProp(this, "name", nameProperty);
    if (Error.captureStackTrace) {
        Error.captureStackTrace(this, this.constructor);
    } else {
        Error.call(this);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bluebird._SomePromiseArray"></a>[module bluebird._SomePromiseArray](#apidoc.module.bluebird._SomePromiseArray)

#### <a name="apidoc.element.bluebird._SomePromiseArray._SomePromiseArray"></a>[function <span class="apidocSignatureSpan">bluebird.</span>_SomePromiseArray (values)](#apidoc.element.bluebird._SomePromiseArray._SomePromiseArray)
- description and source-code
```javascript
function SomePromiseArray(values) {
    this.constructor$(values);
    this._howMany = 0;
    this._unwrap = false;
    this._initialized = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bluebird._SomePromiseArray.prototype"></a>[module bluebird._SomePromiseArray.prototype](#apidoc.module.bluebird._SomePromiseArray.prototype)

#### <a name="apidoc.element.bluebird._SomePromiseArray.prototype._addFulfilled"></a>[function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_addFulfilled (value)](#apidoc.element.bluebird._SomePromiseArray.prototype._addFulfilled)
- description and source-code
```javascript
_addFulfilled = function (value) {
    this._values[this._totalResolved++] = value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird._SomePromiseArray.prototype._addRejected"></a>[function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_addRejected (reason)](#apidoc.element.bluebird._SomePromiseArray.prototype._addRejected)
- description and source-code
```javascript
_addRejected = function (reason) {
    this._values.push(reason);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird._SomePromiseArray.prototype._canPossiblyFulfill"></a>[function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_canPossiblyFulfill ()](#apidoc.element.bluebird._SomePromiseArray.prototype._canPossiblyFulfill)
- description and source-code
```javascript
_canPossiblyFulfill = function () {
    return this.length() - this._rejected();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird._SomePromiseArray.prototype._checkOutcome"></a>[function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_checkOutcome ()](#apidoc.element.bluebird._SomePromiseArray.prototype._checkOutcome)
- description and source-code
```javascript
_checkOutcome = function () {
    if (this.howMany() > this._canPossiblyFulfill()) {
        var e = new AggregateError();
        for (var i = this.length(); i < this._values.length; ++i) {
            if (this._values[i] !== CANCELLATION) {
                e.push(this._values[i]);
            }
        }
        if (e.length > 0) {
            this._reject(e);
        } else {
            this._cancel();
        }
        return true;
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird._SomePromiseArray.prototype._fulfilled"></a>[function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_fulfilled ()](#apidoc.element.bluebird._SomePromiseArray.prototype._fulfilled)
- description and source-code
```javascript
_fulfilled = function () {
    return this._totalResolved;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird._SomePromiseArray.prototype._getRangeError"></a>[function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_getRangeError (count)](#apidoc.element.bluebird._SomePromiseArray.prototype._getRangeError)
- description and source-code
```javascript
_getRangeError = function (count) {
    var message = "Input array must contain at least " +
            this._howMany + " items but contains only " + count + " items";
    return new RangeError(message);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird._SomePromiseArray.prototype._init"></a>[function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_init ()](#apidoc.element.bluebird._SomePromiseArray.prototype._init)
- description and source-code
```javascript
_init = function () {
    if (!this._initialized) {
        return;
    }
    if (this._howMany === 0) {
        this._resolve([]);
        return;
    }
    this._init$(undefined, -5);
    var isArrayResolved = isArray(this._values);
    if (!this._isResolved() &&
        isArrayResolved &&
        this._howMany > this._canPossiblyFulfill()) {
        this._reject(this._getRangeError(this.length()));
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird._SomePromiseArray.prototype._promiseCancelled"></a>[function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_promiseCancelled ()](#apidoc.element.bluebird._SomePromiseArray.prototype._promiseCancelled)
- description and source-code
```javascript
_promiseCancelled = function () {
    if (this._values instanceof Promise || this._values == null) {
        return this._cancel();
    }
    this._addRejected(CANCELLATION);
    return this._checkOutcome();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird._SomePromiseArray.prototype._promiseFulfilled"></a>[function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_promiseFulfilled (value)](#apidoc.element.bluebird._SomePromiseArray.prototype._promiseFulfilled)
- description and source-code
```javascript
_promiseFulfilled = function (value) {
    this._addFulfilled(value);
    if (this._fulfilled() === this.howMany()) {
        this._values.length = this.howMany();
        if (this.howMany() === 1 && this._unwrap) {
            this._resolve(this._values[0]);
        } else {
            this._resolve(this._values);
        }
        return true;
    }
    return false;

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird._SomePromiseArray.prototype._promiseRejected"></a>[function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_promiseRejected (reason)](#apidoc.element.bluebird._SomePromiseArray.prototype._promiseRejected)
- description and source-code
```javascript
_promiseRejected = function (reason) {
    this._addRejected(reason);
    return this._checkOutcome();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird._SomePromiseArray.prototype._rejected"></a>[function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_rejected ()](#apidoc.element.bluebird._SomePromiseArray.prototype._rejected)
- description and source-code
```javascript
_rejected = function () {
    return this._values.length - this.length();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird._SomePromiseArray.prototype._resolveEmptyArray"></a>[function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>_resolveEmptyArray ()](#apidoc.element.bluebird._SomePromiseArray.prototype._resolveEmptyArray)
- description and source-code
```javascript
_resolveEmptyArray = function () {
    this._reject(this._getRangeError(0));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird._SomePromiseArray.prototype.constructor"></a>[function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>constructor (values)](#apidoc.element.bluebird._SomePromiseArray.prototype.constructor)
- description and source-code
```javascript
function SomePromiseArray(values) {
    this.constructor$(values);
    this._howMany = 0;
    this._unwrap = false;
    this._initialized = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird._SomePromiseArray.prototype.howMany"></a>[function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>howMany ()](#apidoc.element.bluebird._SomePromiseArray.prototype.howMany)
- description and source-code
```javascript
howMany = function () {
    return this._howMany;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird._SomePromiseArray.prototype.init"></a>[function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>init ()](#apidoc.element.bluebird._SomePromiseArray.prototype.init)
- description and source-code
```javascript
init = function () {
    this._initialized = true;
    this._init();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird._SomePromiseArray.prototype.setHowMany"></a>[function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>setHowMany (count)](#apidoc.element.bluebird._SomePromiseArray.prototype.setHowMany)
- description and source-code
```javascript
setHowMany = function (count) {
    this._howMany = count;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird._SomePromiseArray.prototype.setUnwrap"></a>[function <span class="apidocSignatureSpan">bluebird._SomePromiseArray.prototype.</span>setUnwrap ()](#apidoc.element.bluebird._SomePromiseArray.prototype.setUnwrap)
- description and source-code
```javascript
setUnwrap = function () {
    this._unwrap = true;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bluebird.coroutine"></a>[module bluebird.coroutine](#apidoc.module.bluebird.coroutine)

#### <a name="apidoc.element.bluebird.coroutine.coroutine"></a>[function <span class="apidocSignatureSpan">bluebird.</span>coroutine (generatorFunction, options)](#apidoc.element.bluebird.coroutine.coroutine)
- description and source-code
```javascript
coroutine = function (generatorFunction, options) {
    if (typeof generatorFunction !== "function") {
        throw new TypeError("generatorFunction must be a function\u000a\u000a    See http://goo.gl/MqrFmX\u000a");
    }
    var yieldHandler = Object(options).yieldHandler;
    var PromiseSpawn$ = PromiseSpawn;
    var stack = new Error().stack;
    return function () {
        var generator = generatorFunction.apply(this, arguments);
        var spawn = new PromiseSpawn$(undefined, undefined, yieldHandler,
                                      stack);
        var ret = spawn.promise();
        spawn._generator = generator;
        spawn._promiseFulfilled(undefined);
        return ret;
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bluebird.coroutine.addYieldHandler"></a>[function <span class="apidocSignatureSpan">bluebird.coroutine.</span>addYieldHandler (fn)](#apidoc.element.bluebird.coroutine.addYieldHandler)
- description and source-code
```javascript
addYieldHandler = function (fn) {
    if (typeof fn !== "function") {
        throw new TypeError("expecting a function but got " + util.classString(fn));
    }
    yieldHandlers.push(fn);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
