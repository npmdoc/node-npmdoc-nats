# npmdoc-nats

#### basic api documentation for  [nats (v0.7.16)](https://nats.io)  [![npm package](https://img.shields.io/npm/v/npmdoc-nats.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-nats) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-nats.svg)](https://travis-ci.org/npmdoc/node-npmdoc-nats)

#### Node.js client for NATS, a lightweight, high-performance cloud native messaging system

[![NPM](https://nodei.co/npm/nats.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/nats)

- [https://npmdoc.github.io/node-npmdoc-nats/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-nats/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-nats/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-nats/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-nats/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-nats/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Derek Collison"
    },
    "bugs": {
        "url": "https://github.com/nats-io/node-nats/issues"
    },
    "contributors": [],
    "dependencies": {
        "nuid": ">=0.6.8"
    },
    "description": "Node.js client for NATS, a lightweight, high-performance cloud native messaging system",
    "devDependencies": {
        "coveralls": "^2.11.2",
        "dependency-check": "2.5.x",
        "istanbul": "0.4.x",
        "jshint": "2.9.x",
        "jshint-stylish": "2.2.x",
        "mocha": "2.5.x",
        "mocha-lcov-reporter": "1.2.x",
        "mocha-multi": "0.9.x",
        "should": ">= 9.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "7e4c35ee79a33a3d2fabcdaa6c17c3e6f00069e5",
        "tarball": "https://registry.npmjs.org/nats/-/nats-0.7.16.tgz"
    },
    "engines": {
        "node": ">= 0.10.x"
    },
    "gitHead": "1fff062a3608629a6b02c0613b1a7712920eb4dd",
    "homepage": "https://nats.io",
    "keywords": [
        "nats",
        "messaging",
        "pubsub",
        "publish",
        "subscribe",
        "queue",
        "distributed",
        "queueing"
    ],
    "license": "MIT",
    "main": "./index.js",
    "maintainers": [
        {
            "name": "aricart"
        },
        {
            "name": "derek"
        }
    ],
    "name": "nats",
    "optionalDependencies": {},
    "private": false,
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/nats-io/node-nats.git"
    },
    "scripts": {
        "cover": "istanbul cover _mocha",
        "coveralls": "npm run cover -- --report lcovonly && cat ./reports/coverage/lcov.info | coveralls",
        "depcheck": "dependency-check . lib/*",
        "depcheck:unused": "dependency-check ./package.json --unused --no-dev lib/*",
        "lint": "jshint --reporter node_modules/jshint-stylish lib test examples",
        "test": "npm run depcheck && npm run depcheck:unused && npm run lint && npm run test:unit",
        "test:unit": "mkdir -p reports/ && NODE_ENV=test multi='spec=- xunit=reports/mocha-xunit.xml' istanbul cover _mocha -- -R mocha-multi --timeout 10000 --slow 750 && istanbul check-coverage"
    },
    "typings": "./index.d.ts",
    "version": "0.7.16",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
