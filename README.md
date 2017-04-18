# npmdoc-elasticdump

#### api documentation for  [elasticdump (v3.1.0)](https://github.com/taskrabbit/elasticsearch-dump#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-elasticdump.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-elasticdump) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-elasticdump.svg)](https://travis-ci.org/npmdoc/node-npmdoc-elasticdump)

#### import and export tools for elasticsearch

[![NPM](https://nodei.co/npm/elasticdump.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/elasticdump)

- [https://npmdoc.github.io/node-npmdoc-elasticdump/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-elasticdump/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-elasticdump/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-elasticdump/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-elasticdump/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-elasticdump/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Evan Tahler"
    },
    "bin": {
        "elasticdump": "./bin/elasticdump",
        "multielasticdump": "./bin/multielasticdump"
    },
    "bugs": {
        "url": "https://github.com/taskrabbit/elasticsearch-dump/issues"
    },
    "dependencies": {
        "JSONStream": "^1.2.0",
        "async": "^2.0.1",
        "aws4": "^1.4.1",
        "awscred": "^1.2.0",
        "ini": "^1.3.4",
        "optimist": "latest",
        "request": "2.x.x"
    },
    "description": "import and export tools for elasticsearch",
    "devDependencies": {
        "mocha": "latest",
        "should": "latest",
        "standard": "^8.6.0"
    },
    "directories": {},
    "dist": {
        "shasum": "4bec1f64f7931b84884306fb5b37a0d269d81e8d",
        "tarball": "https://registry.npmjs.org/elasticdump/-/elasticdump-3.1.0.tgz"
    },
    "engines": {
        "node": ">=4.0.0"
    },
    "gitHead": "2168ea14394a9a4fe751360083378181709c776c",
    "homepage": "https://github.com/taskrabbit/elasticsearch-dump#readme",
    "keywords": [
        "elasticsearch",
        "dump",
        "elasticdump",
        "import",
        "export",
        "transfer",
        "migrate",
        "migartion",
        "elasitic",
        "cluster",
        "elastic-dump",
        "elastic dump"
    ],
    "license": "Apache-2.0",
    "main": "elasticdump.js",
    "maintainers": [
        {
            "name": "evantahler"
        },
        {
            "name": "bleonard"
        },
        {
            "name": "davidjairala"
        }
    ],
    "name": "elasticdump",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/taskrabbit/elasticsearch-dump.git"
    },
    "scripts": {
        "test": "standard && mocha"
    },
    "standard": {
        "globals": [
            "describe",
            "it",
            "describe",
            "before",
            "beforeEach",
            "after",
            "afterEach"
        ]
    },
    "version": "3.1.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
