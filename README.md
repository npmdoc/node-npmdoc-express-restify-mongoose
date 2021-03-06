# npmdoc-express-restify-mongoose

#### api documentation for  [express-restify-mongoose (v4.1.3)](http://florianholzapfel.github.io/express-restify-mongoose/)  [![npm package](https://img.shields.io/npm/v/npmdoc-express-restify-mongoose.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-express-restify-mongoose) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-express-restify-mongoose.svg)](https://travis-ci.org/npmdoc/node-npmdoc-express-restify-mongoose)

#### Easily create a flexible REST interface for mongoose models

[![NPM](https://nodei.co/npm/express-restify-mongoose.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/express-restify-mongoose)

- [https://npmdoc.github.io/node-npmdoc-express-restify-mongoose/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-express-restify-mongoose/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-express-restify-mongoose/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-express-restify-mongoose/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-express-restify-mongoose/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-express-restify-mongoose/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Florian Holzapfel"
    },
    "bugs": {
        "url": "https://github.com/florianholzapfel/express-restify-mongoose/issues"
    },
    "dependencies": {
        "async": "~2.1.0",
        "bluebird": "~3.4.0",
        "is-coordinates": "~1.0.0",
        "lodash": "~4.16.0",
        "mongoose-detective": "~0.1.0",
        "moredots": "~0.1.0",
        "serialize-error": "~2.0.0",
        "weedout": "~0.1.0"
    },
    "description": "Easily create a flexible REST interface for mongoose models",
    "devDependencies": {
        "babel-cli": "^6.6.0",
        "babel-core": "^6.7.0",
        "babel-preset-es2015": "^6.6.0",
        "body-parser": "^1.15.0",
        "express": "^4.13.0",
        "in-publish": "^2.0.0",
        "istanbul": ">=1.0.0-alpha.2",
        "method-override": "^2.3.0",
        "mocha": "^3.0.0",
        "request": "^2.69.0",
        "restify": "^3.0.0",
        "sinon": "^1.17.0",
        "standard": "^8.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "68ea3ecde1dc57123683efdf8b8e9237a984613b",
        "tarball": "https://registry.npmjs.org/express-restify-mongoose/-/express-restify-mongoose-4.1.3.tgz"
    },
    "engines": {
        "node": ">=0.10"
    },
    "files": [
        "CHANGELOG.md",
        "LICENSE",
        "README.md",
        "lib/"
    ],
    "gitHead": "e8e4063b042a1c3efc3821502b08fc6abee31fb6",
    "homepage": "http://florianholzapfel.github.io/express-restify-mongoose/",
    "keywords": [
        "ReST",
        "express",
        "restify",
        "mongodb",
        "mongoose",
        "model"
    ],
    "license": "MIT",
    "main": "./lib/express-restify-mongoose",
    "maintainers": [
        {
            "name": "fholzapfel"
        },
        {
            "name": "zertz"
        }
    ],
    "name": "express-restify-mongoose",
    "optionalDependencies": {},
    "peerDependencies": {
        "mongoose": "^4.0.0"
    },
    "repository": {
        "type": "git",
        "url": "git://github.com/florianholzapfel/express-restify-mongoose.git"
    },
    "scripts": {
        "compile": "babel src -d lib --source-maps both",
        "lint": "standard",
        "prepublish": "in-publish && npm test || not-in-publish",
        "pretest": "npm run lint && npm run compile",
        "report-coverage": "cat ./coverage/lcov.info | coveralls",
        "test": "npm run test-unit && npm run test-filter && npm run test-express && npm run test-restify",
        "test-ci": "npm run test-unit && npm run test-filter && npm run test-cov-express && npm run test-restify",
        "test-cov-express": "istanbul cover node_modules/mocha/bin/_mocha -- --compilers js:babel-core/register -R spec ./test/express.js --timeout 10s",
        "test-cov-restify": "istanbul cover node_modules/mocha/bin/_mocha -- --compilers js:babel-core/register -R spec ./test/restify.js --timeout 10s",
        "test-cov-unit": "istanbul cover node_modules/mocha/bin/_mocha -- --compilers js:babel-core/register -R spec ./test/unit.js",
        "test-express": "mocha -R spec ./test/express.js --compilers js:babel-core/register --timeout 10s",
        "test-filter": "mocha -R spec ./test/integration/resource_filter.js --compilers js:babel-core/register --timeout 10s",
        "test-restify": "mocha -R spec ./test/restify.js --compilers js:babel-core/register --timeout 10s",
        "test-unit": "mocha --compilers js:babel-core/register -R spec ./test/unit.js"
    },
    "standard": {
        "ignore": [
            "lib"
        ],
        "globals": [
            "describe",
            "before",
            "beforeEach",
            "after",
            "afterEach",
            "it"
        ]
    },
    "version": "4.1.3"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
