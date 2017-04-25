# npmdoc-openpgp

#### basic api documentation for  [openpgp (v2.5.4)](http://openpgpjs.org/)  [![npm package](https://img.shields.io/npm/v/npmdoc-openpgp.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-openpgp) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-openpgp.svg)](https://travis-ci.org/npmdoc/node-npmdoc-openpgp)

#### OpenPGP.js is a Javascript implementation of the OpenPGP protocol. This is defined in RFC 4880.

[![NPM](https://nodei.co/npm/openpgp.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/openpgp)

- [https://npmdoc.github.io/node-npmdoc-openpgp/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-openpgp/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-openpgp/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-openpgp/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-openpgp/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-openpgp/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bugs": {
        "url": "https://github.com/openpgpjs/openpgpjs/issues"
    },
    "dependencies": {
        "node-fetch": "^1.3.3",
        "node-localstorage": "~1.3.0"
    },
    "description": "OpenPGP.js is a Javascript implementation of the OpenPGP protocol. This is defined in RFC 4880.",
    "devDependencies": {
        "asmcrypto-lite": "^1.0.0",
        "babel-preset-es2015": "^6.3.13",
        "babelify": "^7.2.0",
        "browserify-derequire": "^0.9.4",
        "chai": "~3.5.0",
        "es6-promise": "^3.1.2",
        "grunt": "~0.4.5",
        "grunt-browserify": "~5.0.0",
        "grunt-contrib-clean": "~1.0.0",
        "grunt-contrib-connect": "~1.0.2",
        "grunt-contrib-copy": "~1.0.0",
        "grunt-contrib-jshint": "~1.0.0",
        "grunt-contrib-uglify": "~1.0.1",
        "grunt-contrib-watch": "^1.0.0",
        "grunt-jsbeautifier": "~0.2.10",
        "grunt-jscs": "^3.0.1",
        "grunt-jsdoc": "~2.1.0",
        "grunt-mocha-istanbul": "^5.0.1",
        "grunt-mocha-test": "~0.12.7",
        "grunt-saucelabs": "8.6.2",
        "grunt-text-replace": "~0.4.0",
        "istanbul": "~0.4.1",
        "mocha": "~2.5.3",
        "rusha": "^0.8.3",
        "sinon": "^1.17.3",
        "whatwg-fetch": "~1.0.0",
        "zlibjs": "~0.2.0"
    },
    "directories": {
        "lib": "src"
    },
    "dist": {
        "shasum": "688799fb9c98317c07ab39a633853819f4364775",
        "tarball": "https://registry.npmjs.org/openpgp/-/openpgp-2.5.4.tgz"
    },
    "engines": {
        "node": ">=0.8"
    },
    "files": [
        "src/",
        "dist/openpgp.js",
        "dist/openpgp.worker.js",
        "dist/openpgp.min.js",
        "dist/openpgp.worker.min.js",
        "test/unittests.js",
        "test/general",
        "test/crypto"
    ],
    "gitHead": "e00cdd138e1294d47793c7d1763d0f6eb52e876e",
    "homepage": "http://openpgpjs.org/",
    "keywords": [
        "crypto",
        "pgp",
        "gpg",
        "openpgp"
    ],
    "license": "LGPL-3.0+",
    "main": "dist/openpgp.js",
    "maintainers": [
        {
            "name": "bartbutler"
        },
        {
            "name": "tanx"
        },
        {
            "name": "toberndo"
        }
    ],
    "name": "openpgp",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/openpgpjs/openpgpjs.git"
    },
    "scripts": {
        "pretest": "grunt",
        "test": "grunt test"
    },
    "version": "2.5.4",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
