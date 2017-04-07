# api documentation for  [passport-local-mongoose (v4.0.0)](https://github.com/saintedlama/passport-local-mongoose#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-passport-local-mongoose.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-passport-local-mongoose) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-passport-local-mongoose.svg)](https://travis-ci.org/npmdoc/node-npmdoc-passport-local-mongoose)
#### Mongoose plugin that simplifies building username and password login with Passport

[![NPM](https://nodei.co/npm/passport-local-mongoose.png?downloads=true)](https://www.npmjs.com/package/passport-local-mongoose)

[![apidoc](https://npmdoc.github.io/node-npmdoc-passport-local-mongoose/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-passport-local-mongoose_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-passport-local-mongoose/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-passport-local-mongoose/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-passport-local-mongoose/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Christoph Walcher",
        "email": "christoph.walcher@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/saintedlama/passport-local-mongoose/issues"
    },
    "dependencies": {
        "generaterr": "^1.2.0",
        "passport-local": "^1.0.0",
        "scmp": "^1.0.0",
        "semver": "^5.1.0"
    },
    "description": "Mongoose plugin that simplifies building username and password login with Passport",
    "devDependencies": {
        "chai": "^3.2.0",
        "mocha": "^2.3.2",
        "mongoose": "4.1.x",
        "shelljs": "^0.5.3"
    },
    "directories": {},
    "dist": {
        "shasum": "10fee927eaf9785bb2e10e2a8c446a0ff1fa0107",
        "tarball": "https://registry.npmjs.org/passport-local-mongoose/-/passport-local-mongoose-4.0.0.tgz"
    },
    "engines": {
        "node": ">= 0.12"
    },
    "gitHead": "0b5da93def0244a551188263bf473d48f3b95876",
    "homepage": "https://github.com/saintedlama/passport-local-mongoose#readme",
    "keywords": [
        "mongoose",
        "passport",
        "authentication",
        "login"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "saintedlama",
            "email": "christoph.walcher@gmail.com"
        }
    ],
    "name": "passport-local-mongoose",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/saintedlama/passport-local-mongoose.git"
    },
    "scripts": {
        "cover": "istanbul cover ./node_modules/mocha/bin/_mocha --report html -- -R spec",
        "release": "node release.js",
        "test": "mocha -R spec test/"
    },
    "version": "4.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module passport-local-mongoose](#apidoc.module.passport-local-mongoose)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.</span>errors.AttemptTooSoonError ()](#apidoc.element.passport-local-mongoose.errors.AttemptTooSoonError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.</span>errors.AuthenticationError ()](#apidoc.element.passport-local-mongoose.errors.AuthenticationError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.</span>errors.IncorrectPasswordError ()](#apidoc.element.passport-local-mongoose.errors.IncorrectPasswordError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.</span>errors.IncorrectUsernameError ()](#apidoc.element.passport-local-mongoose.errors.IncorrectUsernameError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.</span>errors.MissingPasswordError ()](#apidoc.element.passport-local-mongoose.errors.MissingPasswordError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.</span>errors.MissingUsernameError ()](#apidoc.element.passport-local-mongoose.errors.MissingUsernameError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.</span>errors.NoSaltValueStoredError ()](#apidoc.element.passport-local-mongoose.errors.NoSaltValueStoredError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.</span>errors.TooManyAttemptsError ()](#apidoc.element.passport-local-mongoose.errors.TooManyAttemptsError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.</span>errors.UserExistsError ()](#apidoc.element.passport-local-mongoose.errors.UserExistsError)
1.  object <span class="apidocSignatureSpan">passport-local-mongoose.</span>errors

#### [module passport-local-mongoose.errors](#apidoc.module.passport-local-mongoose.errors)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>AttemptTooSoonError ()](#apidoc.element.passport-local-mongoose.errors.AttemptTooSoonError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>AuthenticationError ()](#apidoc.element.passport-local-mongoose.errors.AuthenticationError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>IncorrectPasswordError ()](#apidoc.element.passport-local-mongoose.errors.IncorrectPasswordError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>IncorrectUsernameError ()](#apidoc.element.passport-local-mongoose.errors.IncorrectUsernameError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>MissingPasswordError ()](#apidoc.element.passport-local-mongoose.errors.MissingPasswordError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>MissingUsernameError ()](#apidoc.element.passport-local-mongoose.errors.MissingUsernameError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>NoSaltValueStoredError ()](#apidoc.element.passport-local-mongoose.errors.NoSaltValueStoredError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>TooManyAttemptsError ()](#apidoc.element.passport-local-mongoose.errors.TooManyAttemptsError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>UserExistsError ()](#apidoc.element.passport-local-mongoose.errors.UserExistsError)

#### [module passport-local-mongoose.errors.AttemptTooSoonError](#apidoc.module.passport-local-mongoose.errors.AttemptTooSoonError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>AttemptTooSoonError ()](#apidoc.element.passport-local-mongoose.errors.AttemptTooSoonError.AttemptTooSoonError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.AttemptTooSoonError.</span>super_ ()](#apidoc.element.passport-local-mongoose.errors.AttemptTooSoonError.super_)

#### [module passport-local-mongoose.errors.AuthenticationError](#apidoc.module.passport-local-mongoose.errors.AuthenticationError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>AuthenticationError ()](#apidoc.element.passport-local-mongoose.errors.AuthenticationError.AuthenticationError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.AuthenticationError.</span>super_ ()](#apidoc.element.passport-local-mongoose.errors.AuthenticationError.super_)

#### [module passport-local-mongoose.errors.IncorrectPasswordError](#apidoc.module.passport-local-mongoose.errors.IncorrectPasswordError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>IncorrectPasswordError ()](#apidoc.element.passport-local-mongoose.errors.IncorrectPasswordError.IncorrectPasswordError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.IncorrectPasswordError.</span>super_ ()](#apidoc.element.passport-local-mongoose.errors.IncorrectPasswordError.super_)

#### [module passport-local-mongoose.errors.IncorrectUsernameError](#apidoc.module.passport-local-mongoose.errors.IncorrectUsernameError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>IncorrectUsernameError ()](#apidoc.element.passport-local-mongoose.errors.IncorrectUsernameError.IncorrectUsernameError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.IncorrectUsernameError.</span>super_ ()](#apidoc.element.passport-local-mongoose.errors.IncorrectUsernameError.super_)

#### [module passport-local-mongoose.errors.MissingPasswordError](#apidoc.module.passport-local-mongoose.errors.MissingPasswordError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>MissingPasswordError ()](#apidoc.element.passport-local-mongoose.errors.MissingPasswordError.MissingPasswordError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.MissingPasswordError.</span>super_ ()](#apidoc.element.passport-local-mongoose.errors.MissingPasswordError.super_)

#### [module passport-local-mongoose.errors.MissingUsernameError](#apidoc.module.passport-local-mongoose.errors.MissingUsernameError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>MissingUsernameError ()](#apidoc.element.passport-local-mongoose.errors.MissingUsernameError.MissingUsernameError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.MissingUsernameError.</span>super_ ()](#apidoc.element.passport-local-mongoose.errors.MissingUsernameError.super_)

#### [module passport-local-mongoose.errors.NoSaltValueStoredError](#apidoc.module.passport-local-mongoose.errors.NoSaltValueStoredError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>NoSaltValueStoredError ()](#apidoc.element.passport-local-mongoose.errors.NoSaltValueStoredError.NoSaltValueStoredError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.NoSaltValueStoredError.</span>super_ ()](#apidoc.element.passport-local-mongoose.errors.NoSaltValueStoredError.super_)

#### [module passport-local-mongoose.errors.TooManyAttemptsError](#apidoc.module.passport-local-mongoose.errors.TooManyAttemptsError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>TooManyAttemptsError ()](#apidoc.element.passport-local-mongoose.errors.TooManyAttemptsError.TooManyAttemptsError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.TooManyAttemptsError.</span>super_ ()](#apidoc.element.passport-local-mongoose.errors.TooManyAttemptsError.super_)

#### [module passport-local-mongoose.errors.UserExistsError](#apidoc.module.passport-local-mongoose.errors.UserExistsError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>UserExistsError ()](#apidoc.element.passport-local-mongoose.errors.UserExistsError.UserExistsError)
1.  [function <span class="apidocSignatureSpan">passport-local-mongoose.errors.UserExistsError.</span>super_ ()](#apidoc.element.passport-local-mongoose.errors.UserExistsError.super_)



# <a name="apidoc.module.passport-local-mongoose"></a>[module passport-local-mongoose](#apidoc.module.passport-local-mongoose)

#### <a name="apidoc.element.passport-local-mongoose.errors.AttemptTooSoonError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.</span>errors.AttemptTooSoonError ()](#apidoc.element.passport-local-mongoose.errors.AttemptTooSoonError)
- description and source-code
```javascript
errors.AttemptTooSoonError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-local-mongoose.errors.AuthenticationError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.</span>errors.AuthenticationError ()](#apidoc.element.passport-local-mongoose.errors.AuthenticationError)
- description and source-code
```javascript
errors.AuthenticationError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-local-mongoose.errors.IncorrectPasswordError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.</span>errors.IncorrectPasswordError ()](#apidoc.element.passport-local-mongoose.errors.IncorrectPasswordError)
- description and source-code
```javascript
errors.IncorrectPasswordError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-local-mongoose.errors.IncorrectUsernameError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.</span>errors.IncorrectUsernameError ()](#apidoc.element.passport-local-mongoose.errors.IncorrectUsernameError)
- description and source-code
```javascript
errors.IncorrectUsernameError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-local-mongoose.errors.MissingPasswordError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.</span>errors.MissingPasswordError ()](#apidoc.element.passport-local-mongoose.errors.MissingPasswordError)
- description and source-code
```javascript
errors.MissingPasswordError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-local-mongoose.errors.MissingUsernameError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.</span>errors.MissingUsernameError ()](#apidoc.element.passport-local-mongoose.errors.MissingUsernameError)
- description and source-code
```javascript
errors.MissingUsernameError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-local-mongoose.errors.NoSaltValueStoredError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.</span>errors.NoSaltValueStoredError ()](#apidoc.element.passport-local-mongoose.errors.NoSaltValueStoredError)
- description and source-code
```javascript
errors.NoSaltValueStoredError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-local-mongoose.errors.TooManyAttemptsError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.</span>errors.TooManyAttemptsError ()](#apidoc.element.passport-local-mongoose.errors.TooManyAttemptsError)
- description and source-code
```javascript
errors.TooManyAttemptsError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-local-mongoose.errors.UserExistsError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.</span>errors.UserExistsError ()](#apidoc.element.passport-local-mongoose.errors.UserExistsError)
- description and source-code
```javascript
errors.UserExistsError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-local-mongoose.errors"></a>[module passport-local-mongoose.errors](#apidoc.module.passport-local-mongoose.errors)

#### <a name="apidoc.element.passport-local-mongoose.errors.AttemptTooSoonError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>AttemptTooSoonError ()](#apidoc.element.passport-local-mongoose.errors.AttemptTooSoonError)
- description and source-code
```javascript
AttemptTooSoonError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
...
if (options.limitAttempts) {
  var attemptsInterval = Math.pow(options.interval, Math.log(user.get(options.attemptsField) + 1));
  var calculatedInterval = (attemptsInterval < options.maxInterval) ? attemptsInterval : options.maxInterval;

  if (Date.now() - user.get(options.lastLoginField) < calculatedInterval) {
    user.set(options.lastLoginField, Date.now());
    user.save();
    return cb(null, false, new errors.AttemptTooSoonError(options.errorMessages.AttemptTooSoonError));
  }

  if (user.get(options.attemptsField) >= options.maxAttempts) {
    return cb(null, false, new errors.TooManyAttemptsError(options.errorMessages.TooManyAttemptsError));
  }
}
...
```

#### <a name="apidoc.element.passport-local-mongoose.errors.AuthenticationError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>AuthenticationError ()](#apidoc.element.passport-local-mongoose.errors.AuthenticationError)
- description and source-code
```javascript
AuthenticationError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-local-mongoose.errors.IncorrectPasswordError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>IncorrectPasswordError ()](#apidoc.element.passport-local-mongoose.errors.IncorrectPasswordError)
- description and source-code
```javascript
IncorrectPasswordError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
...
      user.set(options.lastLoginField, Date.now());
      user.set(options.attemptsField, user.get(options.attemptsField) + 1);
      user.save(function(saveErr) {
        if (saveErr) { return cb(saveErr); }
        if (user.get(options.attemptsField) >= options.maxAttempts) {
          return cb(null, false, new errors.TooManyAttemptsError(options.errorMessages.TooManyAttemptsError));
        } else {
          return cb(null, false, new errors.IncorrectPasswordError(options.errorMessages.IncorrectPasswordError));
        }
      });
    } else {
      return cb(null, false, new errors.IncorrectPasswordError(options.errorMessages.IncorrectPasswordError));
    }
  }
});
...
```

#### <a name="apidoc.element.passport-local-mongoose.errors.IncorrectUsernameError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>IncorrectUsernameError ()](#apidoc.element.passport-local-mongoose.errors.IncorrectUsernameError)
- description and source-code
```javascript
IncorrectUsernameError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
...
  if (!self.get(options.saltField)) {
    self.constructor.findByUsername(self.get(options.usernameField), true, function(err, user) {
      if (err) { return cb(err); }

      if (user) {
        return authenticate(user, password, cb);
      } else {
        return cb(null, false, new errors.IncorrectUsernameError(options.errorMessages.IncorrectUsernameError));
      }
    });
  } else {
    return authenticate(self, password, cb);
  }
};
...
```

#### <a name="apidoc.element.passport-local-mongoose.errors.MissingPasswordError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>MissingPasswordError ()](#apidoc.element.passport-local-mongoose.errors.MissingPasswordError)
- description and source-code
```javascript
MissingPasswordError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
...
}

next();
  });

  schema.methods.setPassword = function(password, cb) {
if (!password) {
  return cb(new errors.MissingPasswordError(options.errorMessages.MissingPasswordError));
}

var self = this;

options.passwordValidator(password, function(err) {
  if (err) {
    return cb(err);
...
```

#### <a name="apidoc.element.passport-local-mongoose.errors.MissingUsernameError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>MissingUsernameError ()](#apidoc.element.passport-local-mongoose.errors.MissingUsernameError)
- description and source-code
```javascript
MissingUsernameError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
...
  schema.statics.register = function(user, password, cb) {
    // Create an instance of this in case user isn't already an instance
    if (!(user instanceof this)) {
user = new this(user);
    }

    if (!user.get(options.usernameField)) {
return cb(new errors.MissingUsernameError(options.errorMessages.MissingUsernameError));
    }

    var self = this;
    self.findByUsername(user.get(options.usernameField), function(err, existingUser) {
if (err) { return cb(err); }

if (existingUser) {
...
```

#### <a name="apidoc.element.passport-local-mongoose.errors.NoSaltValueStoredError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>NoSaltValueStoredError ()](#apidoc.element.passport-local-mongoose.errors.NoSaltValueStoredError)
- description and source-code
```javascript
NoSaltValueStoredError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
...

  if (user.get(options.attemptsField) >= options.maxAttempts) {
    return cb(null, false, new errors.TooManyAttemptsError(options.errorMessages.TooManyAttemptsError));
  }
}

if (!user.get(options.saltField)) {
  return cb(null, false, new errors.NoSaltValueStoredError(options.errorMessages.NoSaltValueStoredError));
}

pbkdf2(password, user.get(options.saltField), function(err, hashRaw) {
  if (err) {
    return cb(err);
  }
...
```

#### <a name="apidoc.element.passport-local-mongoose.errors.TooManyAttemptsError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>TooManyAttemptsError ()](#apidoc.element.passport-local-mongoose.errors.TooManyAttemptsError)
- description and source-code
```javascript
TooManyAttemptsError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
...
  if (Date.now() - user.get(options.lastLoginField) < calculatedInterval) {
    user.set(options.lastLoginField, Date.now());
    user.save();
    return cb(null, false, new errors.AttemptTooSoonError(options.errorMessages.AttemptTooSoonError));
  }

  if (user.get(options.attemptsField) >= options.maxAttempts) {
    return cb(null, false, new errors.TooManyAttemptsError(options.errorMessages.TooManyAttemptsError));
  }
}

if (!user.get(options.saltField)) {
  return cb(null, false, new errors.NoSaltValueStoredError(options.errorMessages.NoSaltValueStoredError));
}
...
```

#### <a name="apidoc.element.passport-local-mongoose.errors.UserExistsError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>UserExistsError ()](#apidoc.element.passport-local-mongoose.errors.UserExistsError)
- description and source-code
```javascript
UserExistsError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
...
    }

    var self = this;
    self.findByUsername(user.get(options.usernameField), function(err, existingUser) {
if (err) { return cb(err); }

if (existingUser) {
  return cb(new errors.UserExistsError(options.errorMessages.UserExistsError));
}

user.setPassword(password, function(setPasswordErr, user) {
  if (setPasswordErr) {
    return cb(setPasswordErr);
  }
...
```



# <a name="apidoc.module.passport-local-mongoose.errors.AttemptTooSoonError"></a>[module passport-local-mongoose.errors.AttemptTooSoonError](#apidoc.module.passport-local-mongoose.errors.AttemptTooSoonError)

#### <a name="apidoc.element.passport-local-mongoose.errors.AttemptTooSoonError.AttemptTooSoonError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>AttemptTooSoonError ()](#apidoc.element.passport-local-mongoose.errors.AttemptTooSoonError.AttemptTooSoonError)
- description and source-code
```javascript
AttemptTooSoonError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
...
if (options.limitAttempts) {
  var attemptsInterval = Math.pow(options.interval, Math.log(user.get(options.attemptsField) + 1));
  var calculatedInterval = (attemptsInterval < options.maxInterval) ? attemptsInterval : options.maxInterval;

  if (Date.now() - user.get(options.lastLoginField) < calculatedInterval) {
    user.set(options.lastLoginField, Date.now());
    user.save();
    return cb(null, false, new errors.AttemptTooSoonError(options.errorMessages.AttemptTooSoonError));
  }

  if (user.get(options.attemptsField) >= options.maxAttempts) {
    return cb(null, false, new errors.TooManyAttemptsError(options.errorMessages.TooManyAttemptsError));
  }
}
...
```

#### <a name="apidoc.element.passport-local-mongoose.errors.AttemptTooSoonError.super_"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.AttemptTooSoonError.</span>super_ ()](#apidoc.element.passport-local-mongoose.errors.AttemptTooSoonError.super_)
- description and source-code
```javascript
super_ = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-local-mongoose.errors.AuthenticationError"></a>[module passport-local-mongoose.errors.AuthenticationError](#apidoc.module.passport-local-mongoose.errors.AuthenticationError)

#### <a name="apidoc.element.passport-local-mongoose.errors.AuthenticationError.AuthenticationError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>AuthenticationError ()](#apidoc.element.passport-local-mongoose.errors.AuthenticationError.AuthenticationError)
- description and source-code
```javascript
AuthenticationError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-local-mongoose.errors.AuthenticationError.super_"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.AuthenticationError.</span>super_ ()](#apidoc.element.passport-local-mongoose.errors.AuthenticationError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-local-mongoose.errors.IncorrectPasswordError"></a>[module passport-local-mongoose.errors.IncorrectPasswordError](#apidoc.module.passport-local-mongoose.errors.IncorrectPasswordError)

#### <a name="apidoc.element.passport-local-mongoose.errors.IncorrectPasswordError.IncorrectPasswordError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>IncorrectPasswordError ()](#apidoc.element.passport-local-mongoose.errors.IncorrectPasswordError.IncorrectPasswordError)
- description and source-code
```javascript
IncorrectPasswordError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
...
      user.set(options.lastLoginField, Date.now());
      user.set(options.attemptsField, user.get(options.attemptsField) + 1);
      user.save(function(saveErr) {
        if (saveErr) { return cb(saveErr); }
        if (user.get(options.attemptsField) >= options.maxAttempts) {
          return cb(null, false, new errors.TooManyAttemptsError(options.errorMessages.TooManyAttemptsError));
        } else {
          return cb(null, false, new errors.IncorrectPasswordError(options.errorMessages.IncorrectPasswordError));
        }
      });
    } else {
      return cb(null, false, new errors.IncorrectPasswordError(options.errorMessages.IncorrectPasswordError));
    }
  }
});
...
```

#### <a name="apidoc.element.passport-local-mongoose.errors.IncorrectPasswordError.super_"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.IncorrectPasswordError.</span>super_ ()](#apidoc.element.passport-local-mongoose.errors.IncorrectPasswordError.super_)
- description and source-code
```javascript
super_ = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-local-mongoose.errors.IncorrectUsernameError"></a>[module passport-local-mongoose.errors.IncorrectUsernameError](#apidoc.module.passport-local-mongoose.errors.IncorrectUsernameError)

#### <a name="apidoc.element.passport-local-mongoose.errors.IncorrectUsernameError.IncorrectUsernameError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>IncorrectUsernameError ()](#apidoc.element.passport-local-mongoose.errors.IncorrectUsernameError.IncorrectUsernameError)
- description and source-code
```javascript
IncorrectUsernameError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
...
  if (!self.get(options.saltField)) {
    self.constructor.findByUsername(self.get(options.usernameField), true, function(err, user) {
      if (err) { return cb(err); }

      if (user) {
        return authenticate(user, password, cb);
      } else {
        return cb(null, false, new errors.IncorrectUsernameError(options.errorMessages.IncorrectUsernameError));
      }
    });
  } else {
    return authenticate(self, password, cb);
  }
};
...
```

#### <a name="apidoc.element.passport-local-mongoose.errors.IncorrectUsernameError.super_"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.IncorrectUsernameError.</span>super_ ()](#apidoc.element.passport-local-mongoose.errors.IncorrectUsernameError.super_)
- description and source-code
```javascript
super_ = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-local-mongoose.errors.MissingPasswordError"></a>[module passport-local-mongoose.errors.MissingPasswordError](#apidoc.module.passport-local-mongoose.errors.MissingPasswordError)

#### <a name="apidoc.element.passport-local-mongoose.errors.MissingPasswordError.MissingPasswordError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>MissingPasswordError ()](#apidoc.element.passport-local-mongoose.errors.MissingPasswordError.MissingPasswordError)
- description and source-code
```javascript
MissingPasswordError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
...
}

next();
  });

  schema.methods.setPassword = function(password, cb) {
if (!password) {
  return cb(new errors.MissingPasswordError(options.errorMessages.MissingPasswordError));
}

var self = this;

options.passwordValidator(password, function(err) {
  if (err) {
    return cb(err);
...
```

#### <a name="apidoc.element.passport-local-mongoose.errors.MissingPasswordError.super_"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.MissingPasswordError.</span>super_ ()](#apidoc.element.passport-local-mongoose.errors.MissingPasswordError.super_)
- description and source-code
```javascript
super_ = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-local-mongoose.errors.MissingUsernameError"></a>[module passport-local-mongoose.errors.MissingUsernameError](#apidoc.module.passport-local-mongoose.errors.MissingUsernameError)

#### <a name="apidoc.element.passport-local-mongoose.errors.MissingUsernameError.MissingUsernameError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>MissingUsernameError ()](#apidoc.element.passport-local-mongoose.errors.MissingUsernameError.MissingUsernameError)
- description and source-code
```javascript
MissingUsernameError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
...
  schema.statics.register = function(user, password, cb) {
    // Create an instance of this in case user isn't already an instance
    if (!(user instanceof this)) {
user = new this(user);
    }

    if (!user.get(options.usernameField)) {
return cb(new errors.MissingUsernameError(options.errorMessages.MissingUsernameError));
    }

    var self = this;
    self.findByUsername(user.get(options.usernameField), function(err, existingUser) {
if (err) { return cb(err); }

if (existingUser) {
...
```

#### <a name="apidoc.element.passport-local-mongoose.errors.MissingUsernameError.super_"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.MissingUsernameError.</span>super_ ()](#apidoc.element.passport-local-mongoose.errors.MissingUsernameError.super_)
- description and source-code
```javascript
super_ = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-local-mongoose.errors.NoSaltValueStoredError"></a>[module passport-local-mongoose.errors.NoSaltValueStoredError](#apidoc.module.passport-local-mongoose.errors.NoSaltValueStoredError)

#### <a name="apidoc.element.passport-local-mongoose.errors.NoSaltValueStoredError.NoSaltValueStoredError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>NoSaltValueStoredError ()](#apidoc.element.passport-local-mongoose.errors.NoSaltValueStoredError.NoSaltValueStoredError)
- description and source-code
```javascript
NoSaltValueStoredError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
...

  if (user.get(options.attemptsField) >= options.maxAttempts) {
    return cb(null, false, new errors.TooManyAttemptsError(options.errorMessages.TooManyAttemptsError));
  }
}

if (!user.get(options.saltField)) {
  return cb(null, false, new errors.NoSaltValueStoredError(options.errorMessages.NoSaltValueStoredError));
}

pbkdf2(password, user.get(options.saltField), function(err, hashRaw) {
  if (err) {
    return cb(err);
  }
...
```

#### <a name="apidoc.element.passport-local-mongoose.errors.NoSaltValueStoredError.super_"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.NoSaltValueStoredError.</span>super_ ()](#apidoc.element.passport-local-mongoose.errors.NoSaltValueStoredError.super_)
- description and source-code
```javascript
super_ = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-local-mongoose.errors.TooManyAttemptsError"></a>[module passport-local-mongoose.errors.TooManyAttemptsError](#apidoc.module.passport-local-mongoose.errors.TooManyAttemptsError)

#### <a name="apidoc.element.passport-local-mongoose.errors.TooManyAttemptsError.TooManyAttemptsError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>TooManyAttemptsError ()](#apidoc.element.passport-local-mongoose.errors.TooManyAttemptsError.TooManyAttemptsError)
- description and source-code
```javascript
TooManyAttemptsError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
...
  if (Date.now() - user.get(options.lastLoginField) < calculatedInterval) {
    user.set(options.lastLoginField, Date.now());
    user.save();
    return cb(null, false, new errors.AttemptTooSoonError(options.errorMessages.AttemptTooSoonError));
  }

  if (user.get(options.attemptsField) >= options.maxAttempts) {
    return cb(null, false, new errors.TooManyAttemptsError(options.errorMessages.TooManyAttemptsError));
  }
}

if (!user.get(options.saltField)) {
  return cb(null, false, new errors.NoSaltValueStoredError(options.errorMessages.NoSaltValueStoredError));
}
...
```

#### <a name="apidoc.element.passport-local-mongoose.errors.TooManyAttemptsError.super_"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.TooManyAttemptsError.</span>super_ ()](#apidoc.element.passport-local-mongoose.errors.TooManyAttemptsError.super_)
- description and source-code
```javascript
super_ = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-local-mongoose.errors.UserExistsError"></a>[module passport-local-mongoose.errors.UserExistsError](#apidoc.module.passport-local-mongoose.errors.UserExistsError)

#### <a name="apidoc.element.passport-local-mongoose.errors.UserExistsError.UserExistsError"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.</span>UserExistsError ()](#apidoc.element.passport-local-mongoose.errors.UserExistsError.UserExistsError)
- description and source-code
```javascript
UserExistsError = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
...
    }

    var self = this;
    self.findByUsername(user.get(options.usernameField), function(err, existingUser) {
if (err) { return cb(err); }

if (existingUser) {
  return cb(new errors.UserExistsError(options.errorMessages.UserExistsError));
}

user.setPassword(password, function(setPasswordErr, user) {
  if (setPasswordErr) {
    return cb(setPasswordErr);
  }
...
```

#### <a name="apidoc.element.passport-local-mongoose.errors.UserExistsError.super_"></a>[function <span class="apidocSignatureSpan">passport-local-mongoose.errors.UserExistsError.</span>super_ ()](#apidoc.element.passport-local-mongoose.errors.UserExistsError.super_)
- description and source-code
```javascript
super_ = function () {
  if (!(this instanceof ctor)) {
    var constructorArgs = Array.prototype.slice.call(arguments);
    constructorArgs.unshift(ctor);

    return new (ctor.bind.apply(ctor, constructorArgs))();
  }

  options.inherits.call(this);

  if (options.captureStackTrace) {
    Error.captureStackTrace && Error.captureStackTrace(this, arguments.callee);
  }

  copy(parameters, this);

  var msg = arguments[0];
  if (msg) {
    var args = Array.prototype.slice.call(arguments);

    if (args.length > 1 && typeof args[args.length - 1] == 'object') {
      var instanceParams = args.pop();

      copy(instanceParams, this);
    }

    this.message = util.format.apply(util, args);
  }

  this.name = name;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
