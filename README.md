# api documentation for  [elasticdump (v3.1.0)](https://github.com/taskrabbit/elasticsearch-dump#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-elasticdump.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-elasticdump) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-elasticdump.svg)](https://travis-ci.org/npmdoc/node-npmdoc-elasticdump)
#### import and export tools for elasticsearch

[![NPM](https://nodei.co/npm/elasticdump.png?downloads=true)](https://www.npmjs.com/package/elasticdump)

[![apidoc](https://npmdoc.github.io/node-npmdoc-elasticdump/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-elasticdump_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-elasticdump/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-elasticdump/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-elasticdump/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Evan Tahler",
        "email": "evantahler@gmail.com"
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
            "name": "evantahler",
            "email": "evantahler@gmail.com"
        },
        {
            "name": "bleonard",
            "email": "brian@bleonard.com"
        },
        {
            "name": "davidjairala",
            "email": "davidjairala@gmail.com"
        }
    ],
    "name": "elasticdump",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module elasticdump](#apidoc.module.elasticdump)
1.  [function <span class="apidocSignatureSpan">elasticdump.</span>super_ ()](#apidoc.element.elasticdump.super_)
1.  object <span class="apidocSignatureSpan">elasticdump.</span>jsonparser

#### [module elasticdump.jsonparser](#apidoc.module.elasticdump.jsonparser)
1.  [function <span class="apidocSignatureSpan">elasticdump.jsonparser.</span>parse (str)](#apidoc.element.elasticdump.jsonparser.parse)



# <a name="apidoc.module.elasticdump"></a>[module elasticdump](#apidoc.module.elasticdump)

#### <a name="apidoc.element.elasticdump.super_"></a>[function <span class="apidocSignatureSpan">elasticdump.</span>super_ ()](#apidoc.element.elasticdump.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.elasticdump.jsonparser"></a>[module elasticdump.jsonparser](#apidoc.module.elasticdump.jsonparser)

#### <a name="apidoc.element.elasticdump.jsonparser.parse"></a>[function <span class="apidocSignatureSpan">elasticdump.jsonparser.</span>parse (str)](#apidoc.element.elasticdump.jsonparser.parse)
- description and source-code
```javascript
parse = function (str) {
  var result
  try {
    result = JSON.parse(str)
  } catch (e) {
    throw new Error('failed to parse json (message: "' + e.message + '") - source: ' + JSON.stringify(str))
  }

  return result
}
```
- example usage
```shell
...
var fs = require('fs')
var ini = require('ini')
var url = require('url')

module.exports = addAuth

function addAuth (urlToAddAuth, authFile) {
var authConf = ini.parse(fs.readFileSync(authFile, 'utf-8'))
if (authConf.user && authConf.password) {
  var authString = authConf.user + ':' + authConf.password
} else {
  throw new Error('Malformed Auth File')
}
var urlObject = url.parse(urlToAddAuth)
if (!urlObject.auth) {
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
