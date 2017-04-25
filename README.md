# npmdoc-spdy

#### basic api documentation for  [spdy (v3.4.4)](https://github.com/indutny/node-spdy)  [![npm package](https://img.shields.io/npm/v/npmdoc-spdy.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-spdy) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-spdy.svg)](https://travis-ci.org/npmdoc/node-npmdoc-spdy)

#### Implementation of the SPDY protocol on node.js.

[![NPM](https://nodei.co/npm/spdy.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/spdy)

- [https://npmdoc.github.io/node-npmdoc-spdy/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-spdy/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-spdy/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-spdy/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-spdy/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-spdy/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Fedor Indutny"
    },
    "bugs": {
        "url": "https://github.com/indutny/node-spdy/issues"
    },
    "contributors": [
        {
            "name": "Chris Storm"
        },
        {
            "name": "François de Metz"
        },
        {
            "name": "Ilya Grigorik"
        },
        {
            "name": "Roberto Peon"
        },
        {
            "name": "Tatsuhiro Tsujikawa"
        },
        {
            "name": "Jesse Cravens"
        }
    ],
    "dependencies": {
        "debug": "^2.2.0",
        "handle-thing": "^1.2.4",
        "http-deceiver": "^1.2.4",
        "select-hose": "^2.0.0",
        "spdy-transport": "^2.0.15"
    },
    "description": "Implementation of the SPDY protocol on node.js.",
    "devDependencies": {
        "jscs": "^1.13.1",
        "jshint": "^2.8.0",
        "mocha": "^2.2.x"
    },
    "directories": {},
    "dist": {
        "shasum": "e0406407ca90ff01b553eb013505442649f5a819",
        "tarball": "https://registry.npmjs.org/spdy/-/spdy-3.4.4.tgz"
    },
    "engines": [
        "node >= 0.7.0"
    ],
    "gitHead": "52dc157eef87d7d2bb7b39ab25fdcfee45f88dd9",
    "homepage": "https://github.com/indutny/node-spdy",
    "keywords": [
        "spdy"
    ],
    "license": "MIT",
    "main": "./lib/spdy",
    "maintainers": [
        {
            "name": "fedor.indutny"
        },
        {
            "name": "indutny"
        },
        {
            "name": "rauchg"
        }
    ],
    "name": "spdy",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/indutny/node-spdy.git"
    },
    "scripts": {
        "test": "jscs lib/**/*.js test/*.js && jshint lib/**/*.js && mocha --reporter=spec test/*-test.js"
    },
    "version": "3.4.4",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
