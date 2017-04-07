# api documentation for  [openpgp (v2.5.4)](http://openpgpjs.org/)  [![npm package](https://img.shields.io/npm/v/npmdoc-openpgp.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-openpgp) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-openpgp.svg)](https://travis-ci.org/npmdoc/node-npmdoc-openpgp)
#### OpenPGP.js is a Javascript implementation of the OpenPGP protocol. This is defined in RFC 4880.

[![NPM](https://nodei.co/npm/openpgp.png?downloads=true)](https://www.npmjs.com/package/openpgp)

[![apidoc](https://npmdoc.github.io/node-npmdoc-openpgp/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-openpgp_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-openpgp/build/apidoc.html)

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
            "name": "bartbutler",
            "email": "bartbutler@protonmail.com"
        },
        {
            "name": "tanx",
            "email": "info@tankredhase.de"
        },
        {
            "name": "toberndo",
            "email": "toberndo@yarkon.de"
        }
    ],
    "name": "openpgp",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/openpgpjs/openpgpjs.git"
    },
    "scripts": {
        "pretest": "grunt",
        "test": "grunt test"
    },
    "version": "2.5.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module openpgp](#apidoc.module.openpgp)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>AsyncProxy ()](#apidoc.element.openpgp.AsyncProxy)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>HKP (keyServerBaseUrl)](#apidoc.element.openpgp.HKP)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>Keyid ()](#apidoc.element.openpgp.Keyid)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>Keyring (storeHandler)](#apidoc.element.openpgp.Keyring)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>Keyring.localstore (prefix)](#apidoc.element.openpgp.Keyring.localstore)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>MPI ()](#apidoc.element.openpgp.MPI)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>S2K ()](#apidoc.element.openpgp.S2K)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>cleartext.CleartextMessage (text, signature)](#apidoc.element.openpgp.cleartext.CleartextMessage)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>decrypt (_ref6)](#apidoc.element.openpgp.decrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>decryptKey (_ref4)](#apidoc.element.openpgp.decryptKey)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>decryptSessionKey (_ref10)](#apidoc.element.openpgp.decryptSessionKey)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>destroyWorker ()](#apidoc.element.openpgp.destroyWorker)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>encrypt (_ref5)](#apidoc.element.openpgp.encrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>encryptSessionKey (_ref9)](#apidoc.element.openpgp.encryptSessionKey)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>generateKey ()](#apidoc.element.openpgp.generateKey)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>getWorker ()](#apidoc.element.openpgp.getWorker)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>initWorker ()](#apidoc.element.openpgp.initWorker)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>key.Key (packetlist)](#apidoc.element.openpgp.key.Key)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>message.Message (packetlist)](#apidoc.element.openpgp.message.Message)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>packet.Compressed ()](#apidoc.element.openpgp.packet.Compressed)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>packet.List ()](#apidoc.element.openpgp.packet.List)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>packet.Literal ()](#apidoc.element.openpgp.packet.Literal)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>packet.Marker ()](#apidoc.element.openpgp.packet.Marker)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>packet.OnePassSignature ()](#apidoc.element.openpgp.packet.OnePassSignature)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>packet.PublicKey ()](#apidoc.element.openpgp.packet.PublicKey)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>packet.PublicKeyEncryptedSessionKey ()](#apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>packet.PublicSubkey ()](#apidoc.element.openpgp.packet.PublicSubkey)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>packet.SecretKey ()](#apidoc.element.openpgp.packet.SecretKey)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>packet.SecretSubkey ()](#apidoc.element.openpgp.packet.SecretSubkey)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>packet.Signature ()](#apidoc.element.openpgp.packet.Signature)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>packet.SymEncryptedAEADProtected ()](#apidoc.element.openpgp.packet.SymEncryptedAEADProtected)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>packet.SymEncryptedIntegrityProtected ()](#apidoc.element.openpgp.packet.SymEncryptedIntegrityProtected)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>packet.SymEncryptedSessionKey ()](#apidoc.element.openpgp.packet.SymEncryptedSessionKey)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>packet.SymmetricallyEncrypted ()](#apidoc.element.openpgp.packet.SymmetricallyEncrypted)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>packet.Trust ()](#apidoc.element.openpgp.packet.Trust)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>packet.UserAttribute ()](#apidoc.element.openpgp.packet.UserAttribute)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>packet.Userid ()](#apidoc.element.openpgp.packet.Userid)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>reformatKey ()](#apidoc.element.openpgp.reformatKey)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>sign (_ref7)](#apidoc.element.openpgp.sign)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>signature.Signature (packetlist)](#apidoc.element.openpgp.signature.Signature)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>verify (_ref8)](#apidoc.element.openpgp.verify)
1.  object <span class="apidocSignatureSpan">openpgp.</span>AsyncProxy.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>HKP.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>Keyid.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>Keyring.localstore.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>Keyring.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>MPI.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>S2K.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>armor
1.  object <span class="apidocSignatureSpan">openpgp.</span>cleartext
1.  object <span class="apidocSignatureSpan">openpgp.</span>cleartext.CleartextMessage.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>config
1.  object <span class="apidocSignatureSpan">openpgp.</span>crypto
1.  object <span class="apidocSignatureSpan">openpgp.</span>crypto.cfb
1.  object <span class="apidocSignatureSpan">openpgp.</span>crypto.cipher
1.  object <span class="apidocSignatureSpan">openpgp.</span>crypto.gcm
1.  object <span class="apidocSignatureSpan">openpgp.</span>crypto.hash
1.  object <span class="apidocSignatureSpan">openpgp.</span>crypto.publicKey
1.  object <span class="apidocSignatureSpan">openpgp.</span>crypto.random
1.  object <span class="apidocSignatureSpan">openpgp.</span>crypto.signature
1.  object <span class="apidocSignatureSpan">openpgp.</span>default
1.  object <span class="apidocSignatureSpan">openpgp.</span>enums
1.  object <span class="apidocSignatureSpan">openpgp.</span>key
1.  object <span class="apidocSignatureSpan">openpgp.</span>key.Key.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>message
1.  object <span class="apidocSignatureSpan">openpgp.</span>message.Message.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>packet
1.  object <span class="apidocSignatureSpan">openpgp.</span>packet.Compressed.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>packet.List.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>packet.Literal.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>packet.Marker.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>packet.OnePassSignature.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>packet.PublicKey.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>packet.PublicKeyEncryptedSessionKey.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>packet.PublicSubkey.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>packet.SecretKey.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>packet.SecretSubkey.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>packet.Signature.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>packet.SymEncryptedAEADProtected.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>packet.SymEncryptedIntegrityProtected.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>packet.SymEncryptedSessionKey.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>packet.SymmetricallyEncrypted.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>packet.Trust.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>packet.UserAttribute.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>packet.Userid.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>packet.clone
1.  object <span class="apidocSignatureSpan">openpgp.</span>signature
1.  object <span class="apidocSignatureSpan">openpgp.</span>signature.Signature.prototype
1.  object <span class="apidocSignatureSpan">openpgp.</span>util

#### [module openpgp.AsyncProxy](#apidoc.module.openpgp.AsyncProxy)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>AsyncProxy ()](#apidoc.element.openpgp.AsyncProxy.AsyncProxy)

#### [module openpgp.AsyncProxy.prototype](#apidoc.module.openpgp.AsyncProxy.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.AsyncProxy.prototype.</span>delegate (method, options)](#apidoc.element.openpgp.AsyncProxy.prototype.delegate)
1.  [function <span class="apidocSignatureSpan">openpgp.AsyncProxy.prototype.</span>getID ()](#apidoc.element.openpgp.AsyncProxy.prototype.getID)
1.  [function <span class="apidocSignatureSpan">openpgp.AsyncProxy.prototype.</span>getRandomBuffer (size)](#apidoc.element.openpgp.AsyncProxy.prototype.getRandomBuffer)
1.  [function <span class="apidocSignatureSpan">openpgp.AsyncProxy.prototype.</span>onMessage (event)](#apidoc.element.openpgp.AsyncProxy.prototype.onMessage)
1.  [function <span class="apidocSignatureSpan">openpgp.AsyncProxy.prototype.</span>seedRandom (size)](#apidoc.element.openpgp.AsyncProxy.prototype.seedRandom)
1.  [function <span class="apidocSignatureSpan">openpgp.AsyncProxy.prototype.</span>terminate ()](#apidoc.element.openpgp.AsyncProxy.prototype.terminate)

#### [module openpgp.HKP](#apidoc.module.openpgp.HKP)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>HKP (keyServerBaseUrl)](#apidoc.element.openpgp.HKP.HKP)

#### [module openpgp.HKP.prototype](#apidoc.module.openpgp.HKP.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.HKP.prototype.</span>lookup (options)](#apidoc.element.openpgp.HKP.prototype.lookup)
1.  [function <span class="apidocSignatureSpan">openpgp.HKP.prototype.</span>upload (publicKeyArmored)](#apidoc.element.openpgp.HKP.prototype.upload)

#### [module openpgp.Keyid](#apidoc.module.openpgp.Keyid)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>Keyid ()](#apidoc.element.openpgp.Keyid.Keyid)
1.  [function <span class="apidocSignatureSpan">openpgp.Keyid.</span>fromClone (clone)](#apidoc.element.openpgp.Keyid.fromClone)
1.  [function <span class="apidocSignatureSpan">openpgp.Keyid.</span>fromId (hex)](#apidoc.element.openpgp.Keyid.fromId)
1.  [function <span class="apidocSignatureSpan">openpgp.Keyid.</span>mapToHex (keyId)](#apidoc.element.openpgp.Keyid.mapToHex)

#### [module openpgp.Keyid.prototype](#apidoc.module.openpgp.Keyid.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.Keyid.prototype.</span>equals (keyid)](#apidoc.element.openpgp.Keyid.prototype.equals)
1.  [function <span class="apidocSignatureSpan">openpgp.Keyid.prototype.</span>isNull ()](#apidoc.element.openpgp.Keyid.prototype.isNull)
1.  [function <span class="apidocSignatureSpan">openpgp.Keyid.prototype.</span>read (bytes)](#apidoc.element.openpgp.Keyid.prototype.read)
1.  [function <span class="apidocSignatureSpan">openpgp.Keyid.prototype.</span>toHex ()](#apidoc.element.openpgp.Keyid.prototype.toHex)
1.  [function <span class="apidocSignatureSpan">openpgp.Keyid.prototype.</span>write ()](#apidoc.element.openpgp.Keyid.prototype.write)

#### [module openpgp.Keyring](#apidoc.module.openpgp.Keyring)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>Keyring (storeHandler)](#apidoc.element.openpgp.Keyring.Keyring)
1.  [function <span class="apidocSignatureSpan">openpgp.Keyring.</span>localstore (prefix)](#apidoc.element.openpgp.Keyring.localstore)

#### [module openpgp.Keyring.localstore](#apidoc.module.openpgp.Keyring.localstore)
1.  [function <span class="apidocSignatureSpan">openpgp.Keyring.</span>localstore (prefix)](#apidoc.element.openpgp.Keyring.localstore.localstore)

#### [module openpgp.Keyring.localstore.prototype](#apidoc.module.openpgp.Keyring.localstore.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.Keyring.localstore.prototype.</span>loadPrivate ()](#apidoc.element.openpgp.Keyring.localstore.prototype.loadPrivate)
1.  [function <span class="apidocSignatureSpan">openpgp.Keyring.localstore.prototype.</span>loadPublic ()](#apidoc.element.openpgp.Keyring.localstore.prototype.loadPublic)
1.  [function <span class="apidocSignatureSpan">openpgp.Keyring.localstore.prototype.</span>storePrivate (keys)](#apidoc.element.openpgp.Keyring.localstore.prototype.storePrivate)
1.  [function <span class="apidocSignatureSpan">openpgp.Keyring.localstore.prototype.</span>storePublic (keys)](#apidoc.element.openpgp.Keyring.localstore.prototype.storePublic)
1.  string <span class="apidocSignatureSpan">openpgp.Keyring.localstore.prototype.</span>privateKeysItem
1.  string <span class="apidocSignatureSpan">openpgp.Keyring.localstore.prototype.</span>publicKeysItem

#### [module openpgp.Keyring.prototype](#apidoc.module.openpgp.Keyring.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.Keyring.prototype.</span>clear ()](#apidoc.element.openpgp.Keyring.prototype.clear)
1.  [function <span class="apidocSignatureSpan">openpgp.Keyring.prototype.</span>getAllKeys ()](#apidoc.element.openpgp.Keyring.prototype.getAllKeys)
1.  [function <span class="apidocSignatureSpan">openpgp.Keyring.prototype.</span>getKeysForId (keyId, deep)](#apidoc.element.openpgp.Keyring.prototype.getKeysForId)
1.  [function <span class="apidocSignatureSpan">openpgp.Keyring.prototype.</span>removeKeysForId (keyId)](#apidoc.element.openpgp.Keyring.prototype.removeKeysForId)
1.  [function <span class="apidocSignatureSpan">openpgp.Keyring.prototype.</span>store ()](#apidoc.element.openpgp.Keyring.prototype.store)

#### [module openpgp.MPI](#apidoc.module.openpgp.MPI)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>MPI ()](#apidoc.element.openpgp.MPI.MPI)
1.  [function <span class="apidocSignatureSpan">openpgp.MPI.</span>fromClone (clone)](#apidoc.element.openpgp.MPI.fromClone)

#### [module openpgp.MPI.prototype](#apidoc.module.openpgp.MPI.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.MPI.prototype.</span>byteLength ()](#apidoc.element.openpgp.MPI.prototype.byteLength)
1.  [function <span class="apidocSignatureSpan">openpgp.MPI.prototype.</span>fromBigInteger (bn)](#apidoc.element.openpgp.MPI.prototype.fromBigInteger)
1.  [function <span class="apidocSignatureSpan">openpgp.MPI.prototype.</span>fromBytes (bytes)](#apidoc.element.openpgp.MPI.prototype.fromBytes)
1.  [function <span class="apidocSignatureSpan">openpgp.MPI.prototype.</span>read (bytes)](#apidoc.element.openpgp.MPI.prototype.read)
1.  [function <span class="apidocSignatureSpan">openpgp.MPI.prototype.</span>toBigInteger ()](#apidoc.element.openpgp.MPI.prototype.toBigInteger)
1.  [function <span class="apidocSignatureSpan">openpgp.MPI.prototype.</span>toBytes ()](#apidoc.element.openpgp.MPI.prototype.toBytes)
1.  [function <span class="apidocSignatureSpan">openpgp.MPI.prototype.</span>write ()](#apidoc.element.openpgp.MPI.prototype.write)

#### [module openpgp.S2K](#apidoc.module.openpgp.S2K)
1.  [function <span class="apidocSignatureSpan">openpgp.</span>S2K ()](#apidoc.element.openpgp.S2K.S2K)
1.  [function <span class="apidocSignatureSpan">openpgp.S2K.</span>fromClone (clone)](#apidoc.element.openpgp.S2K.fromClone)

#### [module openpgp.S2K.prototype](#apidoc.module.openpgp.S2K.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.S2K.prototype.</span>get_count ()](#apidoc.element.openpgp.S2K.prototype.get_count)
1.  [function <span class="apidocSignatureSpan">openpgp.S2K.prototype.</span>produce_key (passphrase, numBytes)](#apidoc.element.openpgp.S2K.prototype.produce_key)
1.  [function <span class="apidocSignatureSpan">openpgp.S2K.prototype.</span>read (bytes)](#apidoc.element.openpgp.S2K.prototype.read)
1.  [function <span class="apidocSignatureSpan">openpgp.S2K.prototype.</span>write ()](#apidoc.element.openpgp.S2K.prototype.write)

#### [module openpgp.armor](#apidoc.module.openpgp.armor)
1.  [function <span class="apidocSignatureSpan">openpgp.armor.</span>decode (text)](#apidoc.element.openpgp.armor.decode)
1.  [function <span class="apidocSignatureSpan">openpgp.armor.</span>encode (messagetype, body, partindex, parttotal)](#apidoc.element.openpgp.armor.encode)

#### [module openpgp.cleartext](#apidoc.module.openpgp.cleartext)
1.  [function <span class="apidocSignatureSpan">openpgp.cleartext.</span>CleartextMessage (text, signature)](#apidoc.element.openpgp.cleartext.CleartextMessage)
1.  [function <span class="apidocSignatureSpan">openpgp.cleartext.</span>readArmored (armoredText)](#apidoc.element.openpgp.cleartext.readArmored)

#### [module openpgp.cleartext.CleartextMessage](#apidoc.module.openpgp.cleartext.CleartextMessage)
1.  [function <span class="apidocSignatureSpan">openpgp.cleartext.</span>CleartextMessage (text, signature)](#apidoc.element.openpgp.cleartext.CleartextMessage.CleartextMessage)

#### [module openpgp.cleartext.CleartextMessage.prototype](#apidoc.module.openpgp.cleartext.CleartextMessage.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.cleartext.CleartextMessage.prototype.</span>armor ()](#apidoc.element.openpgp.cleartext.CleartextMessage.prototype.armor)
1.  [function <span class="apidocSignatureSpan">openpgp.cleartext.CleartextMessage.prototype.</span>getSigningKeyIds ()](#apidoc.element.openpgp.cleartext.CleartextMessage.prototype.getSigningKeyIds)
1.  [function <span class="apidocSignatureSpan">openpgp.cleartext.CleartextMessage.prototype.</span>getText ()](#apidoc.element.openpgp.cleartext.CleartextMessage.prototype.getText)
1.  [function <span class="apidocSignatureSpan">openpgp.cleartext.CleartextMessage.prototype.</span>sign (privateKeys)](#apidoc.element.openpgp.cleartext.CleartextMessage.prototype.sign)
1.  [function <span class="apidocSignatureSpan">openpgp.cleartext.CleartextMessage.prototype.</span>signDetached (privateKeys)](#apidoc.element.openpgp.cleartext.CleartextMessage.prototype.signDetached)
1.  [function <span class="apidocSignatureSpan">openpgp.cleartext.CleartextMessage.prototype.</span>verify (keys)](#apidoc.element.openpgp.cleartext.CleartextMessage.prototype.verify)
1.  [function <span class="apidocSignatureSpan">openpgp.cleartext.CleartextMessage.prototype.</span>verifyDetached (signature, keys)](#apidoc.element.openpgp.cleartext.CleartextMessage.prototype.verifyDetached)

#### [module openpgp.crypto](#apidoc.module.openpgp.crypto)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.</span>generateMpi (algo, bits)](#apidoc.element.openpgp.crypto.generateMpi)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.</span>generateSessionKey (algo)](#apidoc.element.openpgp.crypto.generateSessionKey)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.</span>getPrefixRandom (algo)](#apidoc.element.openpgp.crypto.getPrefixRandom)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.</span>getPrivateMpiCount (algo)](#apidoc.element.openpgp.crypto.getPrivateMpiCount)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.</span>getPublicMpiCount (algo)](#apidoc.element.openpgp.crypto.getPublicMpiCount)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.</span>publicKeyDecrypt (algo, keyIntegers, dataIntegers)](#apidoc.element.openpgp.crypto.publicKeyDecrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.</span>publicKeyEncrypt (algo, publicMPIs, data)](#apidoc.element.openpgp.crypto.publicKeyEncrypt)
1.  object <span class="apidocSignatureSpan">openpgp.crypto.</span>cfb
1.  object <span class="apidocSignatureSpan">openpgp.crypto.</span>cipher
1.  object <span class="apidocSignatureSpan">openpgp.crypto.</span>gcm
1.  object <span class="apidocSignatureSpan">openpgp.crypto.</span>hash
1.  object <span class="apidocSignatureSpan">openpgp.crypto.</span>pkcs1
1.  object <span class="apidocSignatureSpan">openpgp.crypto.</span>publicKey
1.  object <span class="apidocSignatureSpan">openpgp.crypto.</span>random
1.  object <span class="apidocSignatureSpan">openpgp.crypto.</span>signature

#### [module openpgp.crypto.cfb](#apidoc.module.openpgp.crypto.cfb)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.cfb.</span>decrypt (cipherfn, key, ciphertext, resync)](#apidoc.element.openpgp.crypto.cfb.decrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.cfb.</span>encrypt (prefixrandom, cipherfn, plaintext, key, resync)](#apidoc.element.openpgp.crypto.cfb.encrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.cfb.</span>mdc (cipherfn, key, ciphertext)](#apidoc.element.openpgp.crypto.cfb.mdc)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.cfb.</span>normalDecrypt (cipherfn, key, ciphertext, iv)](#apidoc.element.openpgp.crypto.cfb.normalDecrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.cfb.</span>normalEncrypt (cipherfn, key, plaintext, iv)](#apidoc.element.openpgp.crypto.cfb.normalEncrypt)

#### [module openpgp.crypto.cipher](#apidoc.module.openpgp.crypto.cipher)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.cipher.</span>aes128 (key)](#apidoc.element.openpgp.crypto.cipher.aes128)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.cipher.</span>aes192 (key)](#apidoc.element.openpgp.crypto.cipher.aes192)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.cipher.</span>aes256 (key)](#apidoc.element.openpgp.crypto.cipher.aes256)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.cipher.</span>blowfish (key)](#apidoc.element.openpgp.crypto.cipher.blowfish)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.cipher.</span>cast5 (key)](#apidoc.element.openpgp.crypto.cipher.cast5)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.cipher.</span>des (key)](#apidoc.element.openpgp.crypto.cipher.des)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.cipher.</span>idea ()](#apidoc.element.openpgp.crypto.cipher.idea)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.cipher.</span>tripledes (key)](#apidoc.element.openpgp.crypto.cipher.tripledes)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.cipher.</span>twofish (key)](#apidoc.element.openpgp.crypto.cipher.twofish)

#### [module openpgp.crypto.gcm](#apidoc.module.openpgp.crypto.gcm)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.gcm.</span>decrypt (cipher, ciphertext, key, iv)](#apidoc.element.openpgp.crypto.gcm.decrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.gcm.</span>encrypt (cipher, plaintext, key, iv)](#apidoc.element.openpgp.crypto.gcm.encrypt)
1.  number <span class="apidocSignatureSpan">openpgp.crypto.gcm.</span>ivLength

#### [module openpgp.crypto.hash](#apidoc.module.openpgp.crypto.hash)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.hash.</span>digest (algo, data)](#apidoc.element.openpgp.crypto.hash.digest)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.hash.</span>getHashByteLength (algo)](#apidoc.element.openpgp.crypto.hash.getHashByteLength)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.hash.</span>md5 (data)](#apidoc.element.openpgp.crypto.hash.md5)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.hash.</span>ripemd (data)](#apidoc.element.openpgp.crypto.hash.ripemd)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.hash.</span>sha1 (data)](#apidoc.element.openpgp.crypto.hash.sha1)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.hash.</span>sha224 (data)](#apidoc.element.openpgp.crypto.hash.sha224)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.hash.</span>sha256 (data)](#apidoc.element.openpgp.crypto.hash.sha256)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.hash.</span>sha384 (data)](#apidoc.element.openpgp.crypto.hash.sha384)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.hash.</span>sha512 (data)](#apidoc.element.openpgp.crypto.hash.sha512)

#### [module openpgp.crypto.publicKey](#apidoc.module.openpgp.crypto.publicKey)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.publicKey.</span>dsa ()](#apidoc.element.openpgp.crypto.publicKey.dsa)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.publicKey.</span>elgamal ()](#apidoc.element.openpgp.crypto.publicKey.elgamal)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.publicKey.</span>rsa ()](#apidoc.element.openpgp.crypto.publicKey.rsa)

#### [module openpgp.crypto.random](#apidoc.module.openpgp.crypto.random)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.random.</span>getRandomBigInteger (bits)](#apidoc.element.openpgp.crypto.random.getRandomBigInteger)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.random.</span>getRandomBigIntegerInRange (min, max)](#apidoc.element.openpgp.crypto.random.getRandomBigIntegerInRange)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.random.</span>getRandomBytes (length)](#apidoc.element.openpgp.crypto.random.getRandomBytes)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.random.</span>getRandomValues (buf)](#apidoc.element.openpgp.crypto.random.getRandomValues)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.random.</span>getSecureRandom (from, to)](#apidoc.element.openpgp.crypto.random.getSecureRandom)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.random.</span>getSecureRandomOctet ()](#apidoc.element.openpgp.crypto.random.getSecureRandomOctet)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.random.</span>getSecureRandomUint ()](#apidoc.element.openpgp.crypto.random.getSecureRandomUint)
1.  object <span class="apidocSignatureSpan">openpgp.crypto.random.</span>randomBuffer

#### [module openpgp.crypto.signature](#apidoc.module.openpgp.crypto.signature)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.signature.</span>sign (hash_algo, algo, keyIntegers, data)](#apidoc.element.openpgp.crypto.signature.sign)
1.  [function <span class="apidocSignatureSpan">openpgp.crypto.signature.</span>verify (algo, hash_algo, msg_MPIs, publickey_MPIs, data)](#apidoc.element.openpgp.crypto.signature.verify)

#### [module openpgp.default](#apidoc.module.openpgp.default)
1.  [function <span class="apidocSignatureSpan">openpgp.default.</span>decrypt (_ref6)](#apidoc.element.openpgp.default.decrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.default.</span>decryptKey (_ref4)](#apidoc.element.openpgp.default.decryptKey)
1.  [function <span class="apidocSignatureSpan">openpgp.default.</span>decryptSessionKey (_ref10)](#apidoc.element.openpgp.default.decryptSessionKey)
1.  [function <span class="apidocSignatureSpan">openpgp.default.</span>destroyWorker ()](#apidoc.element.openpgp.default.destroyWorker)
1.  [function <span class="apidocSignatureSpan">openpgp.default.</span>encrypt (_ref5)](#apidoc.element.openpgp.default.encrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.default.</span>encryptSessionKey (_ref9)](#apidoc.element.openpgp.default.encryptSessionKey)
1.  [function <span class="apidocSignatureSpan">openpgp.default.</span>generateKey ()](#apidoc.element.openpgp.default.generateKey)
1.  [function <span class="apidocSignatureSpan">openpgp.default.</span>getWorker ()](#apidoc.element.openpgp.default.getWorker)
1.  [function <span class="apidocSignatureSpan">openpgp.default.</span>initWorker ()](#apidoc.element.openpgp.default.initWorker)
1.  [function <span class="apidocSignatureSpan">openpgp.default.</span>reformatKey ()](#apidoc.element.openpgp.default.reformatKey)
1.  [function <span class="apidocSignatureSpan">openpgp.default.</span>sign (_ref7)](#apidoc.element.openpgp.default.sign)
1.  [function <span class="apidocSignatureSpan">openpgp.default.</span>verify (_ref8)](#apidoc.element.openpgp.default.verify)

#### [module openpgp.enums](#apidoc.module.openpgp.enums)
1.  [function <span class="apidocSignatureSpan">openpgp.enums.</span>read (type, e)](#apidoc.element.openpgp.enums.read)
1.  [function <span class="apidocSignatureSpan">openpgp.enums.</span>write (type, e)](#apidoc.element.openpgp.enums.write)
1.  object <span class="apidocSignatureSpan">openpgp.enums.</span>armor
1.  object <span class="apidocSignatureSpan">openpgp.enums.</span>compression
1.  object <span class="apidocSignatureSpan">openpgp.enums.</span>hash
1.  object <span class="apidocSignatureSpan">openpgp.enums.</span>keyFlags
1.  object <span class="apidocSignatureSpan">openpgp.enums.</span>keyStatus
1.  object <span class="apidocSignatureSpan">openpgp.enums.</span>literal
1.  object <span class="apidocSignatureSpan">openpgp.enums.</span>packet
1.  object <span class="apidocSignatureSpan">openpgp.enums.</span>publicKey
1.  object <span class="apidocSignatureSpan">openpgp.enums.</span>s2k
1.  object <span class="apidocSignatureSpan">openpgp.enums.</span>signature
1.  object <span class="apidocSignatureSpan">openpgp.enums.</span>signatureSubpacket
1.  object <span class="apidocSignatureSpan">openpgp.enums.</span>symmetric

#### [module openpgp.key](#apidoc.module.openpgp.key)
1.  [function <span class="apidocSignatureSpan">openpgp.key.</span>Key (packetlist)](#apidoc.element.openpgp.key.Key)
1.  [function <span class="apidocSignatureSpan">openpgp.key.</span>generate (options)](#apidoc.element.openpgp.key.generate)
1.  [function <span class="apidocSignatureSpan">openpgp.key.</span>getPreferredSymAlgo (keys)](#apidoc.element.openpgp.key.getPreferredSymAlgo)
1.  [function <span class="apidocSignatureSpan">openpgp.key.</span>readArmored (armoredText)](#apidoc.element.openpgp.key.readArmored)
1.  [function <span class="apidocSignatureSpan">openpgp.key.</span>reformat (options)](#apidoc.element.openpgp.key.reformat)

#### [module openpgp.key.Key](#apidoc.module.openpgp.key.Key)
1.  [function <span class="apidocSignatureSpan">openpgp.key.</span>Key (packetlist)](#apidoc.element.openpgp.key.Key.Key)

#### [module openpgp.key.Key.prototype](#apidoc.module.openpgp.key.Key.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>armor ()](#apidoc.element.openpgp.key.Key.prototype.armor)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>decrypt (passphrase)](#apidoc.element.openpgp.key.Key.prototype.decrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>decryptKeyPacket (keyIds, passphrase)](#apidoc.element.openpgp.key.Key.prototype.decryptKeyPacket)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>encrypt (passphrase)](#apidoc.element.openpgp.key.Key.prototype.encrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>getAllKeyPackets ()](#apidoc.element.openpgp.key.Key.prototype.getAllKeyPackets)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>getEncryptionKeyPacket ()](#apidoc.element.openpgp.key.Key.prototype.getEncryptionKeyPacket)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>getExpirationTime ()](#apidoc.element.openpgp.key.Key.prototype.getExpirationTime)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>getKeyIds ()](#apidoc.element.openpgp.key.Key.prototype.getKeyIds)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>getKeyPacket (keyIds)](#apidoc.element.openpgp.key.Key.prototype.getKeyPacket)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>getPreferredHashAlgorithm ()](#apidoc.element.openpgp.key.Key.prototype.getPreferredHashAlgorithm)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>getPrimaryUser ()](#apidoc.element.openpgp.key.Key.prototype.getPrimaryUser)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>getSigningKeyPacket (keyId)](#apidoc.element.openpgp.key.Key.prototype.getSigningKeyPacket)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>getSubkeyPackets ()](#apidoc.element.openpgp.key.Key.prototype.getSubkeyPackets)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>getUserIds ()](#apidoc.element.openpgp.key.Key.prototype.getUserIds)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>isPrivate ()](#apidoc.element.openpgp.key.Key.prototype.isPrivate)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>isPublic ()](#apidoc.element.openpgp.key.Key.prototype.isPublic)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>packetlist2structure (packetlist)](#apidoc.element.openpgp.key.Key.prototype.packetlist2structure)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>revoke ()](#apidoc.element.openpgp.key.Key.prototype.revoke)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>signAllUsers (privateKeys)](#apidoc.element.openpgp.key.Key.prototype.signAllUsers)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>signPrimaryUser (privateKeys)](#apidoc.element.openpgp.key.Key.prototype.signPrimaryUser)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>toPacketlist ()](#apidoc.element.openpgp.key.Key.prototype.toPacketlist)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>toPublic ()](#apidoc.element.openpgp.key.Key.prototype.toPublic)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>update (key)](#apidoc.element.openpgp.key.Key.prototype.update)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>verifyAllUsers (keys)](#apidoc.element.openpgp.key.Key.prototype.verifyAllUsers)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>verifyPrimaryKey ()](#apidoc.element.openpgp.key.Key.prototype.verifyPrimaryKey)
1.  [function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>verifyPrimaryUser (keys)](#apidoc.element.openpgp.key.Key.prototype.verifyPrimaryUser)

#### [module openpgp.message](#apidoc.module.openpgp.message)
1.  [function <span class="apidocSignatureSpan">openpgp.message.</span>Message (packetlist)](#apidoc.element.openpgp.message.Message)
1.  [function <span class="apidocSignatureSpan">openpgp.message.</span>encryptSessionKey (sessionKey, symAlgo, publicKeys, passwords)](#apidoc.element.openpgp.message.encryptSessionKey)
1.  [function <span class="apidocSignatureSpan">openpgp.message.</span>fromBinary (bytes, filename)](#apidoc.element.openpgp.message.fromBinary)
1.  [function <span class="apidocSignatureSpan">openpgp.message.</span>fromText (text, filename)](#apidoc.element.openpgp.message.fromText)
1.  [function <span class="apidocSignatureSpan">openpgp.message.</span>read (input)](#apidoc.element.openpgp.message.read)
1.  [function <span class="apidocSignatureSpan">openpgp.message.</span>readArmored (armoredText)](#apidoc.element.openpgp.message.readArmored)
1.  [function <span class="apidocSignatureSpan">openpgp.message.</span>readSignedContent (content, detachedSignature)](#apidoc.element.openpgp.message.readSignedContent)

#### [module openpgp.message.Message](#apidoc.module.openpgp.message.Message)
1.  [function <span class="apidocSignatureSpan">openpgp.message.</span>Message (packetlist)](#apidoc.element.openpgp.message.Message.Message)

#### [module openpgp.message.Message.prototype](#apidoc.module.openpgp.message.Message.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>armor ()](#apidoc.element.openpgp.message.Message.prototype.armor)
1.  [function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>decrypt (privateKey, sessionKey, password)](#apidoc.element.openpgp.message.Message.prototype.decrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>decryptSessionKey (privateKey, password)](#apidoc.element.openpgp.message.Message.prototype.decryptSessionKey)
1.  [function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>encrypt (keys, passwords)](#apidoc.element.openpgp.message.Message.prototype.encrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>getEncryptionKeyIds ()](#apidoc.element.openpgp.message.Message.prototype.getEncryptionKeyIds)
1.  [function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>getFilename ()](#apidoc.element.openpgp.message.Message.prototype.getFilename)
1.  [function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>getLiteralData ()](#apidoc.element.openpgp.message.Message.prototype.getLiteralData)
1.  [function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>getSigningKeyIds ()](#apidoc.element.openpgp.message.Message.prototype.getSigningKeyIds)
1.  [function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>getText ()](#apidoc.element.openpgp.message.Message.prototype.getText)
1.  [function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>sign ()](#apidoc.element.openpgp.message.Message.prototype.sign)
1.  [function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>signDetached ()](#apidoc.element.openpgp.message.Message.prototype.signDetached)
1.  [function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>unwrapCompressed ()](#apidoc.element.openpgp.message.Message.prototype.unwrapCompressed)
1.  [function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>verify (keys)](#apidoc.element.openpgp.message.Message.prototype.verify)
1.  [function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>verifyDetached (signature, keys)](#apidoc.element.openpgp.message.Message.prototype.verifyDetached)

#### [module openpgp.packet](#apidoc.module.openpgp.packet)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>Compressed ()](#apidoc.element.openpgp.packet.Compressed)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>List ()](#apidoc.element.openpgp.packet.List)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>Literal ()](#apidoc.element.openpgp.packet.Literal)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>Marker ()](#apidoc.element.openpgp.packet.Marker)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>OnePassSignature ()](#apidoc.element.openpgp.packet.OnePassSignature)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>PublicKey ()](#apidoc.element.openpgp.packet.PublicKey)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>PublicKeyEncryptedSessionKey ()](#apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>PublicSubkey ()](#apidoc.element.openpgp.packet.PublicSubkey)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>SecretKey ()](#apidoc.element.openpgp.packet.SecretKey)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>SecretSubkey ()](#apidoc.element.openpgp.packet.SecretSubkey)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>Signature ()](#apidoc.element.openpgp.packet.Signature)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>SymEncryptedAEADProtected ()](#apidoc.element.openpgp.packet.SymEncryptedAEADProtected)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>SymEncryptedIntegrityProtected ()](#apidoc.element.openpgp.packet.SymEncryptedIntegrityProtected)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>SymEncryptedSessionKey ()](#apidoc.element.openpgp.packet.SymEncryptedSessionKey)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>SymmetricallyEncrypted ()](#apidoc.element.openpgp.packet.SymmetricallyEncrypted)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>Trust ()](#apidoc.element.openpgp.packet.Trust)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>UserAttribute ()](#apidoc.element.openpgp.packet.UserAttribute)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>Userid ()](#apidoc.element.openpgp.packet.Userid)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>fromStructuredClone (packetClone)](#apidoc.element.openpgp.packet.fromStructuredClone)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>newPacketFromTag (tag)](#apidoc.element.openpgp.packet.newPacketFromTag)
1.  object <span class="apidocSignatureSpan">openpgp.packet.</span>clone

#### [module openpgp.packet.Compressed](#apidoc.module.openpgp.packet.Compressed)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>Compressed ()](#apidoc.element.openpgp.packet.Compressed.Compressed)

#### [module openpgp.packet.Compressed.prototype](#apidoc.module.openpgp.packet.Compressed.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Compressed.prototype.</span>compress ()](#apidoc.element.openpgp.packet.Compressed.prototype.compress)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Compressed.prototype.</span>decompress ()](#apidoc.element.openpgp.packet.Compressed.prototype.decompress)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Compressed.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.Compressed.prototype.read)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Compressed.prototype.</span>write ()](#apidoc.element.openpgp.packet.Compressed.prototype.write)

#### [module openpgp.packet.List](#apidoc.module.openpgp.packet.List)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>List ()](#apidoc.element.openpgp.packet.List.List)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.List.</span>fromStructuredClone (packetlistClone)](#apidoc.element.openpgp.packet.List.fromStructuredClone)

#### [module openpgp.packet.List.prototype](#apidoc.module.openpgp.packet.List.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.List.prototype.</span>concat (packetlist)](#apidoc.element.openpgp.packet.List.prototype.concat)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.List.prototype.</span>filter (callback)](#apidoc.element.openpgp.packet.List.prototype.filter)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.List.prototype.</span>filterByTag ()](#apidoc.element.openpgp.packet.List.prototype.filterByTag)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.List.prototype.</span>findPacket (type)](#apidoc.element.openpgp.packet.List.prototype.findPacket)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.List.prototype.</span>forEach (callback)](#apidoc.element.openpgp.packet.List.prototype.forEach)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.List.prototype.</span>indexOfTag ()](#apidoc.element.openpgp.packet.List.prototype.indexOfTag)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.List.prototype.</span>pop ()](#apidoc.element.openpgp.packet.List.prototype.pop)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.List.prototype.</span>push (packet)](#apidoc.element.openpgp.packet.List.prototype.push)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.List.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.List.prototype.read)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.List.prototype.</span>slice (begin, end)](#apidoc.element.openpgp.packet.List.prototype.slice)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.List.prototype.</span>write ()](#apidoc.element.openpgp.packet.List.prototype.write)

#### [module openpgp.packet.Literal](#apidoc.module.openpgp.packet.Literal)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>Literal ()](#apidoc.element.openpgp.packet.Literal.Literal)

#### [module openpgp.packet.Literal.prototype](#apidoc.module.openpgp.packet.Literal.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Literal.prototype.</span>getBytes ()](#apidoc.element.openpgp.packet.Literal.prototype.getBytes)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Literal.prototype.</span>getFilename ()](#apidoc.element.openpgp.packet.Literal.prototype.getFilename)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Literal.prototype.</span>getText ()](#apidoc.element.openpgp.packet.Literal.prototype.getText)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Literal.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.Literal.prototype.read)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Literal.prototype.</span>setBytes (bytes, format)](#apidoc.element.openpgp.packet.Literal.prototype.setBytes)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Literal.prototype.</span>setFilename (filename)](#apidoc.element.openpgp.packet.Literal.prototype.setFilename)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Literal.prototype.</span>setText (text)](#apidoc.element.openpgp.packet.Literal.prototype.setText)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Literal.prototype.</span>write ()](#apidoc.element.openpgp.packet.Literal.prototype.write)

#### [module openpgp.packet.Marker](#apidoc.module.openpgp.packet.Marker)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>Marker ()](#apidoc.element.openpgp.packet.Marker.Marker)

#### [module openpgp.packet.Marker.prototype](#apidoc.module.openpgp.packet.Marker.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Marker.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.Marker.prototype.read)

#### [module openpgp.packet.OnePassSignature](#apidoc.module.openpgp.packet.OnePassSignature)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>OnePassSignature ()](#apidoc.element.openpgp.packet.OnePassSignature.OnePassSignature)

#### [module openpgp.packet.OnePassSignature.prototype](#apidoc.module.openpgp.packet.OnePassSignature.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.OnePassSignature.prototype.</span>postCloneTypeFix ()](#apidoc.element.openpgp.packet.OnePassSignature.prototype.postCloneTypeFix)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.OnePassSignature.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.OnePassSignature.prototype.read)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.OnePassSignature.prototype.</span>write ()](#apidoc.element.openpgp.packet.OnePassSignature.prototype.write)

#### [module openpgp.packet.PublicKey](#apidoc.module.openpgp.packet.PublicKey)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>PublicKey ()](#apidoc.element.openpgp.packet.PublicKey.PublicKey)

#### [module openpgp.packet.PublicKey.prototype](#apidoc.module.openpgp.packet.PublicKey.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.PublicKey.prototype.</span>getBitSize ()](#apidoc.element.openpgp.packet.PublicKey.prototype.getBitSize)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.PublicKey.prototype.</span>getFingerprint ()](#apidoc.element.openpgp.packet.PublicKey.prototype.getFingerprint)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.PublicKey.prototype.</span>getKeyId ()](#apidoc.element.openpgp.packet.PublicKey.prototype.getKeyId)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.PublicKey.prototype.</span>postCloneTypeFix ()](#apidoc.element.openpgp.packet.PublicKey.prototype.postCloneTypeFix)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.PublicKey.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.PublicKey.prototype.read)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.PublicKey.prototype.</span>readPublicKey (bytes)](#apidoc.element.openpgp.packet.PublicKey.prototype.readPublicKey)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.PublicKey.prototype.</span>write ()](#apidoc.element.openpgp.packet.PublicKey.prototype.write)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.PublicKey.prototype.</span>writeOld ()](#apidoc.element.openpgp.packet.PublicKey.prototype.writeOld)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.PublicKey.prototype.</span>writePublicKey ()](#apidoc.element.openpgp.packet.PublicKey.prototype.writePublicKey)

#### [module openpgp.packet.PublicKeyEncryptedSessionKey](#apidoc.module.openpgp.packet.PublicKeyEncryptedSessionKey)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>PublicKeyEncryptedSessionKey ()](#apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey.PublicKeyEncryptedSessionKey)

#### [module openpgp.packet.PublicKeyEncryptedSessionKey.prototype](#apidoc.module.openpgp.packet.PublicKeyEncryptedSessionKey.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.PublicKeyEncryptedSessionKey.prototype.</span>decrypt (key)](#apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey.prototype.decrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.PublicKeyEncryptedSessionKey.prototype.</span>encrypt (key)](#apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey.prototype.encrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.PublicKeyEncryptedSessionKey.prototype.</span>postCloneTypeFix ()](#apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey.prototype.postCloneTypeFix)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.PublicKeyEncryptedSessionKey.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey.prototype.read)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.PublicKeyEncryptedSessionKey.prototype.</span>write ()](#apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey.prototype.write)

#### [module openpgp.packet.PublicSubkey](#apidoc.module.openpgp.packet.PublicSubkey)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>PublicSubkey ()](#apidoc.element.openpgp.packet.PublicSubkey.PublicSubkey)

#### [module openpgp.packet.PublicSubkey.prototype](#apidoc.module.openpgp.packet.PublicSubkey.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.PublicSubkey.prototype.</span>constructor ()](#apidoc.element.openpgp.packet.PublicSubkey.prototype.constructor)
1.  number <span class="apidocSignatureSpan">openpgp.packet.PublicSubkey.prototype.</span>expirationTimeV3
1.  number <span class="apidocSignatureSpan">openpgp.packet.PublicSubkey.prototype.</span>tag
1.  number <span class="apidocSignatureSpan">openpgp.packet.PublicSubkey.prototype.</span>version
1.  object <span class="apidocSignatureSpan">openpgp.packet.PublicSubkey.prototype.</span>created
1.  object <span class="apidocSignatureSpan">openpgp.packet.PublicSubkey.prototype.</span>fingerprint
1.  object <span class="apidocSignatureSpan">openpgp.packet.PublicSubkey.prototype.</span>keyid
1.  object <span class="apidocSignatureSpan">openpgp.packet.PublicSubkey.prototype.</span>mpi
1.  string <span class="apidocSignatureSpan">openpgp.packet.PublicSubkey.prototype.</span>algorithm

#### [module openpgp.packet.SecretKey](#apidoc.module.openpgp.packet.SecretKey)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>SecretKey ()](#apidoc.element.openpgp.packet.SecretKey.SecretKey)

#### [module openpgp.packet.SecretKey.prototype](#apidoc.module.openpgp.packet.SecretKey.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SecretKey.prototype.</span>clearPrivateMPIs ()](#apidoc.element.openpgp.packet.SecretKey.prototype.clearPrivateMPIs)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SecretKey.prototype.</span>constructor ()](#apidoc.element.openpgp.packet.SecretKey.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SecretKey.prototype.</span>decrypt (passphrase)](#apidoc.element.openpgp.packet.SecretKey.prototype.decrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SecretKey.prototype.</span>encrypt (passphrase)](#apidoc.element.openpgp.packet.SecretKey.prototype.encrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SecretKey.prototype.</span>generate (bits)](#apidoc.element.openpgp.packet.SecretKey.prototype.generate)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SecretKey.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.SecretKey.prototype.read)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SecretKey.prototype.</span>write ()](#apidoc.element.openpgp.packet.SecretKey.prototype.write)
1.  number <span class="apidocSignatureSpan">openpgp.packet.SecretKey.prototype.</span>expirationTimeV3
1.  number <span class="apidocSignatureSpan">openpgp.packet.SecretKey.prototype.</span>tag
1.  number <span class="apidocSignatureSpan">openpgp.packet.SecretKey.prototype.</span>version
1.  object <span class="apidocSignatureSpan">openpgp.packet.SecretKey.prototype.</span>created
1.  object <span class="apidocSignatureSpan">openpgp.packet.SecretKey.prototype.</span>fingerprint
1.  object <span class="apidocSignatureSpan">openpgp.packet.SecretKey.prototype.</span>keyid
1.  object <span class="apidocSignatureSpan">openpgp.packet.SecretKey.prototype.</span>mpi
1.  string <span class="apidocSignatureSpan">openpgp.packet.SecretKey.prototype.</span>algorithm

#### [module openpgp.packet.SecretSubkey](#apidoc.module.openpgp.packet.SecretSubkey)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>SecretSubkey ()](#apidoc.element.openpgp.packet.SecretSubkey.SecretSubkey)

#### [module openpgp.packet.SecretSubkey.prototype](#apidoc.module.openpgp.packet.SecretSubkey.prototype)
1.  boolean <span class="apidocSignatureSpan">openpgp.packet.SecretSubkey.prototype.</span>isDecrypted
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SecretSubkey.prototype.</span>constructor ()](#apidoc.element.openpgp.packet.SecretSubkey.prototype.constructor)
1.  number <span class="apidocSignatureSpan">openpgp.packet.SecretSubkey.prototype.</span>expirationTimeV3
1.  number <span class="apidocSignatureSpan">openpgp.packet.SecretSubkey.prototype.</span>tag
1.  number <span class="apidocSignatureSpan">openpgp.packet.SecretSubkey.prototype.</span>version
1.  object <span class="apidocSignatureSpan">openpgp.packet.SecretSubkey.prototype.</span>created
1.  object <span class="apidocSignatureSpan">openpgp.packet.SecretSubkey.prototype.</span>encrypted
1.  object <span class="apidocSignatureSpan">openpgp.packet.SecretSubkey.prototype.</span>fingerprint
1.  object <span class="apidocSignatureSpan">openpgp.packet.SecretSubkey.prototype.</span>keyid
1.  object <span class="apidocSignatureSpan">openpgp.packet.SecretSubkey.prototype.</span>mpi
1.  string <span class="apidocSignatureSpan">openpgp.packet.SecretSubkey.prototype.</span>algorithm

#### [module openpgp.packet.Signature](#apidoc.module.openpgp.packet.Signature)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>Signature ()](#apidoc.element.openpgp.packet.Signature.Signature)

#### [module openpgp.packet.Signature.prototype](#apidoc.module.openpgp.packet.Signature.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Signature.prototype.</span>calculateTrailer ()](#apidoc.element.openpgp.packet.Signature.prototype.calculateTrailer)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Signature.prototype.</span>isExpired ()](#apidoc.element.openpgp.packet.Signature.prototype.isExpired)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Signature.prototype.</span>postCloneTypeFix ()](#apidoc.element.openpgp.packet.Signature.prototype.postCloneTypeFix)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Signature.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.Signature.prototype.read)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Signature.prototype.</span>read_sub_packet (bytes)](#apidoc.element.openpgp.packet.Signature.prototype.read_sub_packet)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Signature.prototype.</span>sign (key, data)](#apidoc.element.openpgp.packet.Signature.prototype.sign)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Signature.prototype.</span>toSign (type, data)](#apidoc.element.openpgp.packet.Signature.prototype.toSign)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Signature.prototype.</span>verify (key, data)](#apidoc.element.openpgp.packet.Signature.prototype.verify)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Signature.prototype.</span>write ()](#apidoc.element.openpgp.packet.Signature.prototype.write)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Signature.prototype.</span>write_all_sub_packets ()](#apidoc.element.openpgp.packet.Signature.prototype.write_all_sub_packets)

#### [module openpgp.packet.SymEncryptedAEADProtected](#apidoc.module.openpgp.packet.SymEncryptedAEADProtected)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>SymEncryptedAEADProtected ()](#apidoc.element.openpgp.packet.SymEncryptedAEADProtected.SymEncryptedAEADProtected)

#### [module openpgp.packet.SymEncryptedAEADProtected.prototype](#apidoc.module.openpgp.packet.SymEncryptedAEADProtected.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedAEADProtected.prototype.</span>decrypt (sessionKeyAlgorithm, key)](#apidoc.element.openpgp.packet.SymEncryptedAEADProtected.prototype.decrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedAEADProtected.prototype.</span>encrypt (sessionKeyAlgorithm, key)](#apidoc.element.openpgp.packet.SymEncryptedAEADProtected.prototype.encrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedAEADProtected.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.SymEncryptedAEADProtected.prototype.read)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedAEADProtected.prototype.</span>write ()](#apidoc.element.openpgp.packet.SymEncryptedAEADProtected.prototype.write)

#### [module openpgp.packet.SymEncryptedIntegrityProtected](#apidoc.module.openpgp.packet.SymEncryptedIntegrityProtected)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>SymEncryptedIntegrityProtected ()](#apidoc.element.openpgp.packet.SymEncryptedIntegrityProtected.SymEncryptedIntegrityProtected)

#### [module openpgp.packet.SymEncryptedIntegrityProtected.prototype](#apidoc.module.openpgp.packet.SymEncryptedIntegrityProtected.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedIntegrityProtected.prototype.</span>decrypt (sessionKeyAlgorithm, key)](#apidoc.element.openpgp.packet.SymEncryptedIntegrityProtected.prototype.decrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedIntegrityProtected.prototype.</span>encrypt (sessionKeyAlgorithm, key)](#apidoc.element.openpgp.packet.SymEncryptedIntegrityProtected.prototype.encrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedIntegrityProtected.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.SymEncryptedIntegrityProtected.prototype.read)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedIntegrityProtected.prototype.</span>write ()](#apidoc.element.openpgp.packet.SymEncryptedIntegrityProtected.prototype.write)

#### [module openpgp.packet.SymEncryptedSessionKey](#apidoc.module.openpgp.packet.SymEncryptedSessionKey)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>SymEncryptedSessionKey ()](#apidoc.element.openpgp.packet.SymEncryptedSessionKey.SymEncryptedSessionKey)

#### [module openpgp.packet.SymEncryptedSessionKey.prototype](#apidoc.module.openpgp.packet.SymEncryptedSessionKey.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedSessionKey.prototype.</span>decrypt (passphrase)](#apidoc.element.openpgp.packet.SymEncryptedSessionKey.prototype.decrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedSessionKey.prototype.</span>encrypt (passphrase)](#apidoc.element.openpgp.packet.SymEncryptedSessionKey.prototype.encrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedSessionKey.prototype.</span>postCloneTypeFix ()](#apidoc.element.openpgp.packet.SymEncryptedSessionKey.prototype.postCloneTypeFix)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedSessionKey.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.SymEncryptedSessionKey.prototype.read)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedSessionKey.prototype.</span>write ()](#apidoc.element.openpgp.packet.SymEncryptedSessionKey.prototype.write)

#### [module openpgp.packet.SymmetricallyEncrypted](#apidoc.module.openpgp.packet.SymmetricallyEncrypted)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>SymmetricallyEncrypted ()](#apidoc.element.openpgp.packet.SymmetricallyEncrypted.SymmetricallyEncrypted)

#### [module openpgp.packet.SymmetricallyEncrypted.prototype](#apidoc.module.openpgp.packet.SymmetricallyEncrypted.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SymmetricallyEncrypted.prototype.</span>decrypt (sessionKeyAlgorithm, key)](#apidoc.element.openpgp.packet.SymmetricallyEncrypted.prototype.decrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SymmetricallyEncrypted.prototype.</span>encrypt (algo, key)](#apidoc.element.openpgp.packet.SymmetricallyEncrypted.prototype.encrypt)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SymmetricallyEncrypted.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.SymmetricallyEncrypted.prototype.read)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.SymmetricallyEncrypted.prototype.</span>write ()](#apidoc.element.openpgp.packet.SymmetricallyEncrypted.prototype.write)

#### [module openpgp.packet.Trust](#apidoc.module.openpgp.packet.Trust)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>Trust ()](#apidoc.element.openpgp.packet.Trust.Trust)

#### [module openpgp.packet.Trust.prototype](#apidoc.module.openpgp.packet.Trust.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Trust.prototype.</span>read ()](#apidoc.element.openpgp.packet.Trust.prototype.read)

#### [module openpgp.packet.UserAttribute](#apidoc.module.openpgp.packet.UserAttribute)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>UserAttribute ()](#apidoc.element.openpgp.packet.UserAttribute.UserAttribute)

#### [module openpgp.packet.UserAttribute.prototype](#apidoc.module.openpgp.packet.UserAttribute.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.UserAttribute.prototype.</span>equals (usrAttr)](#apidoc.element.openpgp.packet.UserAttribute.prototype.equals)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.UserAttribute.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.UserAttribute.prototype.read)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.UserAttribute.prototype.</span>write ()](#apidoc.element.openpgp.packet.UserAttribute.prototype.write)

#### [module openpgp.packet.Userid](#apidoc.module.openpgp.packet.Userid)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.</span>Userid ()](#apidoc.element.openpgp.packet.Userid.Userid)

#### [module openpgp.packet.Userid.prototype](#apidoc.module.openpgp.packet.Userid.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Userid.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.Userid.prototype.read)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.Userid.prototype.</span>write ()](#apidoc.element.openpgp.packet.Userid.prototype.write)

#### [module openpgp.packet.clone](#apidoc.module.openpgp.packet.clone)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.clone.</span>clonePackets (options)](#apidoc.element.openpgp.packet.clone.clonePackets)
1.  [function <span class="apidocSignatureSpan">openpgp.packet.clone.</span>parseClonedPackets (options, method)](#apidoc.element.openpgp.packet.clone.parseClonedPackets)

#### [module openpgp.signature](#apidoc.module.openpgp.signature)
1.  [function <span class="apidocSignatureSpan">openpgp.signature.</span>Signature (packetlist)](#apidoc.element.openpgp.signature.Signature)
1.  [function <span class="apidocSignatureSpan">openpgp.signature.</span>read (input)](#apidoc.element.openpgp.signature.read)
1.  [function <span class="apidocSignatureSpan">openpgp.signature.</span>readArmored (armoredText)](#apidoc.element.openpgp.signature.readArmored)

#### [module openpgp.signature.Signature](#apidoc.module.openpgp.signature.Signature)
1.  [function <span class="apidocSignatureSpan">openpgp.signature.</span>Signature (packetlist)](#apidoc.element.openpgp.signature.Signature.Signature)

#### [module openpgp.signature.Signature.prototype](#apidoc.module.openpgp.signature.Signature.prototype)
1.  [function <span class="apidocSignatureSpan">openpgp.signature.Signature.prototype.</span>armor ()](#apidoc.element.openpgp.signature.Signature.prototype.armor)

#### [module openpgp.util](#apidoc.module.openpgp.util)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>Uint8Array2str (bin)](#apidoc.element.openpgp.util.Uint8Array2str)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>bin2str (bin)](#apidoc.element.openpgp.util.bin2str)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>calc_checksum (text)](#apidoc.element.openpgp.util.calc_checksum)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>collectBuffers (obj, collection)](#apidoc.element.openpgp.util.collectBuffers)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>concatUint8Array (arrays)](#apidoc.element.openpgp.util.concatUint8Array)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>copyUint8Array (array)](#apidoc.element.openpgp.util.copyUint8Array)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>decode_utf8 (utf8)](#apidoc.element.openpgp.util.decode_utf8)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>detectNode ()](#apidoc.element.openpgp.util.detectNode)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>encode_utf8 (str)](#apidoc.element.openpgp.util.encode_utf8)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>equalsUint8Array (array1, array2)](#apidoc.element.openpgp.util.equalsUint8Array)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>getLeftNBits (string, bitcount)](#apidoc.element.openpgp.util.getLeftNBits)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>getNodeBuffer ()](#apidoc.element.openpgp.util.getNodeBuffer)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>getNodeCrypto ()](#apidoc.element.openpgp.util.getNodeCrypto)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>getTransferables (obj)](#apidoc.element.openpgp.util.getTransferables)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>getWebCrypto ()](#apidoc.element.openpgp.util.getWebCrypto)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>getWebCryptoAll ()](#apidoc.element.openpgp.util.getWebCryptoAll)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>get_hashAlgorithmString (algo)](#apidoc.element.openpgp.util.get_hashAlgorithmString)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>hex2bin (hex)](#apidoc.element.openpgp.util.hex2bin)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>hexdump (str)](#apidoc.element.openpgp.util.hexdump)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>hexidump (str)](#apidoc.element.openpgp.util.hexidump)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>hexstrdump (str)](#apidoc.element.openpgp.util.hexstrdump)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>isArray (data)](#apidoc.element.openpgp.util.isArray)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>isEmailAddress (data)](#apidoc.element.openpgp.util.isEmailAddress)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>isString (data)](#apidoc.element.openpgp.util.isString)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>isUint8Array (data)](#apidoc.element.openpgp.util.isUint8Array)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>isUserId (data)](#apidoc.element.openpgp.util.isUserId)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>print_debug (str)](#apidoc.element.openpgp.util.print_debug)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>print_debug_hexstr_dump (str, strToHex)](#apidoc.element.openpgp.util.print_debug_hexstr_dump)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>promisify (fn)](#apidoc.element.openpgp.util.promisify)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>promisifyIE11Op (cryptoOp, errmsg)](#apidoc.element.openpgp.util.promisifyIE11Op)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>readDate (bytes)](#apidoc.element.openpgp.util.readDate)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>readNumber (bytes)](#apidoc.element.openpgp.util.readNumber)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>shiftRight (value, bitcount)](#apidoc.element.openpgp.util.shiftRight)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>str2Uint8Array (str)](#apidoc.element.openpgp.util.str2Uint8Array)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>str2bin (str)](#apidoc.element.openpgp.util.str2bin)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>writeDate (time)](#apidoc.element.openpgp.util.writeDate)
1.  [function <span class="apidocSignatureSpan">openpgp.util.</span>writeNumber (n, bytes)](#apidoc.element.openpgp.util.writeNumber)



# <a name="apidoc.module.openpgp"></a>[module openpgp](#apidoc.module.openpgp)

#### <a name="apidoc.element.openpgp.AsyncProxy"></a>[function <span class="apidocSignatureSpan">openpgp.</span>AsyncProxy ()](#apidoc.element.openpgp.AsyncProxy)
- description and source-code
```javascript
function AsyncProxy() {
  var _ref = arguments.length <= 0 || arguments[0] === undefined ? {} : arguments[0];

  var _ref$path = _ref.path;
  var path = _ref$path === undefined ? 'openpgp.worker.js' : _ref$path;
  var worker = _ref.worker;
  var config = _ref.config;

  this.worker = worker || new Worker(path);
  this.worker.onmessage = this.onMessage.bind(this);
  this.worker.onerror = function (e) {
    throw new Error('Unhandled error in openpgp worker: ' + e.message + ' (' + e.filename + ':' + e.lineno + ')');
  };
  this.seedRandom(INITIAL_RANDOM_SEED);

  if (config) {
    this.worker.postMessage({ event: 'configure', config: config });
  }

  // Cannot rely on task order being maintained, use object keyed by request ID to track tasks
  this.tasks = {};
  this.currentID = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.HKP"></a>[function <span class="apidocSignatureSpan">openpgp.</span>HKP (keyServerBaseUrl)](#apidoc.element.openpgp.HKP)
- description and source-code
```javascript
function HKP(keyServerBaseUrl) {
  this._baseUrl = keyServerBaseUrl ? keyServerBaseUrl : _config2.default.keyserver;
  this._fetch = typeof window !== 'undefined' ? window.fetch : _dereq_('node-fetch');
}
```
- example usage
```shell
...
var pubkey = key.publicKeyArmored;   // '-----BEGIN PGP PUBLIC KEY BLOCK ... '
});
'''

#### Lookup public key on HKP server

'''js
var hkp = new openpgp.HKP('https://pgp.mit.edu');

var options = {
query: 'alice@example.com'
};

hkp.lookup(options).then(function(key) {
var pubkey = openpgp.key.readArmored(key);
...
```

#### <a name="apidoc.element.openpgp.Keyid"></a>[function <span class="apidocSignatureSpan">openpgp.</span>Keyid ()](#apidoc.element.openpgp.Keyid)
- description and source-code
```javascript
function Keyid() {
  this.bytes = '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.Keyring"></a>[function <span class="apidocSignatureSpan">openpgp.</span>Keyring (storeHandler)](#apidoc.element.openpgp.Keyring)
- description and source-code
```javascript
function Keyring(storeHandler) {
  this.storeHandler = storeHandler || new _localstore2.default();
  this.publicKeys = new KeyArray(this.storeHandler.loadPublic());
  this.privateKeys = new KeyArray(this.storeHandler.loadPrivate());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.Keyring.localstore"></a>[function <span class="apidocSignatureSpan">openpgp.</span>Keyring.localstore (prefix)](#apidoc.element.openpgp.Keyring.localstore)
- description and source-code
```javascript
function LocalStore(prefix) {
  prefix = prefix || 'openpgp-';
  this.publicKeysItem = prefix + this.publicKeysItem;
  this.privateKeysItem = prefix + this.privateKeysItem;
  if (typeof window !== 'undefined' && window.localStorage) {
    this.storage = window.localStorage;
  } else {
    this.storage = new (_dereq_('node-localstorage').LocalStorage)(_config2.default.node_store);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.MPI"></a>[function <span class="apidocSignatureSpan">openpgp.</span>MPI ()](#apidoc.element.openpgp.MPI)
- description and source-code
```javascript
function MPI() {
<span class="apidocCodeCommentSpan">  /** An implementation dependent integer */
</span>  this.data = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.S2K"></a>[function <span class="apidocSignatureSpan">openpgp.</span>S2K ()](#apidoc.element.openpgp.S2K)
- description and source-code
```javascript
function S2K() {
<span class="apidocCodeCommentSpan">  /** @type {module:enums.hash} */
</span>  this.algorithm = 'sha256';
  /** @type {module:enums.s2k} */
  this.type = 'iterated';
  this.c = 96;
  /** Eight bytes of salt in a binary string.
   * @type {String}
   */
  this.salt = _crypto2.default.random.getRandomBytes(8);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.cleartext.CleartextMessage"></a>[function <span class="apidocSignatureSpan">openpgp.</span>cleartext.CleartextMessage (text, signature)](#apidoc.element.openpgp.cleartext.CleartextMessage)
- description and source-code
```javascript
function CleartextMessage(text, signature) {
  if (!(this instanceof CleartextMessage)) {
    return new CleartextMessage(text, signature);
  }
  // normalize EOL to canonical form <CR><LF>
  this.text = text.replace(/\r/g, '').replace(/[\t ]+\n/g, "\n").replace(/\n/g, "\r\n");
  if (signature && !(signature instanceof sigModule.Signature)) {
    throw new Error('Invalid signature input');
  }
  this.signature = signature || new sigModule.Signature(new _packet2.default.List());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.decrypt"></a>[function <span class="apidocSignatureSpan">openpgp.</span>decrypt (_ref6)](#apidoc.element.openpgp.decrypt)
- description and source-code
```javascript
function decrypt(_ref6) {
  var message = _ref6.message;
  var privateKey = _ref6.privateKey;
  var publicKeys = _ref6.publicKeys;
  var sessionKey = _ref6.sessionKey;
  var password = _ref6.password;
  var _ref6$format = _ref6.format;
  var format = _ref6$format === undefined ? 'utf8' : _ref6$format;
  var _ref6$signature = _ref6.signature;
  var signature = _ref6$signature === undefined ? null : _ref6$signature;

  checkMessage(message);publicKeys = toArray(publicKeys);

  if (!nativeAEAD() && asyncProxy) {
    // use web worker if web crypto apis are not supported
    return asyncProxy.delegate('decrypt', { message: message, privateKey: privateKey, publicKeys: publicKeys, sessionKey: sessionKey
, password: password, format: format, signature: signature });
  }

  return message.decrypt(privateKey, sessionKey, password).then(function (message) {

    var result = parseMessage(message, format);
    if (result.data) {
      // verify
      if (!publicKeys) {
        publicKeys = [];
      }
      if (signature) {
        //detached signature
        result.signatures = message.verifyDetached(signature, publicKeys);
      } else {
        result.signatures = message.verify(publicKeys);
      }
    }
    return result;
  }).catch(onError.bind(null, 'Error decrypting message'));
}
```
- example usage
```shell
...
'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
'''

#### Encrypt and decrypt *String* data with PGP keys

'''js
...
```

#### <a name="apidoc.element.openpgp.decryptKey"></a>[function <span class="apidocSignatureSpan">openpgp.</span>decryptKey (_ref4)](#apidoc.element.openpgp.decryptKey)
- description and source-code
```javascript
function decryptKey(_ref4) {
  var privateKey = _ref4.privateKey;
  var passphrase = _ref4.passphrase;

  if (asyncProxy) {
    // use web worker if available
    return asyncProxy.delegate('decryptKey', { privateKey: privateKey, passphrase: passphrase });
  }

  return execute(function () {

    if (!privateKey.decrypt(passphrase)) {
      throw new Error('Invalid passphrase');
    }
    return {
      key: privateKey
    };
  }, 'Error decrypting private key');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.decryptSessionKey"></a>[function <span class="apidocSignatureSpan">openpgp.</span>decryptSessionKey (_ref10)](#apidoc.element.openpgp.decryptSessionKey)
- description and source-code
```javascript
function decryptSessionKey(_ref10) {
  var message = _ref10.message;
  var privateKey = _ref10.privateKey;
  var password = _ref10.password;

  checkMessage(message);

  if (asyncProxy) {
    // use web worker if available
    return asyncProxy.delegate('decryptSessionKey', { message: message, privateKey: privateKey, password: password });
  }

  return execute(function () {
    return message.decryptSessionKey(privateKey, password);
  }, 'Error decrypting session key');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.destroyWorker"></a>[function <span class="apidocSignatureSpan">openpgp.</span>destroyWorker ()](#apidoc.element.openpgp.destroyWorker)
- description and source-code
```javascript
function destroyWorker() {
  asyncProxy = undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.encrypt"></a>[function <span class="apidocSignatureSpan">openpgp.</span>encrypt (_ref5)](#apidoc.element.openpgp.encrypt)
- description and source-code
```javascript
function encrypt(_ref5) {
  var data = _ref5.data;
  var publicKeys = _ref5.publicKeys;
  var privateKeys = _ref5.privateKeys;
  var passwords = _ref5.passwords;
  var filename = _ref5.filename;
  var _ref5$armor = _ref5.armor;
  var armor = _ref5$armor === undefined ? true : _ref5$armor;
  var _ref5$detached = _ref5.detached;
  var detached = _ref5$detached === undefined ? false : _ref5$detached;
  var _ref5$signature = _ref5.signature;
  var signature = _ref5$signature === undefined ? null : _ref5$signature;

  checkData(data);publicKeys = toArray(publicKeys);privateKeys = toArray(privateKeys);passwords = toArray(passwords);

  if (!nativeAEAD() && asyncProxy) {
    // use web worker if web crypto apis are not supported
    return asyncProxy.delegate('encrypt', { data: data, publicKeys: publicKeys, privateKeys: privateKeys, passwords: passwords,
filename: filename, armor: armor, detached: detached, signature: signature });
  }
  var result = {};
  return Promise.resolve().then(function () {

    var message = createMessage(data, filename);
    if (!privateKeys) {
      privateKeys = [];
    }
    if (privateKeys.length || signature) {
      // sign the message only if private keys or signature is specified
      if (detached) {
        var detachedSignature = message.signDetached(privateKeys, signature);
        if (armor) {
          result.signature = detachedSignature.armor();
        } else {
          result.signature = detachedSignature;
        }
      } else {
        message = message.sign(privateKeys, signature);
      }
    }
    return message.encrypt(publicKeys, passwords);
  }).then(function (message) {
    if (armor) {
      result.data = message.armor();
    } else {
      result.message = message;
    }
    return result;
  }).catch(onError.bind(null, 'Error encrypting message'));
}
```
- example usage
```shell
...

options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
...
```

#### <a name="apidoc.element.openpgp.encryptSessionKey"></a>[function <span class="apidocSignatureSpan">openpgp.</span>encryptSessionKey (_ref9)](#apidoc.element.openpgp.encryptSessionKey)
- description and source-code
```javascript
function encryptSessionKey(_ref9) {
  var data = _ref9.data;
  var algorithm = _ref9.algorithm;
  var publicKeys = _ref9.publicKeys;
  var passwords = _ref9.passwords;

  checkbinary(data);checkString(algorithm, 'algorithm');publicKeys = toArray(publicKeys);passwords = toArray(passwords);

  if (asyncProxy) {
    // use web worker if available
    return asyncProxy.delegate('encryptSessionKey', { data: data, algorithm: algorithm, publicKeys: publicKeys, passwords: passwords
 });
  }

  return execute(function () {
    return {

      message: messageLib.encryptSessionKey(data, algorithm, publicKeys, passwords)

    };
  }, 'Error encrypting session key');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.generateKey"></a>[function <span class="apidocSignatureSpan">openpgp.</span>generateKey ()](#apidoc.element.openpgp.generateKey)
- description and source-code
```javascript
function generateKey() {
  var _ref2 = arguments.length <= 0 || arguments[0] === undefined ? {} : arguments[0];

  var _ref2$userIds = _ref2.userIds;
  var userIds = _ref2$userIds === undefined ? [] : _ref2$userIds;
  var passphrase = _ref2.passphrase;
  var _ref2$numBits = _ref2.numBits;
  var numBits = _ref2$numBits === undefined ? 2048 : _ref2$numBits;
  var _ref2$unlocked = _ref2.unlocked;
  var unlocked = _ref2$unlocked === undefined ? false : _ref2$unlocked;
  var _ref2$keyExpirationTi = _ref2.keyExpirationTime;
  var keyExpirationTime = _ref2$keyExpirationTi === undefined ? 0 : _ref2$keyExpirationTi;

  var options = formatUserIds({ userIds: userIds, passphrase: passphrase, numBits: numBits, unlocked: unlocked, keyExpirationTime
: keyExpirationTime });

  if (!_util2.default.getWebCryptoAll() && asyncProxy) {
    // use web worker if web crypto apis are not supported
    return asyncProxy.delegate('generateKey', options);
  }

  return key.generate(options).then(function (newKey) {
    return {

      key: newKey,
      privateKeyArmored: newKey.armor(),
      publicKeyArmored: newKey.toPublic().armor()

    };
  }).catch(onError.bind(null, 'Error generating keypair'));
}
```
- example usage
```shell
...
'''js
var options = {
    userIds: [{ name:'Jon Smith', email:'jon@example.com' }], // multiple user IDs
    numBits: 4096,                                            // RSA key size
    passphrase: 'super long and hard to guess secret'         // protects the private key
};

openpgp.generateKey(options).then(function(key) {
    var privkey = key.privateKeyArmored; // '-----BEGIN PGP PRIVATE KEY BLOCK ... '
    var pubkey = key.publicKeyArmored;   // '-----BEGIN PGP PUBLIC KEY BLOCK ... '
});
'''

#### Lookup public key on HKP server
...
```

#### <a name="apidoc.element.openpgp.getWorker"></a>[function <span class="apidocSignatureSpan">openpgp.</span>getWorker ()](#apidoc.element.openpgp.getWorker)
- description and source-code
```javascript
function getWorker() {
  return asyncProxy;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.initWorker"></a>[function <span class="apidocSignatureSpan">openpgp.</span>initWorker ()](#apidoc.element.openpgp.initWorker)
- description and source-code
```javascript
function initWorker() {
  var _ref = arguments.length <= 0 || arguments[0] === undefined ? {} : arguments[0];

  var _ref$path = _ref.path;
  var path = _ref$path === undefined ? 'openpgp.worker.js' : _ref$path;
  var worker = _ref.worker;

  if (worker || typeof window !== 'undefined' && window.Worker) {
    asyncProxy = new _async_proxy2.default({ path: path, worker: worker, config: _config2.default });
    return true;
  }
}
```
- example usage
```shell
...
Here are some examples of how to use the v2.x api. For more elaborate examples and working code, please check out the [public api
 unit tests](https://github.com/openpgpjs/openpgpjs/blob/master/test/general/openpgp.js). If you're upgrading from v1.x it might
 help to check out the [documentation](https://github.com/openpgpjs/openpgpjs#documentation).

#### Set up

'''js
var openpgp = require('openpgp'); // use as CommonJS, AMD, ES6 module or via window.openpgp

openpgp.initWorker({ path:'openpgp.worker.js' }) // set the relative web worker path

openpgp.config.aead_protect = true // activate fast AES-GCM mode (not yet OpenPGP standard)
'''

#### Encrypt and decrypt *Uint8Array* data with a password

'''js
...
```

#### <a name="apidoc.element.openpgp.key.Key"></a>[function <span class="apidocSignatureSpan">openpgp.</span>key.Key (packetlist)](#apidoc.element.openpgp.key.Key)
- description and source-code
```javascript
function Key(packetlist) {
  if (!(this instanceof Key)) {
    return new Key(packetlist);
  }
  // same data as in packetlist but in structured form
  this.primaryKey = null;
  this.revocationSignature = null;
  this.directSignatures = null;
  this.users = null;
  this.subKeys = null;
  this.packetlist2structure(packetlist);
  if (!this.primaryKey || !this.users) {
    throw new Error('Invalid key: need at least key and user ID packet');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.message.Message"></a>[function <span class="apidocSignatureSpan">openpgp.</span>message.Message (packetlist)](#apidoc.element.openpgp.message.Message)
- description and source-code
```javascript
function Message(packetlist) {
  if (!(this instanceof Message)) {
    return new Message(packetlist);
  }
  this.packets = packetlist || new _packet2.default.List();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Compressed"></a>[function <span class="apidocSignatureSpan">openpgp.</span>packet.Compressed ()](#apidoc.element.openpgp.packet.Compressed)
- description and source-code
```javascript
function Compressed() {
<span class="apidocCodeCommentSpan">  /**
   * Packet type
   * @type {module:enums.packet}
   */
</span>  this.tag = _enums2.default.packet.compressed;
  /**
   * List of packets
   * @type {module:packet/packetlist}
   */
  this.packets = null;
  /**
   * Compression algorithm
   * @type {compression}
   */
  this.algorithm = 'zip';

  /**
   * Compressed packet data
   * @type {String}
   */
  this.compressed = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.List"></a>[function <span class="apidocSignatureSpan">openpgp.</span>packet.List ()](#apidoc.element.openpgp.packet.List)
- description and source-code
```javascript
function Packetlist() {
<span class="apidocCodeCommentSpan">  /** The number of packets contained within the list.
   * @readonly
   * @type {Integer} */
</span>  this.length = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Literal"></a>[function <span class="apidocSignatureSpan">openpgp.</span>packet.Literal ()](#apidoc.element.openpgp.packet.Literal)
- description and source-code
```javascript
function Literal() {
  this.tag = _enums2.default.packet.literal;
  this.format = 'utf8'; // default format for literal data packets
  this.date = new Date();
  this.data = new Uint8Array(0); // literal data representation
  this.filename = 'msg.txt';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Marker"></a>[function <span class="apidocSignatureSpan">openpgp.</span>packet.Marker ()](#apidoc.element.openpgp.packet.Marker)
- description and source-code
```javascript
function Marker() {
  this.tag = _enums2.default.packet.marker;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.OnePassSignature"></a>[function <span class="apidocSignatureSpan">openpgp.</span>packet.OnePassSignature ()](#apidoc.element.openpgp.packet.OnePassSignature)
- description and source-code
```javascript
function OnePassSignature() {
  this.tag = _enums2.default.packet.onePassSignature; // The packet type
  this.version = null; // A one-octet version number.  The current version is 3.
  this.type = null; // A one-octet signature type.  Signature types are described in {@link http://tools.ietf.org/html/rfc4880#section
-5.2.1|RFC4880 Section 5.2.1}.
  this.hashAlgorithm = null; // A one-octet number describing the hash algorithm used. (See {@link http://tools.ietf.org/html/rfc4880
#section-9.4|RFC4880 9.4})
  this.publicKeyAlgorithm = null; // A one-octet number describing the public-key algorithm used. (See {@link http://tools.ietf.
org/html/rfc4880#section-9.1|RFC4880 9.1})
  this.signingKeyId = null; // An eight-octet number holding the Key ID of the signing key.
  this.flags = null; //  A one-octet number holding a flag showing whether the signature is nested.  A zero value indicates that
 the next packet is another One-Pass Signature packet that describes another signature to be applied to the same message data.
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.PublicKey"></a>[function <span class="apidocSignatureSpan">openpgp.</span>packet.PublicKey ()](#apidoc.element.openpgp.packet.PublicKey)
- description and source-code
```javascript
function PublicKey() {
  this.tag = _enums2.default.packet.publicKey;
  this.version = 4;
<span class="apidocCodeCommentSpan">  /** Key creation date.
   * @type {Date} */
</span>  this.created = new Date();
  /** A list of multiprecision integers
   * @type {module:type/mpi} */
  this.mpi = [];
  /** Public key algorithm
   * @type {module:enums.publicKey} */
  this.algorithm = 'rsa_sign';
  // time in days (V3 only)
  this.expirationTimeV3 = 0;
  /**
   * Fingerprint in lowercase hex
   * @type {String}
   */
  this.fingerprint = null;
  /**
   * Keyid
   * @type {module:type/keyid}
   */
  this.keyid = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey"></a>[function <span class="apidocSignatureSpan">openpgp.</span>packet.PublicKeyEncryptedSessionKey ()](#apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey)
- description and source-code
```javascript
function PublicKeyEncryptedSessionKey() {
  this.tag = _enums2.default.packet.publicKeyEncryptedSessionKey;
  this.version = 3;

  this.publicKeyId = new _keyid2.default();
  this.publicKeyAlgorithm = 'rsa_encrypt';

  this.sessionKey = null;
  this.sessionKeyAlgorithm = 'aes256';

<span class="apidocCodeCommentSpan">  /** @type {Array<module:type/mpi>} */
</span>  this.encrypted = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.PublicSubkey"></a>[function <span class="apidocSignatureSpan">openpgp.</span>packet.PublicSubkey ()](#apidoc.element.openpgp.packet.PublicSubkey)
- description and source-code
```javascript
function PublicSubkey() {
  _public_key2.default.call(this);
  this.tag = _enums2.default.packet.publicSubkey;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.SecretKey"></a>[function <span class="apidocSignatureSpan">openpgp.</span>packet.SecretKey ()](#apidoc.element.openpgp.packet.SecretKey)
- description and source-code
```javascript
function SecretKey() {
  _public_key2.default.call(this);
  this.tag = _enums2.default.packet.secretKey;
  // encrypted secret-key data
  this.encrypted = null;
  // indicator if secret-key data is available in decrypted form
  this.isDecrypted = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.SecretSubkey"></a>[function <span class="apidocSignatureSpan">openpgp.</span>packet.SecretSubkey ()](#apidoc.element.openpgp.packet.SecretSubkey)
- description and source-code
```javascript
function SecretSubkey() {
  _secret_key2.default.call(this);
  this.tag = _enums2.default.packet.secretSubkey;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Signature"></a>[function <span class="apidocSignatureSpan">openpgp.</span>packet.Signature ()](#apidoc.element.openpgp.packet.Signature)
- description and source-code
```javascript
function Signature() {
  this.tag = _enums2.default.packet.signature;
  this.version = 4;
  this.signatureType = null;
  this.hashAlgorithm = null;
  this.publicKeyAlgorithm = null;

  this.signatureData = null;
  this.unhashedSubpackets = null;
  this.signedHashValue = null;

  this.created = new Date();
  this.signatureExpirationTime = null;
  this.signatureNeverExpires = true;
  this.exportable = null;
  this.trustLevel = null;
  this.trustAmount = null;
  this.regularExpression = null;
  this.revocable = null;
  this.keyExpirationTime = null;
  this.keyNeverExpires = null;
  this.preferredSymmetricAlgorithms = null;
  this.revocationKeyClass = null;
  this.revocationKeyAlgorithm = null;
  this.revocationKeyFingerprint = null;
  this.issuerKeyId = new _keyid2.default();
  this.notation = null;
  this.preferredHashAlgorithms = null;
  this.preferredCompressionAlgorithms = null;
  this.keyServerPreferences = null;
  this.preferredKeyServer = null;
  this.isPrimaryUserID = null;
  this.policyURI = null;
  this.keyFlags = null;
  this.signersUserId = null;
  this.reasonForRevocationFlag = null;
  this.reasonForRevocationString = null;
  this.features = null;
  this.signatureTargetPublicKeyAlgorithm = null;
  this.signatureTargetHashAlgorithm = null;
  this.signatureTargetHash = null;
  this.embeddedSignature = null;

  this.verified = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.SymEncryptedAEADProtected"></a>[function <span class="apidocSignatureSpan">openpgp.</span>packet.SymEncryptedAEADProtected ()](#apidoc.element.openpgp.packet.SymEncryptedAEADProtected)
- description and source-code
```javascript
function SymEncryptedAEADProtected() {
  this.tag = _enums2.default.packet.symEncryptedAEADProtected;
  this.version = VERSION;
  this.iv = null;
  this.encrypted = null;
  this.packets = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.SymEncryptedIntegrityProtected"></a>[function <span class="apidocSignatureSpan">openpgp.</span>packet.SymEncryptedIntegrityProtected ()](#apidoc.element.openpgp.packet.SymEncryptedIntegrityProtected)
- description and source-code
```javascript
function SymEncryptedIntegrityProtected() {
  this.tag = _enums2.default.packet.symEncryptedIntegrityProtected;
  this.version = VERSION;
<span class="apidocCodeCommentSpan">  /** The encrypted payload. */
</span>  this.encrypted = null; // string
  /**
   * If after decrypting the packet this is set to true,
   * a modification has been detected and thus the contents
   * should be discarded.
   * @type {Boolean}
   */
  this.modification = false;
  this.packets = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.SymEncryptedSessionKey"></a>[function <span class="apidocSignatureSpan">openpgp.</span>packet.SymEncryptedSessionKey ()](#apidoc.element.openpgp.packet.SymEncryptedSessionKey)
- description and source-code
```javascript
function SymEncryptedSessionKey() {
  this.tag = _enums2.default.packet.symEncryptedSessionKey;
  this.version = 4;
  this.sessionKey = null;
  this.sessionKeyEncryptionAlgorithm = null;
  this.sessionKeyAlgorithm = 'aes256';
  this.encrypted = null;
  this.s2k = new _s2k2.default();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.SymmetricallyEncrypted"></a>[function <span class="apidocSignatureSpan">openpgp.</span>packet.SymmetricallyEncrypted ()](#apidoc.element.openpgp.packet.SymmetricallyEncrypted)
- description and source-code
```javascript
function SymmetricallyEncrypted() {
  this.tag = _enums2.default.packet.symmetricallyEncrypted;
  this.encrypted = null;
<span class="apidocCodeCommentSpan">  /** Decrypted packets contained within.
   * @type {module:packet/packetlist} */
</span>  this.packets = null;
  this.ignore_mdc_error = _config2.default.ignore_mdc_error;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Trust"></a>[function <span class="apidocSignatureSpan">openpgp.</span>packet.Trust ()](#apidoc.element.openpgp.packet.Trust)
- description and source-code
```javascript
function Trust() {
  this.tag = _enums2.default.packet.trust;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.UserAttribute"></a>[function <span class="apidocSignatureSpan">openpgp.</span>packet.UserAttribute ()](#apidoc.element.openpgp.packet.UserAttribute)
- description and source-code
```javascript
function UserAttribute() {
  this.tag = _enums2.default.packet.userAttribute;
  this.attributes = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Userid"></a>[function <span class="apidocSignatureSpan">openpgp.</span>packet.Userid ()](#apidoc.element.openpgp.packet.Userid)
- description and source-code
```javascript
function Userid() {
  this.tag = _enums2.default.packet.userid;
<span class="apidocCodeCommentSpan">  /** A string containing the user id. Usually in the form
   * John Doe <john@example.com>
   * @type {String}
   */
</span>  this.userid = '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.reformatKey"></a>[function <span class="apidocSignatureSpan">openpgp.</span>reformatKey ()](#apidoc.element.openpgp.reformatKey)
- description and source-code
```javascript
function reformatKey() {
  var _ref3 = arguments.length <= 0 || arguments[0] === undefined ? {} : arguments[0];

  var privateKey = _ref3.privateKey;
  var _ref3$userIds = _ref3.userIds;
  var userIds = _ref3$userIds === undefined ? [] : _ref3$userIds;
  var _ref3$passphrase = _ref3.passphrase;
  var passphrase = _ref3$passphrase === undefined ? "" : _ref3$passphrase;
  var _ref3$unlocked = _ref3.unlocked;
  var unlocked = _ref3$unlocked === undefined ? false : _ref3$unlocked;
  var _ref3$keyExpirationTi = _ref3.keyExpirationTime;
  var keyExpirationTime = _ref3$keyExpirationTi === undefined ? 0 : _ref3$keyExpirationTi;

  var options = formatUserIds({ privateKey: privateKey, userIds: userIds, passphrase: passphrase, unlocked: unlocked, keyExpirationTime
: keyExpirationTime });

  if (asyncProxy) {
    return asyncProxy.delegate('reformatKey', options);
  }

  return key.reformat(options).then(function (newKey) {
    return {

      key: newKey,
      privateKeyArmored: newKey.armor(),
      publicKeyArmored: newKey.toPublic().armor()

    };
  }).catch(onError.bind(null, 'Error reformatting keypair'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.sign"></a>[function <span class="apidocSignatureSpan">openpgp.</span>sign (_ref7)](#apidoc.element.openpgp.sign)
- description and source-code
```javascript
function sign(_ref7) {
  var data = _ref7.data;
  var privateKeys = _ref7.privateKeys;
  var _ref7$armor = _ref7.armor;
  var armor = _ref7$armor === undefined ? true : _ref7$armor;
  var _ref7$detached = _ref7.detached;
  var detached = _ref7$detached === undefined ? false : _ref7$detached;

  checkString(data);
  privateKeys = toArray(privateKeys);

  if (asyncProxy) {
    // use web worker if available
    return asyncProxy.delegate('sign', { data: data, privateKeys: privateKeys, armor: armor, detached: detached });
  }

  var result = {};
  return execute(function () {

    var cleartextMessage = new cleartext.CleartextMessage(data);

    if (detached) {
      var signature = cleartextMessage.signDetached(privateKeys);
      if (armor) {
        result.signature = signature.armor();
      } else {
        result.signature = signature;
      }
    } else {
      cleartextMessage.sign(privateKeys);
    }

    if (armor) {
      result.data = cleartextMessage.armor();
    } else {
      result.message = cleartextMessage;
    }
    return result;
  }, 'Error signing cleartext message');
}
```
- example usage
```shell
...

'''js
options = {
data: 'Hello, World!',                             // input as String (or Uint8Array)
privateKeys: privKeyObj // for signing
};

openpgp.sign(options).then(function(signed) {
cleartext = signed.data; // '-----BEGIN PGP SIGNED MESSAGE ... END PGP SIGNATURE-----'
});
'''

'''js
options = {
message: openpgp.cleartext.readArmored(cleartext), // parse armored message
...
```

#### <a name="apidoc.element.openpgp.signature.Signature"></a>[function <span class="apidocSignatureSpan">openpgp.</span>signature.Signature (packetlist)](#apidoc.element.openpgp.signature.Signature)
- description and source-code
```javascript
function Signature(packetlist) {
  if (!(this instanceof Signature)) {
    return new Signature(packetlist);
  }
  this.packets = packetlist || new _packet2.default.List();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.verify"></a>[function <span class="apidocSignatureSpan">openpgp.</span>verify (_ref8)](#apidoc.element.openpgp.verify)
- description and source-code
```javascript
function verify(_ref8) {
  var message = _ref8.message;
  var publicKeys = _ref8.publicKeys;
  var _ref8$signature = _ref8.signature;
  var signature = _ref8$signature === undefined ? null : _ref8$signature;

  checkCleartextMessage(message);
  publicKeys = toArray(publicKeys);

  if (asyncProxy) {
    // use web worker if available
    return asyncProxy.delegate('verify', { message: message, publicKeys: publicKeys, signature: signature });
  }

  var result = {};
  return execute(function () {
    result.data = message.getText();

    if (signature) {
      //detached signature
      result.signatures = message.verifyDetached(signature, publicKeys);
    } else {
      result.signatures = message.verify(publicKeys);
    }
    return result;
  }, 'Error verifying cleartext signed message');
}
```
- example usage
```shell
...

'''js
options = {
    message: openpgp.cleartext.readArmored(cleartext), // parse armored message
    publicKeys: openpgp.key.readArmored(pubkey).keys   // for verification
};

openpgp.verify(options).then(function(verified) {
	validity = verified.signatures[0].valid; // true
	if (validity) {
		console.log('signed by key id ' + verified.signatures[0].keyid.toHex());
	}
});
'''
...
```



# <a name="apidoc.module.openpgp.AsyncProxy"></a>[module openpgp.AsyncProxy](#apidoc.module.openpgp.AsyncProxy)

#### <a name="apidoc.element.openpgp.AsyncProxy.AsyncProxy"></a>[function <span class="apidocSignatureSpan">openpgp.</span>AsyncProxy ()](#apidoc.element.openpgp.AsyncProxy.AsyncProxy)
- description and source-code
```javascript
function AsyncProxy() {
  var _ref = arguments.length <= 0 || arguments[0] === undefined ? {} : arguments[0];

  var _ref$path = _ref.path;
  var path = _ref$path === undefined ? 'openpgp.worker.js' : _ref$path;
  var worker = _ref.worker;
  var config = _ref.config;

  this.worker = worker || new Worker(path);
  this.worker.onmessage = this.onMessage.bind(this);
  this.worker.onerror = function (e) {
    throw new Error('Unhandled error in openpgp worker: ' + e.message + ' (' + e.filename + ':' + e.lineno + ')');
  };
  this.seedRandom(INITIAL_RANDOM_SEED);

  if (config) {
    this.worker.postMessage({ event: 'configure', config: config });
  }

  // Cannot rely on task order being maintained, use object keyed by request ID to track tasks
  this.tasks = {};
  this.currentID = 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.AsyncProxy.prototype"></a>[module openpgp.AsyncProxy.prototype](#apidoc.module.openpgp.AsyncProxy.prototype)

#### <a name="apidoc.element.openpgp.AsyncProxy.prototype.delegate"></a>[function <span class="apidocSignatureSpan">openpgp.AsyncProxy.prototype.</span>delegate (method, options)](#apidoc.element.openpgp.AsyncProxy.prototype.delegate)
- description and source-code
```javascript
delegate = function (method, options) {
  var _this = this;

  var id = this.getID();

  return new Promise(function (_resolve, reject) {
    // clone packets (for web worker structured cloning algorithm)
    _this.worker.postMessage({ id: id, event: method, options: _packet2.default.clone.clonePackets(options) }, _util2.default.getTransferables
.call(_util2.default, options));

    // remember to handle parsing cloned packets from worker
    _this.tasks[id] = { resolve: function resolve(data) {
        return _resolve(_packet2.default.clone.parseClonedPackets(data, method));
      }, reject: reject };
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.AsyncProxy.prototype.getID"></a>[function <span class="apidocSignatureSpan">openpgp.AsyncProxy.prototype.</span>getID ()](#apidoc.element.openpgp.AsyncProxy.prototype.getID)
- description and source-code
```javascript
getID = function () {
  return this.currentID++;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.AsyncProxy.prototype.getRandomBuffer"></a>[function <span class="apidocSignatureSpan">openpgp.AsyncProxy.prototype.</span>getRandomBuffer (size)](#apidoc.element.openpgp.AsyncProxy.prototype.getRandomBuffer)
- description and source-code
```javascript
getRandomBuffer = function (size) {
  if (!size) {
    return null;
  }
  var buf = new Uint8Array(size);
  _crypto2.default.random.getRandomValues(buf);
  return buf;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.AsyncProxy.prototype.onMessage"></a>[function <span class="apidocSignatureSpan">openpgp.AsyncProxy.prototype.</span>onMessage (event)](#apidoc.element.openpgp.AsyncProxy.prototype.onMessage)
- description and source-code
```javascript
onMessage = function (event) {
  var msg = event.data;
  switch (msg.event) {
    case 'method-return':
      if (msg.err) {
        // fail
        this.tasks[msg.id].reject(new Error(msg.err));
      } else {
        // success
        this.tasks[msg.id].resolve(msg.data);
      }
      delete this.tasks[msg.id];
      break;
    case 'request-seed':
      this.seedRandom(RANDOM_SEED_REQUEST);
      break;
    default:
      throw new Error('Unknown Worker Event.');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.AsyncProxy.prototype.seedRandom"></a>[function <span class="apidocSignatureSpan">openpgp.AsyncProxy.prototype.</span>seedRandom (size)](#apidoc.element.openpgp.AsyncProxy.prototype.seedRandom)
- description and source-code
```javascript
seedRandom = function (size) {
  var buf = this.getRandomBuffer(size);
  this.worker.postMessage({ event: 'seed-random', buf: buf }, _util2.default.getTransferables.call(_util2.default, buf));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.AsyncProxy.prototype.terminate"></a>[function <span class="apidocSignatureSpan">openpgp.AsyncProxy.prototype.</span>terminate ()](#apidoc.element.openpgp.AsyncProxy.prototype.terminate)
- description and source-code
```javascript
terminate = function () {
  this.worker.terminate();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.HKP"></a>[module openpgp.HKP](#apidoc.module.openpgp.HKP)

#### <a name="apidoc.element.openpgp.HKP.HKP"></a>[function <span class="apidocSignatureSpan">openpgp.</span>HKP (keyServerBaseUrl)](#apidoc.element.openpgp.HKP.HKP)
- description and source-code
```javascript
function HKP(keyServerBaseUrl) {
  this._baseUrl = keyServerBaseUrl ? keyServerBaseUrl : _config2.default.keyserver;
  this._fetch = typeof window !== 'undefined' ? window.fetch : _dereq_('node-fetch');
}
```
- example usage
```shell
...
var pubkey = key.publicKeyArmored;   // '-----BEGIN PGP PUBLIC KEY BLOCK ... '
});
'''

#### Lookup public key on HKP server

'''js
var hkp = new openpgp.HKP('https://pgp.mit.edu');

var options = {
query: 'alice@example.com'
};

hkp.lookup(options).then(function(key) {
var pubkey = openpgp.key.readArmored(key);
...
```



# <a name="apidoc.module.openpgp.HKP.prototype"></a>[module openpgp.HKP.prototype](#apidoc.module.openpgp.HKP.prototype)

#### <a name="apidoc.element.openpgp.HKP.prototype.lookup"></a>[function <span class="apidocSignatureSpan">openpgp.HKP.prototype.</span>lookup (options)](#apidoc.element.openpgp.HKP.prototype.lookup)
- description and source-code
```javascript
lookup = function (options) {
  var uri = this._baseUrl + '/pks/lookup?op=get&options=mr&search=',
      fetch = this._fetch;

  if (options.keyId) {
    uri += '0x' + encodeURIComponent(options.keyId);
  } else if (options.query) {
    uri += encodeURIComponent(options.query);
  } else {
    throw new Error('You must provide a query parameter!');
  }

  return fetch(uri).then(function (response) {
    if (response.status === 200) {
      return response.text();
    }
  }).then(function (publicKeyArmored) {
    if (!publicKeyArmored || publicKeyArmored.indexOf('-----END PGP PUBLIC KEY BLOCK-----') < 0) {
      return;
    }
    return publicKeyArmored.trim();
  });
}
```
- example usage
```shell
...
'''js
var hkp = new openpgp.HKP('https://pgp.mit.edu');

var options = {
    query: 'alice@example.com'
};

hkp.lookup(options).then(function(key) {
    var pubkey = openpgp.key.readArmored(key);
});
'''

#### Upload public key to HKP server

'''js
...
```

#### <a name="apidoc.element.openpgp.HKP.prototype.upload"></a>[function <span class="apidocSignatureSpan">openpgp.HKP.prototype.</span>upload (publicKeyArmored)](#apidoc.element.openpgp.HKP.prototype.upload)
- description and source-code
```javascript
upload = function (publicKeyArmored) {
  var uri = this._baseUrl + '/pks/add',
      fetch = this._fetch;

  return fetch(uri, {
    method: 'post',
    headers: {
      'Content-Type': 'application/x-www-form-urlencoded; charset=UTF-8'
    },
    body: 'keytext=' + encodeURIComponent(publicKeyArmored)
  });
}
```
- example usage
```shell
...
#### Upload public key to HKP server

'''js
var hkp = new openpgp.HKP('https://pgp.mit.edu');

var pubkey = '-----BEGIN PGP PUBLIC KEY BLOCK ... END PGP PUBLIC KEY BLOCK-----';

hkp.upload(pubkey).then(function() { ... });
'''

#### Sign and verify cleartext messages

'''js
var options, cleartext, validity;
...
```



# <a name="apidoc.module.openpgp.Keyid"></a>[module openpgp.Keyid](#apidoc.module.openpgp.Keyid)

#### <a name="apidoc.element.openpgp.Keyid.Keyid"></a>[function <span class="apidocSignatureSpan">openpgp.</span>Keyid ()](#apidoc.element.openpgp.Keyid.Keyid)
- description and source-code
```javascript
function Keyid() {
  this.bytes = '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.Keyid.fromClone"></a>[function <span class="apidocSignatureSpan">openpgp.Keyid.</span>fromClone (clone)](#apidoc.element.openpgp.Keyid.fromClone)
- description and source-code
```javascript
fromClone = function (clone) {
  var keyid = new Keyid();
  keyid.bytes = clone.bytes;
  return keyid;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.Keyid.fromId"></a>[function <span class="apidocSignatureSpan">openpgp.Keyid.</span>fromId (hex)](#apidoc.element.openpgp.Keyid.fromId)
- description and source-code
```javascript
fromId = function (hex) {
  var keyid = new Keyid();
  keyid.read(_util2.default.str2Uint8Array(_util2.default.hex2bin(hex)));
  return keyid;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.Keyid.mapToHex"></a>[function <span class="apidocSignatureSpan">openpgp.Keyid.</span>mapToHex (keyId)](#apidoc.element.openpgp.Keyid.mapToHex)
- description and source-code
```javascript
mapToHex = function (keyId) {
  return keyId.toHex();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.Keyid.prototype"></a>[module openpgp.Keyid.prototype](#apidoc.module.openpgp.Keyid.prototype)

#### <a name="apidoc.element.openpgp.Keyid.prototype.equals"></a>[function <span class="apidocSignatureSpan">openpgp.Keyid.prototype.</span>equals (keyid)](#apidoc.element.openpgp.Keyid.prototype.equals)
- description and source-code
```javascript
equals = function (keyid) {
  return this.bytes === keyid.bytes;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.Keyid.prototype.isNull"></a>[function <span class="apidocSignatureSpan">openpgp.Keyid.prototype.</span>isNull ()](#apidoc.element.openpgp.Keyid.prototype.isNull)
- description and source-code
```javascript
isNull = function () {
  return this.bytes === '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.Keyid.prototype.read"></a>[function <span class="apidocSignatureSpan">openpgp.Keyid.prototype.</span>read (bytes)](#apidoc.element.openpgp.Keyid.prototype.read)
- description and source-code
```javascript
read = function (bytes) {
  this.bytes = _util2.default.Uint8Array2str(bytes.subarray(0, 8));
}
```
- example usage
```shell
...
openpgp.encrypt(options).then(function(ciphertext) {
    encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
...
```

#### <a name="apidoc.element.openpgp.Keyid.prototype.toHex"></a>[function <span class="apidocSignatureSpan">openpgp.Keyid.prototype.</span>toHex ()](#apidoc.element.openpgp.Keyid.prototype.toHex)
- description and source-code
```javascript
toHex = function () {
  return _util2.default.hexstrdump(this.bytes);
}
```
- example usage
```shell
...
    message: openpgp.cleartext.readArmored(cleartext), // parse armored message
    publicKeys: openpgp.key.readArmored(pubkey).keys   // for verification
};

openpgp.verify(options).then(function(verified) {
	validity = verified.signatures[0].valid; // true
	if (validity) {
		console.log('signed by key id ' + verified.signatures[0].keyid.toHex());
	}
});
'''

#### Create and verify *detached* signatures

'''js
...
```

#### <a name="apidoc.element.openpgp.Keyid.prototype.write"></a>[function <span class="apidocSignatureSpan">openpgp.Keyid.prototype.</span>write ()](#apidoc.element.openpgp.Keyid.prototype.write)
- description and source-code
```javascript
write = function () {
  return _util2.default.str2Uint8Array(this.bytes);
}
```
- example usage
```shell
...
options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
password: 'secret stuff',                 // decrypt with password
...
```



# <a name="apidoc.module.openpgp.Keyring"></a>[module openpgp.Keyring](#apidoc.module.openpgp.Keyring)

#### <a name="apidoc.element.openpgp.Keyring.Keyring"></a>[function <span class="apidocSignatureSpan">openpgp.</span>Keyring (storeHandler)](#apidoc.element.openpgp.Keyring.Keyring)
- description and source-code
```javascript
function Keyring(storeHandler) {
  this.storeHandler = storeHandler || new _localstore2.default();
  this.publicKeys = new KeyArray(this.storeHandler.loadPublic());
  this.privateKeys = new KeyArray(this.storeHandler.loadPrivate());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.Keyring.localstore"></a>[function <span class="apidocSignatureSpan">openpgp.Keyring.</span>localstore (prefix)](#apidoc.element.openpgp.Keyring.localstore)
- description and source-code
```javascript
function LocalStore(prefix) {
  prefix = prefix || 'openpgp-';
  this.publicKeysItem = prefix + this.publicKeysItem;
  this.privateKeysItem = prefix + this.privateKeysItem;
  if (typeof window !== 'undefined' && window.localStorage) {
    this.storage = window.localStorage;
  } else {
    this.storage = new (_dereq_('node-localstorage').LocalStorage)(_config2.default.node_store);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.Keyring.localstore"></a>[module openpgp.Keyring.localstore](#apidoc.module.openpgp.Keyring.localstore)

#### <a name="apidoc.element.openpgp.Keyring.localstore.localstore"></a>[function <span class="apidocSignatureSpan">openpgp.Keyring.</span>localstore (prefix)](#apidoc.element.openpgp.Keyring.localstore.localstore)
- description and source-code
```javascript
function LocalStore(prefix) {
  prefix = prefix || 'openpgp-';
  this.publicKeysItem = prefix + this.publicKeysItem;
  this.privateKeysItem = prefix + this.privateKeysItem;
  if (typeof window !== 'undefined' && window.localStorage) {
    this.storage = window.localStorage;
  } else {
    this.storage = new (_dereq_('node-localstorage').LocalStorage)(_config2.default.node_store);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.Keyring.localstore.prototype"></a>[module openpgp.Keyring.localstore.prototype](#apidoc.module.openpgp.Keyring.localstore.prototype)

#### <a name="apidoc.element.openpgp.Keyring.localstore.prototype.loadPrivate"></a>[function <span class="apidocSignatureSpan">openpgp.Keyring.localstore.prototype.</span>loadPrivate ()](#apidoc.element.openpgp.Keyring.localstore.prototype.loadPrivate)
- description and source-code
```javascript
loadPrivate = function () {
  return loadKeys(this.storage, this.privateKeysItem);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.Keyring.localstore.prototype.loadPublic"></a>[function <span class="apidocSignatureSpan">openpgp.Keyring.localstore.prototype.</span>loadPublic ()](#apidoc.element.openpgp.Keyring.localstore.prototype.loadPublic)
- description and source-code
```javascript
loadPublic = function () {
  return loadKeys(this.storage, this.publicKeysItem);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.Keyring.localstore.prototype.storePrivate"></a>[function <span class="apidocSignatureSpan">openpgp.Keyring.localstore.prototype.</span>storePrivate (keys)](#apidoc.element.openpgp.Keyring.localstore.prototype.storePrivate)
- description and source-code
```javascript
storePrivate = function (keys) {
  storeKeys(this.storage, this.privateKeysItem, keys);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.Keyring.localstore.prototype.storePublic"></a>[function <span class="apidocSignatureSpan">openpgp.Keyring.localstore.prototype.</span>storePublic (keys)](#apidoc.element.openpgp.Keyring.localstore.prototype.storePublic)
- description and source-code
```javascript
storePublic = function (keys) {
  storeKeys(this.storage, this.publicKeysItem, keys);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.Keyring.prototype"></a>[module openpgp.Keyring.prototype](#apidoc.module.openpgp.Keyring.prototype)

#### <a name="apidoc.element.openpgp.Keyring.prototype.clear"></a>[function <span class="apidocSignatureSpan">openpgp.Keyring.prototype.</span>clear ()](#apidoc.element.openpgp.Keyring.prototype.clear)
- description and source-code
```javascript
clear = function () {
  this.publicKeys.keys = [];
  this.privateKeys.keys = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.Keyring.prototype.getAllKeys"></a>[function <span class="apidocSignatureSpan">openpgp.Keyring.prototype.</span>getAllKeys ()](#apidoc.element.openpgp.Keyring.prototype.getAllKeys)
- description and source-code
```javascript
getAllKeys = function () {
  return this.publicKeys.keys.concat(this.privateKeys.keys);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.Keyring.prototype.getKeysForId"></a>[function <span class="apidocSignatureSpan">openpgp.Keyring.prototype.</span>getKeysForId (keyId, deep)](#apidoc.element.openpgp.Keyring.prototype.getKeysForId)
- description and source-code
```javascript
getKeysForId = function (keyId, deep) {
  var result = [];
  result = result.concat(this.publicKeys.getForId(keyId, deep) || []);
  result = result.concat(this.privateKeys.getForId(keyId, deep) || []);
  return result.length ? result : null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.Keyring.prototype.removeKeysForId"></a>[function <span class="apidocSignatureSpan">openpgp.Keyring.prototype.</span>removeKeysForId (keyId)](#apidoc.element.openpgp.Keyring.prototype.removeKeysForId)
- description and source-code
```javascript
removeKeysForId = function (keyId) {
  var result = [];
  result = result.concat(this.publicKeys.removeForId(keyId) || []);
  result = result.concat(this.privateKeys.removeForId(keyId) || []);
  return result.length ? result : null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.Keyring.prototype.store"></a>[function <span class="apidocSignatureSpan">openpgp.Keyring.prototype.</span>store ()](#apidoc.element.openpgp.Keyring.prototype.store)
- description and source-code
```javascript
store = function () {
  this.storeHandler.storePublic(this.publicKeys.keys);
  this.storeHandler.storePrivate(this.privateKeys.keys);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.MPI"></a>[module openpgp.MPI](#apidoc.module.openpgp.MPI)

#### <a name="apidoc.element.openpgp.MPI.MPI"></a>[function <span class="apidocSignatureSpan">openpgp.</span>MPI ()](#apidoc.element.openpgp.MPI.MPI)
- description and source-code
```javascript
function MPI() {
<span class="apidocCodeCommentSpan">  /** An implementation dependent integer */
</span>  this.data = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.MPI.fromClone"></a>[function <span class="apidocSignatureSpan">openpgp.MPI.</span>fromClone (clone)](#apidoc.element.openpgp.MPI.fromClone)
- description and source-code
```javascript
fromClone = function (clone) {
  clone.data.copyTo = _jsbn2.default.prototype.copyTo;
  var bn = new _jsbn2.default();
  clone.data.copyTo(bn);
  var mpi = new MPI();
  mpi.data = bn;
  return mpi;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.MPI.prototype"></a>[module openpgp.MPI.prototype](#apidoc.module.openpgp.MPI.prototype)

#### <a name="apidoc.element.openpgp.MPI.prototype.byteLength"></a>[function <span class="apidocSignatureSpan">openpgp.MPI.prototype.</span>byteLength ()](#apidoc.element.openpgp.MPI.prototype.byteLength)
- description and source-code
```javascript
byteLength = function () {
  return this.toBytes().length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.MPI.prototype.fromBigInteger"></a>[function <span class="apidocSignatureSpan">openpgp.MPI.prototype.</span>fromBigInteger (bn)](#apidoc.element.openpgp.MPI.prototype.fromBigInteger)
- description and source-code
```javascript
fromBigInteger = function (bn) {
  this.data = bn.clone();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.MPI.prototype.fromBytes"></a>[function <span class="apidocSignatureSpan">openpgp.MPI.prototype.</span>fromBytes (bytes)](#apidoc.element.openpgp.MPI.prototype.fromBytes)
- description and source-code
```javascript
fromBytes = function (bytes) {
  this.data = new _jsbn2.default(_util2.default.hexstrdump(bytes), 16);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.MPI.prototype.read"></a>[function <span class="apidocSignatureSpan">openpgp.MPI.prototype.</span>read (bytes)](#apidoc.element.openpgp.MPI.prototype.read)
- description and source-code
```javascript
read = function (bytes) {

  if (typeof bytes === 'string' || String.prototype.isPrototypeOf(bytes)) {
    bytes = _util2.default.str2Uint8Array(bytes);
  }

  var bits = bytes[0] << 8 | bytes[1];

  // Additional rules:
  //
  //    The size of an MPI is ((MPI.length + 7) / 8) + 2 octets.
  //
  //    The length field of an MPI describes the length starting from its
  //    most significant non-zero bit.  Thus, the MPI [00 02 01] is not
  //    formed correctly.  It should be [00 01 01].

  // TODO: Verification of this size method! This size calculation as
  //      specified above is not applicable in JavaScript
  var bytelen = Math.ceil(bits / 8);

  var raw = _util2.default.Uint8Array2str(bytes.subarray(2, 2 + bytelen));
  this.fromBytes(raw);

  return 2 + bytelen;
}
```
- example usage
```shell
...
openpgp.encrypt(options).then(function(ciphertext) {
    encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
...
```

#### <a name="apidoc.element.openpgp.MPI.prototype.toBigInteger"></a>[function <span class="apidocSignatureSpan">openpgp.MPI.prototype.</span>toBigInteger ()](#apidoc.element.openpgp.MPI.prototype.toBigInteger)
- description and source-code
```javascript
toBigInteger = function () {
  return this.data.clone();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.MPI.prototype.toBytes"></a>[function <span class="apidocSignatureSpan">openpgp.MPI.prototype.</span>toBytes ()](#apidoc.element.openpgp.MPI.prototype.toBytes)
- description and source-code
```javascript
toBytes = function () {
  var bytes = _util2.default.Uint8Array2str(this.write());
  return bytes.substr(2);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.MPI.prototype.write"></a>[function <span class="apidocSignatureSpan">openpgp.MPI.prototype.</span>write ()](#apidoc.element.openpgp.MPI.prototype.write)
- description and source-code
```javascript
write = function () {
  return _util2.default.str2Uint8Array(this.data.toMPI());
}
```
- example usage
```shell
...
options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
password: 'secret stuff',                 // decrypt with password
...
```



# <a name="apidoc.module.openpgp.S2K"></a>[module openpgp.S2K](#apidoc.module.openpgp.S2K)

#### <a name="apidoc.element.openpgp.S2K.S2K"></a>[function <span class="apidocSignatureSpan">openpgp.</span>S2K ()](#apidoc.element.openpgp.S2K.S2K)
- description and source-code
```javascript
function S2K() {
<span class="apidocCodeCommentSpan">  /** @type {module:enums.hash} */
</span>  this.algorithm = 'sha256';
  /** @type {module:enums.s2k} */
  this.type = 'iterated';
  this.c = 96;
  /** Eight bytes of salt in a binary string.
   * @type {String}
   */
  this.salt = _crypto2.default.random.getRandomBytes(8);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.S2K.fromClone"></a>[function <span class="apidocSignatureSpan">openpgp.S2K.</span>fromClone (clone)](#apidoc.element.openpgp.S2K.fromClone)
- description and source-code
```javascript
fromClone = function (clone) {
  var s2k = new S2K();
  s2k.algorithm = clone.algorithm;
  s2k.type = clone.type;
  s2k.c = clone.c;
  s2k.salt = clone.salt;
  return s2k;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.S2K.prototype"></a>[module openpgp.S2K.prototype](#apidoc.module.openpgp.S2K.prototype)

#### <a name="apidoc.element.openpgp.S2K.prototype.get_count"></a>[function <span class="apidocSignatureSpan">openpgp.S2K.prototype.</span>get_count ()](#apidoc.element.openpgp.S2K.prototype.get_count)
- description and source-code
```javascript
get_count = function () {
  // Exponent bias, defined in RFC4880
  var expbias = 6;

  return 16 + (this.c & 15) << (this.c >> 4) + expbias;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.S2K.prototype.produce_key"></a>[function <span class="apidocSignatureSpan">openpgp.S2K.prototype.</span>produce_key (passphrase, numBytes)](#apidoc.element.openpgp.S2K.prototype.produce_key)
- description and source-code
```javascript
produce_key = function (passphrase, numBytes) {
  passphrase = _util2.default.str2Uint8Array(_util2.default.encode_utf8(passphrase));

  function round(prefix, s2k) {
    var algorithm = _enums2.default.write(_enums2.default.hash, s2k.algorithm);

    switch (s2k.type) {
      case 'simple':
        return _crypto2.default.hash.digest(algorithm, _util2.default.concatUint8Array([prefix, passphrase]));

      case 'salted':
        return _crypto2.default.hash.digest(algorithm, _util2.default.concatUint8Array([prefix, s2k.salt, passphrase]));

      case 'iterated':
        var isp = [],
            count = s2k.get_count(),
            data = _util2.default.concatUint8Array([s2k.salt, passphrase]);

        while (isp.length * data.length < count) {
          isp.push(data);
        }

        isp = _util2.default.concatUint8Array(isp);

        if (isp.length > count) {
          isp = isp.subarray(0, count);
        }

        return _crypto2.default.hash.digest(algorithm, _util2.default.concatUint8Array([prefix, isp]));

      case 'gnu':
        throw new Error("GNU s2k type not supported.");

      default:
        throw new Error("Unknown s2k type.");
    }
  }

  var arr = [],
      rlength = 0,
      prefix = new Uint8Array(numBytes);

  for (var i = 0; i < numBytes; i++) {
    prefix[i] = 0;
  }
  i = 0;

  while (rlength < numBytes) {
    var result = round(prefix.subarray(0, i), this);
    arr.push(result);
    rlength += result.length;
    i++;
  }

  return _util2.default.concatUint8Array(arr).subarray(0, numBytes);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.S2K.prototype.read"></a>[function <span class="apidocSignatureSpan">openpgp.S2K.prototype.</span>read (bytes)](#apidoc.element.openpgp.S2K.prototype.read)
- description and source-code
```javascript
read = function (bytes) {
  var i = 0;
  this.type = _enums2.default.read(_enums2.default.s2k, bytes[i++]);
  this.algorithm = _enums2.default.read(_enums2.default.hash, bytes[i++]);

  switch (this.type) {
    case 'simple':
      break;

    case 'salted':
      this.salt = bytes.subarray(i, i + 8);
      i += 8;
      break;

    case 'iterated':
      this.salt = bytes.subarray(i, i + 8);
      i += 8;

      // Octet 10: count, a one-octet, coded value
      this.c = bytes[i++];
      break;

    case 'gnu':
      if (_util2.default.Uint8Array2str(bytes.subarray(i, 3)) === "GNU") {
        i += 3; // GNU
        var gnuExtType = 1000 + bytes[i++];
        if (gnuExtType === 1001) {
          this.type = gnuExtType;
          // GnuPG extension mode 1001 -- don't write secret key at all
        } else {
          throw new Error("Unknown s2k gnu protection mode.");
        }
      } else {
        throw new Error("Unknown s2k type.");
      }
      break;

    default:
      throw new Error("Unknown s2k type.");
  }

  return i;
}
```
- example usage
```shell
...
openpgp.encrypt(options).then(function(ciphertext) {
    encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
...
```

#### <a name="apidoc.element.openpgp.S2K.prototype.write"></a>[function <span class="apidocSignatureSpan">openpgp.S2K.prototype.</span>write ()](#apidoc.element.openpgp.S2K.prototype.write)
- description and source-code
```javascript
write = function () {

  var arr = [new Uint8Array([_enums2.default.write(_enums2.default.s2k, this.type), _enums2.default.write(_enums2.default.hash,
this.algorithm)])];

  switch (this.type) {
    case 'simple':
      break;
    case 'salted':
      arr.push(this.salt);
      break;
    case 'iterated':
      arr.push(this.salt);
      arr.push(new Uint8Array([this.c]));
      break;
    case 'gnu':
      throw new Error("GNU s2k type not supported.");
    default:
      throw new Error("Unknown s2k type.");
  }

  return _util2.default.concatUint8Array(arr);
}
```
- example usage
```shell
...
options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
password: 'secret stuff',                 // decrypt with password
...
```



# <a name="apidoc.module.openpgp.armor"></a>[module openpgp.armor](#apidoc.module.openpgp.armor)

#### <a name="apidoc.element.openpgp.armor.decode"></a>[function <span class="apidocSignatureSpan">openpgp.armor.</span>decode (text)](#apidoc.element.openpgp.armor.decode)
- description and source-code
```javascript
function dearmor(text) {
  var reSplit = /^-----[^-]+-----$\n/m;

  // remove trailing whitespace at end of line
  text = text.replace(/[\t\r ]+\n/g, '\n');

  var type = getType(text);

  var splittext = text.split(reSplit);

  // IE has a bug in split with a re. If the pattern matches the beginning of the
  // string it doesn't create an empty array element 0. So we need to detect this
  // so we know the index of the data we are interested in.
  var indexBase = 1;

  var result, checksum, msg;

  if (text.search(reSplit) !== splittext[0].length) {
    indexBase = 0;
  }

  if (type !== 2) {
    msg = splitHeaders(splittext[indexBase]);
    var msg_sum = splitChecksum(msg.body);

    result = {
      data: _base2.default.decode(msg_sum.body),
      headers: msg.headers,
      type: type
    };

    checksum = msg_sum.checksum;
  } else {
    // Reverse dash-escaping for msg
    msg = splitHeaders(splittext[indexBase].replace(/^- /mg, ''));
    var sig = splitHeaders(splittext[indexBase + 1].replace(/^- /mg, ''));
    verifyHeaders(sig.headers);
    var sig_sum = splitChecksum(sig.body);

    result = {
      text: msg.body.replace(/\n$/, '').replace(/\n/g, "\r\n"),
      data: _base2.default.decode(sig_sum.body),
      headers: msg.headers,
      type: type
    };

    checksum = sig_sum.checksum;
  }

  checksum = checksum.substr(0, 4);

  if (!verifyCheckSum(result.data, checksum)) {
    throw new Error("Ascii armor integrity check on message failed: '" + checksum + "' should be '" + getCheckSum(result.data) + "'");
  }

  verifyHeaders(result.headers);

  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.armor.encode"></a>[function <span class="apidocSignatureSpan">openpgp.armor.</span>encode (messagetype, body, partindex, parttotal)](#apidoc.element.openpgp.armor.encode)
- description and source-code
```javascript
function armor(messagetype, body, partindex, parttotal) {
  var result = [];
  switch (messagetype) {
    case _enums2.default.armor.multipart_section:
      result.push("-----BEGIN PGP MESSAGE, PART " + partindex + "/" + parttotal + "-----\r\n");
      result.push(addheader());
      result.push(_base2.default.encode(body));
      result.push("\r\n=" + getCheckSum(body) + "\r\n");
      result.push("-----END PGP MESSAGE, PART " + partindex + "/" + parttotal + "-----\r\n");
      break;
    case _enums2.default.armor.multipart_last:
      result.push("-----BEGIN PGP MESSAGE, PART " + partindex + "-----\r\n");
      result.push(addheader());
      result.push(_base2.default.encode(body));
      result.push("\r\n=" + getCheckSum(body) + "\r\n");
      result.push("-----END PGP MESSAGE, PART " + partindex + "-----\r\n");
      break;
    case _enums2.default.armor.signed:
      result.push("\r\n-----BEGIN PGP SIGNED MESSAGE-----\r\n");
      result.push("Hash: " + body.hash + "\r\n\r\n");
      result.push(body.text.replace(/\n-/g, "\n- -"));
      result.push("\r\n-----BEGIN PGP SIGNATURE-----\r\n");
      result.push(addheader());
      result.push(_base2.default.encode(body.data));
      result.push("\r\n=" + getCheckSum(body.data) + "\r\n");
      result.push("-----END PGP SIGNATURE-----\r\n");
      break;
    case _enums2.default.armor.message:
      result.push("-----BEGIN PGP MESSAGE-----\r\n");
      result.push(addheader());
      result.push(_base2.default.encode(body));
      result.push("\r\n=" + getCheckSum(body) + "\r\n");
      result.push("-----END PGP MESSAGE-----\r\n");
      break;
    case _enums2.default.armor.public_key:
      result.push("-----BEGIN PGP PUBLIC KEY BLOCK-----\r\n");
      result.push(addheader());
      result.push(_base2.default.encode(body));
      result.push("\r\n=" + getCheckSum(body) + "\r\n");
      result.push("-----END PGP PUBLIC KEY BLOCK-----\r\n\r\n");
      break;
    case _enums2.default.armor.private_key:
      result.push("-----BEGIN PGP PRIVATE KEY BLOCK-----\r\n");
      result.push(addheader());
      result.push(_base2.default.encode(body));
      result.push("\r\n=" + getCheckSum(body) + "\r\n");
      result.push("-----END PGP PRIVATE KEY BLOCK-----\r\n");
      break;
    case _enums2.default.armor.signature:
      result.push("-----BEGIN PGP SIGNATURE-----\r\n");
      result.push(addheader());
      result.push(_base2.default.encode(body));
      result.push("\r\n=" + getCheckSum(body) + "\r\n");
      result.push("-----END PGP SIGNATURE-----\r\n");
      break;
  }

  return result.join('');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.cleartext"></a>[module openpgp.cleartext](#apidoc.module.openpgp.cleartext)

#### <a name="apidoc.element.openpgp.cleartext.CleartextMessage"></a>[function <span class="apidocSignatureSpan">openpgp.cleartext.</span>CleartextMessage (text, signature)](#apidoc.element.openpgp.cleartext.CleartextMessage)
- description and source-code
```javascript
function CleartextMessage(text, signature) {
  if (!(this instanceof CleartextMessage)) {
    return new CleartextMessage(text, signature);
  }
  // normalize EOL to canonical form <CR><LF>
  this.text = text.replace(/\r/g, '').replace(/[\t ]+\n/g, "\n").replace(/\n/g, "\r\n");
  if (signature && !(signature instanceof sigModule.Signature)) {
    throw new Error('Invalid signature input');
  }
  this.signature = signature || new sigModule.Signature(new _packet2.default.List());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.cleartext.readArmored"></a>[function <span class="apidocSignatureSpan">openpgp.cleartext.</span>readArmored (armoredText)](#apidoc.element.openpgp.cleartext.readArmored)
- description and source-code
```javascript
function readArmored(armoredText) {
  var input = _armor2.default.decode(armoredText);
  if (input.type !== _enums2.default.armor.signed) {
    throw new Error('No cleartext signed message.');
  }
  var packetlist = new _packet2.default.List();
  packetlist.read(input.data);
  verifyHeaders(input.headers, packetlist);
  var signature = new sigModule.Signature(packetlist);
  var newMessage = new CleartextMessage(input.text, signature);
  return newMessage;
}
```
- example usage
```shell
...
'''js
var options, encrypted;

var pubkey = '-----BEGIN PGP PUBLIC KEY BLOCK ... END PGP PUBLIC KEY BLOCK-----';
var privkey = '-----BEGIN PGP PRIVATE KEY BLOCK ... END PGP PRIVATE KEY BLOCK-----'; //encrypted private key
var passphrase = 'secret passphrase'; //what the privKey is encrypted with

var privKeyObj = openpgp.key.readArmored(privkey).keys[0];
privKeyObj.decrypt(passphrase);

options = {
    data: 'Hello, World!',                             // input as String (or Uint8Array)
    publicKeys: openpgp.key.readArmored(pubkey).keys,  // for encryption
    privateKeys: privKeyObj // for signing (optional)
};
...
```



# <a name="apidoc.module.openpgp.cleartext.CleartextMessage"></a>[module openpgp.cleartext.CleartextMessage](#apidoc.module.openpgp.cleartext.CleartextMessage)

#### <a name="apidoc.element.openpgp.cleartext.CleartextMessage.CleartextMessage"></a>[function <span class="apidocSignatureSpan">openpgp.cleartext.</span>CleartextMessage (text, signature)](#apidoc.element.openpgp.cleartext.CleartextMessage.CleartextMessage)
- description and source-code
```javascript
function CleartextMessage(text, signature) {
  if (!(this instanceof CleartextMessage)) {
    return new CleartextMessage(text, signature);
  }
  // normalize EOL to canonical form <CR><LF>
  this.text = text.replace(/\r/g, '').replace(/[\t ]+\n/g, "\n").replace(/\n/g, "\r\n");
  if (signature && !(signature instanceof sigModule.Signature)) {
    throw new Error('Invalid signature input');
  }
  this.signature = signature || new sigModule.Signature(new _packet2.default.List());
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.cleartext.CleartextMessage.prototype"></a>[module openpgp.cleartext.CleartextMessage.prototype](#apidoc.module.openpgp.cleartext.CleartextMessage.prototype)

#### <a name="apidoc.element.openpgp.cleartext.CleartextMessage.prototype.armor"></a>[function <span class="apidocSignatureSpan">openpgp.cleartext.CleartextMessage.prototype.</span>armor ()](#apidoc.element.openpgp.cleartext.CleartextMessage.prototype.armor)
- description and source-code
```javascript
armor = function () {
  var body = {
    hash: _enums2.default.read(_enums2.default.hash, _config2.default.prefer_hash_algorithm).toUpperCase(),
    text: this.text,
    data: this.signature.packets.write()
  };
  return _armor2.default.encode(_enums2.default.armor.signed, body);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.cleartext.CleartextMessage.prototype.getSigningKeyIds"></a>[function <span class="apidocSignatureSpan">openpgp.cleartext.CleartextMessage.prototype.</span>getSigningKeyIds ()](#apidoc.element.openpgp.cleartext.CleartextMessage.prototype.getSigningKeyIds)
- description and source-code
```javascript
getSigningKeyIds = function () {
  var keyIds = [];
  var signatureList = this.signature.packets;
  signatureList.forEach(function (packet) {
    keyIds.push(packet.issuerKeyId);
  });
  return keyIds;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.cleartext.CleartextMessage.prototype.getText"></a>[function <span class="apidocSignatureSpan">openpgp.cleartext.CleartextMessage.prototype.</span>getText ()](#apidoc.element.openpgp.cleartext.CleartextMessage.prototype.getText)
- description and source-code
```javascript
getText = function () {
  // normalize end of line to \n
  return this.text.replace(/\r\n/g, "\n");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.cleartext.CleartextMessage.prototype.sign"></a>[function <span class="apidocSignatureSpan">openpgp.cleartext.CleartextMessage.prototype.</span>sign (privateKeys)](#apidoc.element.openpgp.cleartext.CleartextMessage.prototype.sign)
- description and source-code
```javascript
sign = function (privateKeys) {
  this.signature = this.signDetached(privateKeys);
}
```
- example usage
```shell
...

'''js
options = {
data: 'Hello, World!',                             // input as String (or Uint8Array)
privateKeys: privKeyObj // for signing
};

openpgp.sign(options).then(function(signed) {
cleartext = signed.data; // '-----BEGIN PGP SIGNED MESSAGE ... END PGP SIGNATURE-----'
});
'''

'''js
options = {
message: openpgp.cleartext.readArmored(cleartext), // parse armored message
...
```

#### <a name="apidoc.element.openpgp.cleartext.CleartextMessage.prototype.signDetached"></a>[function <span class="apidocSignatureSpan">openpgp.cleartext.CleartextMessage.prototype.</span>signDetached (privateKeys)](#apidoc.element.openpgp.cleartext.CleartextMessage.prototype.signDetached)
- description and source-code
```javascript
signDetached = function (privateKeys) {
  var packetlist = new _packet2.default.List();
  var literalDataPacket = new _packet2.default.Literal();
  literalDataPacket.setText(this.text);
  for (var i = 0; i < privateKeys.length; i++) {
    if (privateKeys[i].isPublic()) {
      throw new Error('Need private key for signing');
    }
    var signaturePacket = new _packet2.default.Signature();
    signaturePacket.signatureType = _enums2.default.signature.text;
    signaturePacket.hashAlgorithm = _config2.default.prefer_hash_algorithm;
    var signingKeyPacket = privateKeys[i].getSigningKeyPacket();
    signaturePacket.publicKeyAlgorithm = signingKeyPacket.algorithm;
    if (!signingKeyPacket.isDecrypted) {
      throw new Error('Private key is not decrypted.');
    }
    signaturePacket.sign(signingKeyPacket, literalDataPacket);
    packetlist.push(signaturePacket);
  }
  return new sigModule.Signature(packetlist);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.cleartext.CleartextMessage.prototype.verify"></a>[function <span class="apidocSignatureSpan">openpgp.cleartext.CleartextMessage.prototype.</span>verify (keys)](#apidoc.element.openpgp.cleartext.CleartextMessage.prototype.verify)
- description and source-code
```javascript
verify = function (keys) {
  return this.verifyDetached(this.signature, keys);
}
```
- example usage
```shell
...

'''js
options = {
    message: openpgp.cleartext.readArmored(cleartext), // parse armored message
    publicKeys: openpgp.key.readArmored(pubkey).keys   // for verification
};

openpgp.verify(options).then(function(verified) {
	validity = verified.signatures[0].valid; // true
	if (validity) {
		console.log('signed by key id ' + verified.signatures[0].keyid.toHex());
	}
});
'''
...
```

#### <a name="apidoc.element.openpgp.cleartext.CleartextMessage.prototype.verifyDetached"></a>[function <span class="apidocSignatureSpan">openpgp.cleartext.CleartextMessage.prototype.</span>verifyDetached (signature, keys)](#apidoc.element.openpgp.cleartext.CleartextMessage.prototype.verifyDetached)
- description and source-code
```javascript
verifyDetached = function (signature, keys) {
  var result = [];
  var signatureList = signature.packets;
  var literalDataPacket = new _packet2.default.Literal();
  // we assume that cleartext signature is generated based on UTF8 cleartext
  literalDataPacket.setText(this.text);
  for (var i = 0; i < signatureList.length; i++) {
    var keyPacket = null;
    for (var j = 0; j < keys.length; j++) {
      keyPacket = keys[j].getSigningKeyPacket(signatureList[i].issuerKeyId);
      if (keyPacket) {
        break;
      }
    }

    var verifiedSig = {};
    if (keyPacket) {
      verifiedSig.keyid = signatureList[i].issuerKeyId;
      verifiedSig.valid = signatureList[i].verify(keyPacket, literalDataPacket);
    } else {
      verifiedSig.keyid = signatureList[i].issuerKeyId;
      verifiedSig.valid = null;
    }
    verifiedSig.signature = new sigModule.Signature([signatureList[i]]);

    result.push(verifiedSig);
  }
  return result;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.crypto"></a>[module openpgp.crypto](#apidoc.module.openpgp.crypto)

#### <a name="apidoc.element.openpgp.crypto.generateMpi"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.</span>generateMpi (algo, bits)](#apidoc.element.openpgp.crypto.generateMpi)
- description and source-code
```javascript
function generateMpi(algo, bits) {
  switch (algo) {
    case 'rsa_encrypt':
    case 'rsa_encrypt_sign':
    case 'rsa_sign':
      //remember "publicKey" refers to the crypto/public_key dir
      var rsa = new _public_key2.default.rsa();
      return rsa.generate(bits, "10001").then(function (keyObject) {
        var output = [];
        output.push(keyObject.n);
        output.push(keyObject.ee);
        output.push(keyObject.d);
        output.push(keyObject.p);
        output.push(keyObject.q);
        output.push(keyObject.u);
        return mapResult(output);
      });
    default:
      throw new Error('Unsupported algorithm for key generation.');
  }

  function mapResult(result) {
    return result.map(function (bn) {
      var mpi = new _mpi2.default();
      mpi.fromBigInteger(bn);
      return mpi;
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.generateSessionKey"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.</span>generateSessionKey (algo)](#apidoc.element.openpgp.crypto.generateSessionKey)
- description and source-code
```javascript
function generateSessionKey(algo) {
  return _random2.default.getRandomBytes(_cipher2.default[algo].keySize);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.getPrefixRandom"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.</span>getPrefixRandom (algo)](#apidoc.element.openpgp.crypto.getPrefixRandom)
- description and source-code
```javascript
function getPrefixRandom(algo) {
  return _random2.default.getRandomBytes(_cipher2.default[algo].blockSize);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.getPrivateMpiCount"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.</span>getPrivateMpiCount (algo)](#apidoc.element.openpgp.crypto.getPrivateMpiCount)
- description and source-code
```javascript
function getPrivateMpiCount(algo) {
  switch (algo) {
    case 'rsa_encrypt':
    case 'rsa_encrypt_sign':
    case 'rsa_sign':
      //   Algorithm-Specific Fields for RSA secret keys:
      //   - multiprecision integer (MPI) of RSA secret exponent d.
      //   - MPI of RSA secret prime value p.
      //   - MPI of RSA secret prime value q (p < q).
      //   - MPI of u, the multiplicative inverse of p, mod q.
      return 4;
    case 'elgamal':
      // Algorithm-Specific Fields for Elgamal secret keys:
      //   - MPI of Elgamal secret exponent x.
      return 1;
    case 'dsa':
      // Algorithm-Specific Fields for DSA secret keys:
      //   - MPI of DSA secret exponent x.
      return 1;
    default:
      throw new Error('Unknown algorithm');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.getPublicMpiCount"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.</span>getPublicMpiCount (algo)](#apidoc.element.openpgp.crypto.getPublicMpiCount)
- description and source-code
```javascript
function getPublicMpiCount(algo) {
  // - A series of multiprecision integers comprising the key material:
  //   Algorithm-Specific Fields for RSA public keys:
  //       - a multiprecision integer (MPI) of RSA public modulus n;
  //       - an MPI of RSA public encryption exponent e.
  switch (algo) {
    case 'rsa_encrypt':
    case 'rsa_encrypt_sign':
    case 'rsa_sign':
      return 2;

    //   Algorithm-Specific Fields for Elgamal public keys:
    //     - MPI of Elgamal prime p;
    //     - MPI of Elgamal group generator g;
    //     - MPI of Elgamal public key value y (= g**x mod p where x  is secret).
    case 'elgamal':
      return 3;

    //   Algorithm-Specific Fields for DSA public keys:
    //       - MPI of DSA prime p;
    //       - MPI of DSA group order q (q is a prime divisor of p-1);
    //       - MPI of DSA group generator g;
    //       - MPI of DSA public-key value y (= g**x mod p where x  is secret).
    case 'dsa':
      return 4;

    default:
      throw new Error('Unknown algorithm.');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.publicKeyDecrypt"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.</span>publicKeyDecrypt (algo, keyIntegers, dataIntegers)](#apidoc.element.openpgp.crypto.publicKeyDecrypt)
- description and source-code
```javascript
function publicKeyDecrypt(algo, keyIntegers, dataIntegers) {
  var p;

  var bn = function () {
    switch (algo) {
      case 'rsa_encrypt_sign':
      case 'rsa_encrypt':
        var rsa = new _public_key2.default.rsa();
        // 0 and 1 are the public key.
        var n = keyIntegers[0].toBigInteger();
        var e = keyIntegers[1].toBigInteger();
        // 2 to 5 are the private key.
        var d = keyIntegers[2].toBigInteger();
        p = keyIntegers[3].toBigInteger();
        var q = keyIntegers[4].toBigInteger();
        var u = keyIntegers[5].toBigInteger();
        var m = dataIntegers[0].toBigInteger();
        return rsa.decrypt(m, n, e, d, p, q, u);
      case 'elgamal':
        var elgamal = new _public_key2.default.elgamal();
        var x = keyIntegers[3].toBigInteger();
        var c1 = dataIntegers[0].toBigInteger();
        var c2 = dataIntegers[1].toBigInteger();
        p = keyIntegers[0].toBigInteger();
        return elgamal.decrypt(c1, c2, p, x);
      default:
        return null;
    }
  }();

  var result = new _mpi2.default();
  result.fromBigInteger(bn);
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.publicKeyEncrypt"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.</span>publicKeyEncrypt (algo, publicMPIs, data)](#apidoc.element.openpgp.crypto.publicKeyEncrypt)
- description and source-code
```javascript
function publicKeyEncrypt(algo, publicMPIs, data) {
  var result = function () {
    var m;
    switch (algo) {
      case 'rsa_encrypt':
      case 'rsa_encrypt_sign':
        var rsa = new _public_key2.default.rsa();
        var n = publicMPIs[0].toBigInteger();
        var e = publicMPIs[1].toBigInteger();
        m = data.toBigInteger();
        return [rsa.encrypt(m, e, n)];

      case 'elgamal':
        var elgamal = new _public_key2.default.elgamal();
        var p = publicMPIs[0].toBigInteger();
        var g = publicMPIs[1].toBigInteger();
        var y = publicMPIs[2].toBigInteger();
        m = data.toBigInteger();
        return elgamal.encrypt(m, g, p, y);

      default:
        return [];
    }
  }();

  return result.map(function (bn) {
    var mpi = new _mpi2.default();
    mpi.fromBigInteger(bn);
    return mpi;
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.crypto.cfb"></a>[module openpgp.crypto.cfb](#apidoc.module.openpgp.crypto.cfb)

#### <a name="apidoc.element.openpgp.crypto.cfb.decrypt"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.cfb.</span>decrypt (cipherfn, key, ciphertext, resync)](#apidoc.element.openpgp.crypto.cfb.decrypt)
- description and source-code
```javascript
function decrypt(cipherfn, key, ciphertext, resync) {
  cipherfn = new _cipher2.default[cipherfn](key);
  var block_size = cipherfn.blockSize;

  var iblock = new Uint8Array(block_size);
  var ablock = new Uint8Array(block_size);

  var i, j, n;
  var text = new Uint8Array(ciphertext.length - block_size);

  // initialisation vector
  for (i = 0; i < block_size; i++) {
    iblock[i] = 0;
  }

  iblock = cipherfn.encrypt(iblock);
  for (i = 0; i < block_size; i++) {
    ablock[i] = ciphertext[i];
    iblock[i] ^= ablock[i];
  }

  ablock = cipherfn.encrypt(ablock);

  // test check octets
  if (iblock[block_size - 2] !== (ablock[0] ^ ciphertext[block_size]) || iblock[block_size - 1] !== (ablock[1] ^ ciphertext[block_size
 + 1])) {
    throw new Error('CFB decrypt: invalid key');
  }

<span class="apidocCodeCommentSpan">  /*  RFC4880: Tag 18 and Resync:
   *  [...] Unlike the Symmetrically Encrypted Data Packet, no
   *  special CFB resynchronization is done after encrypting this prefix
   *  data.  See "OpenPGP CFB Mode" below for more details.
    */
</span>
  j = 0;
  if (resync) {
    for (i = 0; i < block_size; i++) {
      iblock[i] = ciphertext[i + 2];
    }
    for (n = block_size + 2; n < ciphertext.length; n += block_size) {
      ablock = cipherfn.encrypt(iblock);

      for (i = 0; i < block_size && i + n < ciphertext.length; i++) {
        iblock[i] = ciphertext[n + i];
        if (j < text.length) {
          text[j] = ablock[i] ^ iblock[i];
          j++;
        }
      }
    }
  } else {
    for (i = 0; i < block_size; i++) {
      iblock[i] = ciphertext[i];
    }
    for (n = block_size; n < ciphertext.length; n += block_size) {
      ablock = cipherfn.encrypt(iblock);
      for (i = 0; i < block_size && i + n < ciphertext.length; i++) {
        iblock[i] = ciphertext[n + i];
        if (j < text.length) {
          text[j] = ablock[i] ^ iblock[i];
          j++;
        }
      }
    }
  }

  n = resync ? 0 : 2;

  text = text.subarray(n, ciphertext.length - block_size - 2 + n);

  return text;
}
```
- example usage
```shell
...
'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
'''

#### Encrypt and decrypt *String* data with PGP keys

'''js
...
```

#### <a name="apidoc.element.openpgp.crypto.cfb.encrypt"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.cfb.</span>encrypt (prefixrandom, cipherfn, plaintext, key, resync)](#apidoc.element.openpgp.crypto.cfb.encrypt)
- description and source-code
```javascript
function encrypt(prefixrandom, cipherfn, plaintext, key, resync) {
  cipherfn = new _cipher2.default[cipherfn](key);
  var block_size = cipherfn.blockSize;

  var FR = new Uint8Array(block_size);
  var FRE = new Uint8Array(block_size);

  var new_prefix = new Uint8Array(prefixrandom.length + 2);
  new_prefix.set(prefixrandom);
  new_prefix[prefixrandom.length] = prefixrandom[block_size - 2];
  new_prefix[prefixrandom.length + 1] = prefixrandom[block_size - 1];
  prefixrandom = new_prefix;

  var ciphertext = new Uint8Array(plaintext.length + 2 + block_size * 2);
  var i, n, begin;
  var offset = resync ? 0 : 2;

  // 1.  The feedback register (FR) is set to the IV, which is all zeros.
  for (i = 0; i < block_size; i++) {
    FR[i] = 0;
  }

  // 2.  FR is encrypted to produce FRE (FR Encrypted).  This is the
  //     encryption of an all-zero value.
  FRE = cipherfn.encrypt(FR);
  // 3.  FRE is xored with the first BS octets of random data prefixed to
  //     the plaintext to produce C[1] through C[BS], the first BS octets
  //     of ciphertext.
  for (i = 0; i < block_size; i++) {
    ciphertext[i] = FRE[i] ^ prefixrandom[i];
  }

  // 4.  FR is loaded with C[1] through C[BS].
  FR.set(ciphertext.subarray(0, block_size));

  // 5.  FR is encrypted to produce FRE, the encryption of the first BS
  //     octets of ciphertext.
  FRE = cipherfn.encrypt(FR);

  // 6.  The left two octets of FRE get xored with the next two octets of
  //     data that were prefixed to the plaintext.  This produces C[BS+1]
  //     and C[BS+2], the next two octets of ciphertext.
  ciphertext[block_size] = FRE[0] ^ prefixrandom[block_size];
  ciphertext[block_size + 1] = FRE[1] ^ prefixrandom[block_size + 1];

  if (resync) {
    // 7.  (The resync step) FR is loaded with C[3] through C[BS+2].
    FR.set(ciphertext.subarray(2, block_size + 2));
  } else {
    FR.set(ciphertext.subarray(0, block_size));
  }
  // 8.  FR is encrypted to produce FRE.
  FRE = cipherfn.encrypt(FR);

  // 9.  FRE is xored with the first BS octets of the given plaintext, now
  //     that we have finished encrypting the BS+2 octets of prefixed
  //     data.  This produces C[BS+3] through C[BS+(BS+2)], the next BS
  //     octets of ciphertext.
  for (i = 0; i < block_size; i++) {
    ciphertext[block_size + 2 + i] = FRE[i + offset] ^ plaintext[i];
  }
  for (n = block_size; n < plaintext.length + offset; n += block_size) {
    // 10. FR is loaded with C[BS+3] to C[BS + (BS+2)] (which is C11-C18 for
    // an 8-octet block).
    begin = n + 2 - offset;
    FR.set(ciphertext.subarray(begin, begin + block_size));

    // 11. FR is encrypted to produce FRE.
    FRE = cipherfn.encrypt(FR);

    // 12. FRE is xored with the next BS octets of plaintext, to produce
    // the next BS octets of ciphertext.  These are loaded into FR, and
    // the process is repeated until the plaintext is used up.
    for (i = 0; i < block_size; i++) {
      ciphertext[block_size + begin + i] = FRE[i] ^ plaintext[n + i - offset];
    }
  }

  ciphertext = ciphertext.subarray(0, plaintext.length + 2 + block_size);
  return ciphertext;
}
```
- example usage
```shell
...

options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
...
```

#### <a name="apidoc.element.openpgp.crypto.cfb.mdc"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.cfb.</span>mdc (cipherfn, key, ciphertext)](#apidoc.element.openpgp.crypto.cfb.mdc)
- description and source-code
```javascript
function mdc(cipherfn, key, ciphertext) {
  cipherfn = new _cipher2.default[cipherfn](key);
  var block_size = cipherfn.blockSize;

  var iblock = new Uint8Array(block_size);
  var ablock = new Uint8Array(block_size);
  var i;

  // initialisation vector
  for (i = 0; i < block_size; i++) {
    iblock[i] = 0;
  }

  iblock = cipherfn.encrypt(iblock);
  for (i = 0; i < block_size; i++) {
    ablock[i] = ciphertext[i];
    iblock[i] ^= ablock[i];
  }

  ablock = cipherfn.encrypt(ablock);

  var result = new Uint8Array(iblock.length + 2);
  result.set(iblock);
  result[iblock.length] = ablock[0] ^ ciphertext[block_size];
  result[iblock.length + 1] = ablock[1] ^ ciphertext[block_size + 1];
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.cfb.normalDecrypt"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.cfb.</span>normalDecrypt (cipherfn, key, ciphertext, iv)](#apidoc.element.openpgp.crypto.cfb.normalDecrypt)
- description and source-code
```javascript
function normalDecrypt(cipherfn, key, ciphertext, iv) {
  cipherfn = new _cipher2.default[cipherfn](key);
  var block_size = cipherfn.blockSize;

  var blockp;
  var pos = 0;
  var plaintext = new Uint8Array(ciphertext.length);
  var offset = 0;
  var i,
      j = 0;

  if (iv === null) {
    blockp = new Uint8Array(block_size);
    for (i = 0; i < block_size; i++) {
      blockp[i] = 0;
    }
  } else {
    blockp = iv.subarray(0, block_size);
  }
  while (ciphertext.length > block_size * pos) {
    var decblock = cipherfn.encrypt(blockp);
    blockp = ciphertext.subarray(pos * block_size + offset, pos * block_size + block_size + offset);
    for (i = 0; i < blockp.length; i++) {
      plaintext[j++] = blockp[i] ^ decblock[i];
    }
    pos++;
  }

  return plaintext;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.cfb.normalEncrypt"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.cfb.</span>normalEncrypt (cipherfn, key, plaintext, iv)](#apidoc.element.openpgp.crypto.cfb.normalEncrypt)
- description and source-code
```javascript
function normalEncrypt(cipherfn, key, plaintext, iv) {
  cipherfn = new _cipher2.default[cipherfn](key);
  var block_size = cipherfn.blockSize;

  var blocki = new Uint8Array(block_size);
  var blockc = new Uint8Array(block_size);
  var pos = 0;
  var cyphertext = new Uint8Array(plaintext.length);
  var i,
      j = 0;

  if (iv === null) {
    for (i = 0; i < block_size; i++) {
      blockc[i] = 0;
    }
  } else {
    for (i = 0; i < block_size; i++) {
      blockc[i] = iv[i];
    }
  }
  while (plaintext.length > block_size * pos) {
    var encblock = cipherfn.encrypt(blockc);
    blocki = plaintext.subarray(pos * block_size, pos * block_size + block_size);
    for (i = 0; i < blocki.length; i++) {
      blockc[i] = blocki[i] ^ encblock[i];
      cyphertext[j++] = blockc[i];
    }
    pos++;
  }
  return cyphertext;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.crypto.cipher"></a>[module openpgp.crypto.cipher](#apidoc.module.openpgp.crypto.cipher)

#### <a name="apidoc.element.openpgp.crypto.cipher.aes128"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.cipher.</span>aes128 (key)](#apidoc.element.openpgp.crypto.cipher.aes128)
- description and source-code
```javascript
function c(key) {
  this.key = keyExpansion(key);
  this._temp = new Uint32Array(this.blockSize / 4);

  this.encrypt = function (block) {
    return AESencrypt(block, this.key, this._temp);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.cipher.aes192"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.cipher.</span>aes192 (key)](#apidoc.element.openpgp.crypto.cipher.aes192)
- description and source-code
```javascript
function c(key) {
  this.key = keyExpansion(key);
  this._temp = new Uint32Array(this.blockSize / 4);

  this.encrypt = function (block) {
    return AESencrypt(block, this.key, this._temp);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.cipher.aes256"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.cipher.</span>aes256 (key)](#apidoc.element.openpgp.crypto.cipher.aes256)
- description and source-code
```javascript
function c(key) {
  this.key = keyExpansion(key);
  this._temp = new Uint32Array(this.blockSize / 4);

  this.encrypt = function (block) {
    return AESencrypt(block, this.key, this._temp);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.cipher.blowfish"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.cipher.</span>blowfish (key)](#apidoc.element.openpgp.crypto.cipher.blowfish)
- description and source-code
```javascript
function BF(key) {
  this.bf = new Blowfish();
  this.bf.init(key);

  this.encrypt = function (block) {
    return this.bf.encrypt_block(block);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.cipher.cast5"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.cipher.</span>cast5 (key)](#apidoc.element.openpgp.crypto.cipher.cast5)
- description and source-code
```javascript
function Cast5(key) {
  this.cast5 = new OpenpgpSymencCast5();
  this.cast5.setKey(key);

  this.encrypt = function (block) {
    return this.cast5.encrypt(block);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.cipher.des"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.cipher.</span>des (key)](#apidoc.element.openpgp.crypto.cipher.des)
- description and source-code
```javascript
function OriginalDes(key) {
  this.key = key;

  this.encrypt = function (block, padding) {
    var keys = des_createKeys(this.key);
    return des(keys, block, true, 0, null, padding);
  };

  this.decrypt = function (block, padding) {
    var keys = des_createKeys(this.key);
    return des(keys, block, false, 0, null, padding);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.cipher.idea"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.cipher.</span>idea ()](#apidoc.element.openpgp.crypto.cipher.idea)
- description and source-code
```javascript
function idea() {
  throw new Error('IDEA symmetric-key algorithm not implemented');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.cipher.tripledes"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.cipher.</span>tripledes (key)](#apidoc.element.openpgp.crypto.cipher.tripledes)
- description and source-code
```javascript
function Des(key) {
  this.key = [];

  for (var i = 0; i < 3; i++) {
    this.key.push(new Uint8Array(key.subarray(i * 8, i * 8 + 8)));
  }

  this.encrypt = function (block) {
    return des(des_createKeys(this.key[2]), des(des_createKeys(this.key[1]), des(des_createKeys(this.key[0]), block, true, 0, null
, null), false, 0, null, null), true, 0, null, null);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.cipher.twofish"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.cipher.</span>twofish (key)](#apidoc.element.openpgp.crypto.cipher.twofish)
- description and source-code
```javascript
function TF(key) {
  this.tf = createTwofish();
  this.tf.open(toArray(key), 0);

  this.encrypt = function (block) {
    return this.tf.encrypt(toArray(block), 0);
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.crypto.gcm"></a>[module openpgp.crypto.gcm](#apidoc.module.openpgp.crypto.gcm)

#### <a name="apidoc.element.openpgp.crypto.gcm.decrypt"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.gcm.</span>decrypt (cipher, ciphertext, key, iv)](#apidoc.element.openpgp.crypto.gcm.decrypt)
- description and source-code
```javascript
function decrypt(cipher, ciphertext, key, iv) {
  if (cipher.substr(0, 3) !== 'aes') {
    return Promise.reject(new Error('GCM mode supports only AES cipher'));
  }

  if (webCrypto && _config2.default.use_native && key.length !== 24) {
    // WebCrypto (no 192 bit support) see: https://www.chromium.org/blink/webcrypto#TOC-AES-support
    return webDecrypt(ciphertext, key, iv);
  } else if (nodeCrypto && _config2.default.use_native) {
    // Node crypto library
    return nodeDecrypt(ciphertext, key, iv);
  } else {
    // asm.js fallback
    return Promise.resolve(_asmcryptoLite2.default.AES_GCM.decrypt(ciphertext, key, iv));
  }
}
```
- example usage
```shell
...
'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
'''

#### Encrypt and decrypt *String* data with PGP keys

'''js
...
```

#### <a name="apidoc.element.openpgp.crypto.gcm.encrypt"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.gcm.</span>encrypt (cipher, plaintext, key, iv)](#apidoc.element.openpgp.crypto.gcm.encrypt)
- description and source-code
```javascript
function encrypt(cipher, plaintext, key, iv) {
  if (cipher.substr(0, 3) !== 'aes') {
    return Promise.reject(new Error('GCM mode supports only AES cipher'));
  }

  if (webCrypto && _config2.default.use_native && key.length !== 24) {
    // WebCrypto (no 192 bit support) see: https://www.chromium.org/blink/webcrypto#TOC-AES-support
    return webEncrypt(plaintext, key, iv);
  } else if (nodeCrypto && _config2.default.use_native) {
    // Node crypto library
    return nodeEncrypt(plaintext, key, iv);
  } else {
    // asm.js fallback
    return Promise.resolve(_asmcryptoLite2.default.AES_GCM.encrypt(plaintext, key, iv));
  }
}
```
- example usage
```shell
...

options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
...
```



# <a name="apidoc.module.openpgp.crypto.hash"></a>[module openpgp.crypto.hash](#apidoc.module.openpgp.crypto.hash)

#### <a name="apidoc.element.openpgp.crypto.hash.digest"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.hash.</span>digest (algo, data)](#apidoc.element.openpgp.crypto.hash.digest)
- description and source-code
```javascript
function digest(algo, data) {
  switch (algo) {
    case 1:
      // - MD5 [HAC]
      return this.md5(data);
    case 2:
      // - SHA-1 [FIPS180]
      return this.sha1(data);
    case 3:
      // - RIPE-MD/160 [HAC]
      return this.ripemd(data);
    case 8:
      // - SHA256 [FIPS180]
      return this.sha256(data);
    case 9:
      // - SHA384 [FIPS180]
      return this.sha384(data);
    case 10:
      // - SHA512 [FIPS180]
      return this.sha512(data);
    case 11:
      // - SHA224 [FIPS180]
      return this.sha224(data);
    default:
      throw new Error('Invalid hash function.');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.hash.getHashByteLength"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.hash.</span>getHashByteLength (algo)](#apidoc.element.openpgp.crypto.hash.getHashByteLength)
- description and source-code
```javascript
function getHashByteLength(algo) {
  switch (algo) {
    case 1:
      // - MD5 [HAC]
      return 16;
    case 2:
    // - SHA-1 [FIPS180]
    case 3:
      // - RIPE-MD/160 [HAC]
      return 20;
    case 8:
      // - SHA256 [FIPS180]
      return 32;
    case 9:
      // - SHA384 [FIPS180]
      return 48;
    case 10:
      // - SHA512 [FIPS180]
      return 64;
    case 11:
      // - SHA224 [FIPS180]
      return 28;
    default:
      throw new Error('Invalid hash algorithm.');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.hash.md5"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.hash.</span>md5 (data)](#apidoc.element.openpgp.crypto.hash.md5)
- description and source-code
```javascript
md5 = function (data) {
  var shasum = nodeCrypto.createHash(type);
  shasum.update(new Buffer(data));
  return new Uint8Array(shasum.digest());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.hash.ripemd"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.hash.</span>ripemd (data)](#apidoc.element.openpgp.crypto.hash.ripemd)
- description and source-code
```javascript
ripemd = function (data) {
  var shasum = nodeCrypto.createHash(type);
  shasum.update(new Buffer(data));
  return new Uint8Array(shasum.digest());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.hash.sha1"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.hash.</span>sha1 (data)](#apidoc.element.openpgp.crypto.hash.sha1)
- description and source-code
```javascript
sha1 = function (data) {
  var shasum = nodeCrypto.createHash(type);
  shasum.update(new Buffer(data));
  return new Uint8Array(shasum.digest());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.hash.sha224"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.hash.</span>sha224 (data)](#apidoc.element.openpgp.crypto.hash.sha224)
- description and source-code
```javascript
sha224 = function (data) {
  var shasum = nodeCrypto.createHash(type);
  shasum.update(new Buffer(data));
  return new Uint8Array(shasum.digest());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.hash.sha256"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.hash.</span>sha256 (data)](#apidoc.element.openpgp.crypto.hash.sha256)
- description and source-code
```javascript
sha256 = function (data) {
  var shasum = nodeCrypto.createHash(type);
  shasum.update(new Buffer(data));
  return new Uint8Array(shasum.digest());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.hash.sha384"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.hash.</span>sha384 (data)](#apidoc.element.openpgp.crypto.hash.sha384)
- description and source-code
```javascript
sha384 = function (data) {
  var shasum = nodeCrypto.createHash(type);
  shasum.update(new Buffer(data));
  return new Uint8Array(shasum.digest());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.hash.sha512"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.hash.</span>sha512 (data)](#apidoc.element.openpgp.crypto.hash.sha512)
- description and source-code
```javascript
sha512 = function (data) {
  var shasum = nodeCrypto.createHash(type);
  shasum.update(new Buffer(data));
  return new Uint8Array(shasum.digest());
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.crypto.publicKey"></a>[module openpgp.crypto.publicKey](#apidoc.module.openpgp.crypto.publicKey)

#### <a name="apidoc.element.openpgp.crypto.publicKey.dsa"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.publicKey.</span>dsa ()](#apidoc.element.openpgp.crypto.publicKey.dsa)
- description and source-code
```javascript
function DSA() {
  // s1 = ((g**s) mod p) mod q
  // s1 = ((s**-1)*(sha-1(m)+(s1*x) mod q)
  function sign(hashalgo, m, g, p, q, x) {
    // If the output size of the chosen hash is larger than the number of
    // bits of q, the hash result is truncated to fit by taking the number
    // of leftmost bits equal to the number of bits of q.  This (possibly
    // truncated) hash function result is treated as a number and used
    // directly in the DSA signature algorithm.
    var hashed_data = _util2.default.getLeftNBits(_util2.default.Uint8Array2str(_hash2.default.digest(hashalgo, _util2.default.str2Uint8Array
(m))), q.bitLength());
    var hash = new _jsbn2.default(_util2.default.hexstrdump(hashed_data), 16);
    // FIPS-186-4, section 4.6:
    // The values of r and s shall be checked to determine if r = 0 or s = 0.
    // If either r = 0 or s = 0, a new value of k shall be generated, and the
    // signature shall be recalculated. It is extremely unlikely that r = 0
    // or s = 0 if signatures are generated properly.
    var k, s1, s2;
    while (true) {
      k = _random2.default.getRandomBigIntegerInRange(_jsbn2.default.ONE, q.subtract(_jsbn2.default.ONE));
      s1 = g.modPow(k, p).mod(q);
      s2 = k.modInverse(q).multiply(hash.add(x.multiply(s1))).mod(q);
      if (s1 !== 0 && s2 !== 0) {
        break;
      }
    }
    var result = [];
    result[0] = s1.toMPI();
    result[1] = s2.toMPI();
    return result;
  }

  function select_hash_algorithm(q) {
    var usersetting = _config2.default.prefer_hash_algorithm;
<span class="apidocCodeCommentSpan">    /*
     * 1024-bit key, 160-bit q, SHA-1, SHA-224, SHA-256, SHA-384, or SHA-512 hash
     * 2048-bit key, 224-bit q, SHA-224, SHA-256, SHA-384, or SHA-512 hash
     * 2048-bit key, 256-bit q, SHA-256, SHA-384, or SHA-512 hash
     * 3072-bit key, 256-bit q, SHA-256, SHA-384, or SHA-512 hash
     */
</span>    switch (Math.round(q.bitLength() / 8)) {
      case 20:
        // 1024 bit
        if (usersetting !== 2 && usersetting > 11 && usersetting !== 10 && usersetting < 8) {
          return 2; // prefer sha1
        }
        return usersetting;
      case 28:
        // 2048 bit
        if (usersetting > 11 && usersetting < 8) {
          return 11;
        }
        return usersetting;
      case 32:
        // 4096 bit // prefer sha224
        if (usersetting > 10 && usersetting < 8) {
          return 8; // prefer sha256
        }
        return usersetting;
      default:
        _util2.default.print_debug("DSA select hash algorithm: returning null for an unknown length of q");
        return null;
    }
  }
  this.select_hash_algorithm = select_hash_algorithm;

  function verify(hashalgo, s1, s2, m, p, q, g, y) {
    var hashed_data = _util2.default.getLeftNBits(_util2.default.Uint8Array2str(_hash2.default.digest(hashalgo, _util2.default.str2Uint8Array
(m))), q.bitLength());
    var hash = new _jsbn2.default(_util2.default.hexstrdump(hashed_data), 16);
    if (_jsbn2.default.ZERO.compareTo(s1) >= 0 || s1.compareTo(q) >= 0 || _jsbn2.default.ZERO.compareTo(s2) >= 0 || s2.compareTo
(q) >= 0) {
      _util2.default.print_debug("invalid DSA Signature");
      return null;
    }
    var w = s2.modInverse(q);
    if (_jsbn2.default.ZERO.compareTo(w) === 0) {
      _util2.default.print_debug("invalid DSA Signature");
      return null;
    }
    var u1 = hash.multiply(w).mod(q);
    var u2 = s1.multiply(w).mod(q);
    return g.modPow(u1, p).multiply(y.modPow(u2, p)).mod(p).mod(q);
  }

  this.sign = sign;
  this.verify = verify;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.publicKey.elgamal"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.publicKey.</span>elgamal ()](#apidoc.element.openpgp.crypto.publicKey.elgamal)
- description and source-code
```javascript
function Elgamal() {

  function encrypt(m, g, p, y) {
    //  choose k in {2,...,p-2}
    var pMinus2 = p.subtract(_jsbn2.default.TWO);
    var k = _random2.default.getRandomBigIntegerInRange(_jsbn2.default.ONE, pMinus2);
    k = k.mod(pMinus2).add(_jsbn2.default.ONE);
    var c = [];
    c[0] = g.modPow(k, p);
    c[1] = y.modPow(k, p).multiply(m).mod(p);
    return c;
  }

  function decrypt(c1, c2, p, x) {
    _util2.default.print_debug("Elgamal Decrypt:\nc1:" + _util2.default.hexstrdump(c1.toMPI()) + "\n" + "c2:" + _util2.default.hexstrdump
(c2.toMPI()) + "\n" + "p:" + _util2.default.hexstrdump(p.toMPI()) + "\n" + "x:" + _util2.default.hexstrdump(x.toMPI()));
    return c1.modPow(x, p).modInverse(p).multiply(c2).mod(p);
    //var c = c1.pow(x).modInverse(p); // c0^-a mod p
    //return c.multiply(c2).mod(p);
  }

  // signing and signature verification using Elgamal is not required by OpenPGP.
  this.encrypt = encrypt;
  this.decrypt = decrypt;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.publicKey.rsa"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.publicKey.</span>rsa ()](#apidoc.element.openpgp.crypto.publicKey.rsa)
- description and source-code
```javascript
function RSA() {
<span class="apidocCodeCommentSpan">  /**
   * This function uses jsbn Big Num library to decrypt RSA
   * @param m
   *            message
   * @param n
   *            RSA public modulus n as BigInteger
   * @param e
   *            RSA public exponent as BigInteger
   * @param d
   *            RSA d as BigInteger
   * @param p
   *            RSA p as BigInteger
   * @param q
   *            RSA q as BigInteger
   * @param u
   *            RSA u as BigInteger
   * @return {BigInteger} The decrypted value of the message
   */
</span>  function decrypt(m, n, e, d, p, q, u) {
    if (_config2.default.rsa_blinding) {
      m = blind(m, n, e);
    }
    var xp = m.mod(p).modPow(d.mod(p.subtract(_jsbn2.default.ONE)), p);
    var xq = m.mod(q).modPow(d.mod(q.subtract(_jsbn2.default.ONE)), q);
    _util2.default.print_debug("rsa.js decrypt\nxpn:" + _util2.default.hexstrdump(xp.toMPI()) + "\nxqn:" + _util2.default.hexstrdump
(xq.toMPI()));

    var t = xq.subtract(xp);
    if (t[0] === 0) {
      t = xp.subtract(xq);
      t = t.multiply(u).mod(q);
      t = q.subtract(t);
    } else {
      t = t.multiply(u).mod(q);
    }
    t = t.multiply(p).add(xp);
    if (_config2.default.rsa_blinding) {
      t = unblind(t, n);
    }
    return t;
  }

  /**
   * encrypt message
   * @param m message as BigInteger
   * @param e public MPI part as BigInteger
   * @param n public MPI part as BigInteger
   * @return BigInteger
   */
  function encrypt(m, e, n) {
    return m.modPowInt(e, n);
  }

  /* Sign and Verify */
  function sign(m, d, n) {
    return m.modPow(d, n);
  }

  function verify(x, e, n) {
    return x.modPowInt(e, n);
  }

  // "empty" RSA key constructor

  function KeyObject() {
    this.n = null;
    this.e = 0;
    this.ee = null;
    this.d = null;
    this.p = null;
    this.q = null;
    this.dmp1 = null;
    this.dmq1 = null;
    this.u = null;
  }

  // Generate a new random private key B bits long, using public expt E

  function generate(B, E) {
    var webCrypto = _util2.default.getWebCryptoAll();

    //
    // Native RSA keygen using Web Crypto
    //

    if (webCrypto) {
      var Euint32 = new Uint32Array([parseInt(E, 16)]); // get integer of exponent
      var Euint8 = new Uint8Array(Euint32.buffer); // get bytes of exponent
      var keyGenOpt;

      var keys;
      if (window.crypto && window.crypto.webkitSubtle) {
        // outdated spec implemented by Webkit
        keyGenOpt = {
          name: 'RSA-OAEP',
          modulusLength: B, // the specified keysize in bits
          publicExponent: Euint8.subarray(0, 3) // take three bytes (max 65537)
        };
        keys = webCrypto.generateKey(keyGenOpt, true, ['encrypt', 'decrypt']);
      } else {
        // current standard spec
        keyGenOpt = {
          name: 'RSASSA-PKCS1-v1_5',
          modulusLength: B, // the specified keysize in bits
          publicExponent: Euint8.subarray(0, 3), // take three bytes (max 65537)
          hash: {
            name: 'SHA-1' // not required for actual RSA keys, but for crypto api 'sign' and 'verify'
          }
        };

        keys = webCrypto.generateKey(keyGenOpt, true, ['sign', 'verify']);
        if (typeof keys.then !== 'function') {
          // IE11 KeyOperation
          keys = _util2.default.promisifyIE11Op(keys, 'Error generating RSA key pair.');
        }
      }

      return keys.then(exportKey).then(function (key) {
        if (key instanceof ArrayBuffer) {
          // parse raw ArrayBuffer bytes to jwk/json (WebKit/Safari/IE11 quirk)
          return decodeKey(JSON.parse(String.fromCharCode.apply(null, new Uint8Array(key))));
        }
        return decodeKey(key);
      });
    }

    function exportKey(keypair) {
      // export the generated keys as JsonWebKey (JWK)
      // https://tools.ietf.org/html/draft-ietf-jose-json-web-key-33
      var key = webCrypto.exportKey('jwk', keypair.privateKey);
      if (typeof key.then !== 'function') {
        // IE11 KeyOperation
        key = _util2.default.promisifyIE11Op(key, 'Error exporting RSA key pair.');
      }
      return key;
    }

    function decode ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.crypto.random"></a>[module openpgp.crypto.random](#apidoc.module.openpgp.crypto.random)

#### <a name="apidoc.element.openpgp.crypto.random.getRandomBigInteger"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.random.</span>getRandomBigInteger (bits)](#apidoc.element.openpgp.crypto.random.getRandomBigInteger)
- description and source-code
```javascript
function getRandomBigInteger(bits) {
  if (bits < 1) {
    throw new Error('Illegal parameter value: bits < 1');
  }
  var numBytes = Math.floor((bits + 7) / 8);

  var randomBits = _util2.default.Uint8Array2str(this.getRandomBytes(numBytes));
  if (bits % 8 > 0) {

    randomBits = String.fromCharCode(Math.pow(2, bits % 8) - 1 & randomBits.charCodeAt(0)) + randomBits.substring(1);
  }
  var mpi = new _mpi2.default();
  mpi.fromBytes(randomBits);
  return mpi.toBigInteger();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.random.getRandomBigIntegerInRange"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.random.</span>getRandomBigIntegerInRange (min, max)](#apidoc.element.openpgp.crypto.random.getRandomBigIntegerInRange)
- description and source-code
```javascript
function getRandomBigIntegerInRange(min, max) {
  if (max.compareTo(min) <= 0) {
    throw new Error('Illegal parameter value: max <= min');
  }

  var range = max.subtract(min);
  var r = this.getRandomBigInteger(range.bitLength());
  while (r.compareTo(range) > 0) {
    r = this.getRandomBigInteger(range.bitLength());
  }
  return min.add(r);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.random.getRandomBytes"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.random.</span>getRandomBytes (length)](#apidoc.element.openpgp.crypto.random.getRandomBytes)
- description and source-code
```javascript
function getRandomBytes(length) {
  var result = new Uint8Array(length);
  for (var i = 0; i < length; i++) {
    result[i] = this.getSecureRandomOctet();
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.random.getRandomValues"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.random.</span>getRandomValues (buf)](#apidoc.element.openpgp.crypto.random.getRandomValues)
- description and source-code
```javascript
function getRandomValues(buf) {
  if (!(buf instanceof Uint8Array)) {
    throw new Error('Invalid type: buf not an Uint8Array');
  }
  if (typeof window !== 'undefined' && window.crypto && window.crypto.getRandomValues) {
    window.crypto.getRandomValues(buf);
  } else if (typeof window !== 'undefined' && _typeof(window.msCrypto) === 'object' && typeof window.msCrypto.getRandomValues === '
function') {
    window.msCrypto.getRandomValues(buf);
  } else if (nodeCrypto) {
    var bytes = nodeCrypto.randomBytes(buf.length);
    buf.set(bytes);
  } else if (this.randomBuffer.buffer) {
    this.randomBuffer.get(buf);
  } else {
    throw new Error('No secure random number generator available.');
  }
  return buf;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.random.getSecureRandom"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.random.</span>getSecureRandom (from, to)](#apidoc.element.openpgp.crypto.random.getSecureRandom)
- description and source-code
```javascript
function getSecureRandom(from, to) {
  var randUint = this.getSecureRandomUint();
  var bits = (to - from).toString(2).length;
  while ((randUint & Math.pow(2, bits) - 1) > to - from) {
    randUint = this.getSecureRandomUint();
  }
  return from + Math.abs(randUint & Math.pow(2, bits) - 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.random.getSecureRandomOctet"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.random.</span>getSecureRandomOctet ()](#apidoc.element.openpgp.crypto.random.getSecureRandomOctet)
- description and source-code
```javascript
function getSecureRandomOctet() {
  var buf = new Uint8Array(1);
  this.getRandomValues(buf);
  return buf[0];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.crypto.random.getSecureRandomUint"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.random.</span>getSecureRandomUint ()](#apidoc.element.openpgp.crypto.random.getSecureRandomUint)
- description and source-code
```javascript
function getSecureRandomUint() {
  var buf = new Uint8Array(4);
  var dv = new DataView(buf.buffer);
  this.getRandomValues(buf);
  return dv.getUint32(0);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.crypto.signature"></a>[module openpgp.crypto.signature](#apidoc.module.openpgp.crypto.signature)

#### <a name="apidoc.element.openpgp.crypto.signature.sign"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.signature.</span>sign (hash_algo, algo, keyIntegers, data)](#apidoc.element.openpgp.crypto.signature.sign)
- description and source-code
```javascript
function sign(hash_algo, algo, keyIntegers, data) {

  data = _util2.default.Uint8Array2str(data);

  var m;

  switch (algo) {
    case 1:
    // RSA (Encrypt or Sign) [HAC]
    case 2:
    // RSA Encrypt-Only [HAC]
    case 3:
      // RSA Sign-Only [HAC]
      var rsa = new _public_key2.default.rsa();
      var d = keyIntegers[2].toBigInteger();
      var n = keyIntegers[0].toBigInteger();
      m = _pkcs2.default.emsa.encode(hash_algo, data, keyIntegers[0].byteLength());
      return _util2.default.str2Uint8Array(rsa.sign(m, d, n).toMPI());

    case 17:
      // DSA (Digital Signature Algorithm) [FIPS186] [HAC]
      var dsa = new _public_key2.default.dsa();

      var p = keyIntegers[0].toBigInteger();
      var q = keyIntegers[1].toBigInteger();
      var g = keyIntegers[2].toBigInteger();
      var x = keyIntegers[4].toBigInteger();
      m = data;
      var result = dsa.sign(hash_algo, m, g, p, q, x);

      return _util2.default.str2Uint8Array(result[0].toString() + result[1].toString());
    case 16:
      // Elgamal (Encrypt-Only) [ELGAMAL] [HAC]
      throw new Error('Signing with Elgamal is not defined in the OpenPGP standard.');
    default:
      throw new Error('Invalid signature algorithm.');
  }
}
```
- example usage
```shell
...

'''js
options = {
data: 'Hello, World!',                             // input as String (or Uint8Array)
privateKeys: privKeyObj // for signing
};

openpgp.sign(options).then(function(signed) {
cleartext = signed.data; // '-----BEGIN PGP SIGNED MESSAGE ... END PGP SIGNATURE-----'
});
'''

'''js
options = {
message: openpgp.cleartext.readArmored(cleartext), // parse armored message
...
```

#### <a name="apidoc.element.openpgp.crypto.signature.verify"></a>[function <span class="apidocSignatureSpan">openpgp.crypto.signature.</span>verify (algo, hash_algo, msg_MPIs, publickey_MPIs, data)](#apidoc.element.openpgp.crypto.signature.verify)
- description and source-code
```javascript
function verify(algo, hash_algo, msg_MPIs, publickey_MPIs, data) {
  var m;

  data = _util2.default.Uint8Array2str(data);

  switch (algo) {
    case 1:
    // RSA (Encrypt or Sign) [HAC]
    case 2:
    // RSA Encrypt-Only [HAC]
    case 3:
      // RSA Sign-Only [HAC]
      var rsa = new _public_key2.default.rsa();
      var n = publickey_MPIs[0].toBigInteger();
      var k = publickey_MPIs[0].byteLength();
      var e = publickey_MPIs[1].toBigInteger();
      m = msg_MPIs[0].toBigInteger();
      var EM = rsa.verify(m, e, n);
      var EM2 = _pkcs2.default.emsa.encode(hash_algo, data, k);
      return EM.compareTo(EM2) === 0;
    case 16:
      // Elgamal (Encrypt-Only) [ELGAMAL] [HAC]
      throw new Error("signing with Elgamal is not defined in the OpenPGP standard.");
    case 17:
      // DSA (Digital Signature Algorithm) [FIPS186] [HAC]
      var dsa = new _public_key2.default.dsa();
      var s1 = msg_MPIs[0].toBigInteger();
      var s2 = msg_MPIs[1].toBigInteger();
      var p = publickey_MPIs[0].toBigInteger();
      var q = publickey_MPIs[1].toBigInteger();
      var g = publickey_MPIs[2].toBigInteger();
      var y = publickey_MPIs[3].toBigInteger();
      m = data;
      var dopublic = dsa.verify(hash_algo, s1, s2, m, p, q, g, y);
      return dopublic.compareTo(s1) === 0;
    default:
      throw new Error('Invalid signature algorithm.');
  }
}
```
- example usage
```shell
...

'''js
options = {
    message: openpgp.cleartext.readArmored(cleartext), // parse armored message
    publicKeys: openpgp.key.readArmored(pubkey).keys   // for verification
};

openpgp.verify(options).then(function(verified) {
	validity = verified.signatures[0].valid; // true
	if (validity) {
		console.log('signed by key id ' + verified.signatures[0].keyid.toHex());
	}
});
'''
...
```



# <a name="apidoc.module.openpgp.default"></a>[module openpgp.default](#apidoc.module.openpgp.default)

#### <a name="apidoc.element.openpgp.default.decrypt"></a>[function <span class="apidocSignatureSpan">openpgp.default.</span>decrypt (_ref6)](#apidoc.element.openpgp.default.decrypt)
- description and source-code
```javascript
function decrypt(_ref6) {
  var message = _ref6.message;
  var privateKey = _ref6.privateKey;
  var publicKeys = _ref6.publicKeys;
  var sessionKey = _ref6.sessionKey;
  var password = _ref6.password;
  var _ref6$format = _ref6.format;
  var format = _ref6$format === undefined ? 'utf8' : _ref6$format;
  var _ref6$signature = _ref6.signature;
  var signature = _ref6$signature === undefined ? null : _ref6$signature;

  checkMessage(message);publicKeys = toArray(publicKeys);

  if (!nativeAEAD() && asyncProxy) {
    // use web worker if web crypto apis are not supported
    return asyncProxy.delegate('decrypt', { message: message, privateKey: privateKey, publicKeys: publicKeys, sessionKey: sessionKey
, password: password, format: format, signature: signature });
  }

  return message.decrypt(privateKey, sessionKey, password).then(function (message) {

    var result = parseMessage(message, format);
    if (result.data) {
      // verify
      if (!publicKeys) {
        publicKeys = [];
      }
      if (signature) {
        //detached signature
        result.signatures = message.verifyDetached(signature, publicKeys);
      } else {
        result.signatures = message.verify(publicKeys);
      }
    }
    return result;
  }).catch(onError.bind(null, 'Error decrypting message'));
}
```
- example usage
```shell
...
'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
'''

#### Encrypt and decrypt *String* data with PGP keys

'''js
...
```

#### <a name="apidoc.element.openpgp.default.decryptKey"></a>[function <span class="apidocSignatureSpan">openpgp.default.</span>decryptKey (_ref4)](#apidoc.element.openpgp.default.decryptKey)
- description and source-code
```javascript
function decryptKey(_ref4) {
  var privateKey = _ref4.privateKey;
  var passphrase = _ref4.passphrase;

  if (asyncProxy) {
    // use web worker if available
    return asyncProxy.delegate('decryptKey', { privateKey: privateKey, passphrase: passphrase });
  }

  return execute(function () {

    if (!privateKey.decrypt(passphrase)) {
      throw new Error('Invalid passphrase');
    }
    return {
      key: privateKey
    };
  }, 'Error decrypting private key');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.default.decryptSessionKey"></a>[function <span class="apidocSignatureSpan">openpgp.default.</span>decryptSessionKey (_ref10)](#apidoc.element.openpgp.default.decryptSessionKey)
- description and source-code
```javascript
function decryptSessionKey(_ref10) {
  var message = _ref10.message;
  var privateKey = _ref10.privateKey;
  var password = _ref10.password;

  checkMessage(message);

  if (asyncProxy) {
    // use web worker if available
    return asyncProxy.delegate('decryptSessionKey', { message: message, privateKey: privateKey, password: password });
  }

  return execute(function () {
    return message.decryptSessionKey(privateKey, password);
  }, 'Error decrypting session key');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.default.destroyWorker"></a>[function <span class="apidocSignatureSpan">openpgp.default.</span>destroyWorker ()](#apidoc.element.openpgp.default.destroyWorker)
- description and source-code
```javascript
function destroyWorker() {
  asyncProxy = undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.default.encrypt"></a>[function <span class="apidocSignatureSpan">openpgp.default.</span>encrypt (_ref5)](#apidoc.element.openpgp.default.encrypt)
- description and source-code
```javascript
function encrypt(_ref5) {
  var data = _ref5.data;
  var publicKeys = _ref5.publicKeys;
  var privateKeys = _ref5.privateKeys;
  var passwords = _ref5.passwords;
  var filename = _ref5.filename;
  var _ref5$armor = _ref5.armor;
  var armor = _ref5$armor === undefined ? true : _ref5$armor;
  var _ref5$detached = _ref5.detached;
  var detached = _ref5$detached === undefined ? false : _ref5$detached;
  var _ref5$signature = _ref5.signature;
  var signature = _ref5$signature === undefined ? null : _ref5$signature;

  checkData(data);publicKeys = toArray(publicKeys);privateKeys = toArray(privateKeys);passwords = toArray(passwords);

  if (!nativeAEAD() && asyncProxy) {
    // use web worker if web crypto apis are not supported
    return asyncProxy.delegate('encrypt', { data: data, publicKeys: publicKeys, privateKeys: privateKeys, passwords: passwords,
filename: filename, armor: armor, detached: detached, signature: signature });
  }
  var result = {};
  return Promise.resolve().then(function () {

    var message = createMessage(data, filename);
    if (!privateKeys) {
      privateKeys = [];
    }
    if (privateKeys.length || signature) {
      // sign the message only if private keys or signature is specified
      if (detached) {
        var detachedSignature = message.signDetached(privateKeys, signature);
        if (armor) {
          result.signature = detachedSignature.armor();
        } else {
          result.signature = detachedSignature;
        }
      } else {
        message = message.sign(privateKeys, signature);
      }
    }
    return message.encrypt(publicKeys, passwords);
  }).then(function (message) {
    if (armor) {
      result.data = message.armor();
    } else {
      result.message = message;
    }
    return result;
  }).catch(onError.bind(null, 'Error encrypting message'));
}
```
- example usage
```shell
...

options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
...
```

#### <a name="apidoc.element.openpgp.default.encryptSessionKey"></a>[function <span class="apidocSignatureSpan">openpgp.default.</span>encryptSessionKey (_ref9)](#apidoc.element.openpgp.default.encryptSessionKey)
- description and source-code
```javascript
function encryptSessionKey(_ref9) {
  var data = _ref9.data;
  var algorithm = _ref9.algorithm;
  var publicKeys = _ref9.publicKeys;
  var passwords = _ref9.passwords;

  checkbinary(data);checkString(algorithm, 'algorithm');publicKeys = toArray(publicKeys);passwords = toArray(passwords);

  if (asyncProxy) {
    // use web worker if available
    return asyncProxy.delegate('encryptSessionKey', { data: data, algorithm: algorithm, publicKeys: publicKeys, passwords: passwords
 });
  }

  return execute(function () {
    return {

      message: messageLib.encryptSessionKey(data, algorithm, publicKeys, passwords)

    };
  }, 'Error encrypting session key');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.default.generateKey"></a>[function <span class="apidocSignatureSpan">openpgp.default.</span>generateKey ()](#apidoc.element.openpgp.default.generateKey)
- description and source-code
```javascript
function generateKey() {
  var _ref2 = arguments.length <= 0 || arguments[0] === undefined ? {} : arguments[0];

  var _ref2$userIds = _ref2.userIds;
  var userIds = _ref2$userIds === undefined ? [] : _ref2$userIds;
  var passphrase = _ref2.passphrase;
  var _ref2$numBits = _ref2.numBits;
  var numBits = _ref2$numBits === undefined ? 2048 : _ref2$numBits;
  var _ref2$unlocked = _ref2.unlocked;
  var unlocked = _ref2$unlocked === undefined ? false : _ref2$unlocked;
  var _ref2$keyExpirationTi = _ref2.keyExpirationTime;
  var keyExpirationTime = _ref2$keyExpirationTi === undefined ? 0 : _ref2$keyExpirationTi;

  var options = formatUserIds({ userIds: userIds, passphrase: passphrase, numBits: numBits, unlocked: unlocked, keyExpirationTime
: keyExpirationTime });

  if (!_util2.default.getWebCryptoAll() && asyncProxy) {
    // use web worker if web crypto apis are not supported
    return asyncProxy.delegate('generateKey', options);
  }

  return key.generate(options).then(function (newKey) {
    return {

      key: newKey,
      privateKeyArmored: newKey.armor(),
      publicKeyArmored: newKey.toPublic().armor()

    };
  }).catch(onError.bind(null, 'Error generating keypair'));
}
```
- example usage
```shell
...
'''js
var options = {
    userIds: [{ name:'Jon Smith', email:'jon@example.com' }], // multiple user IDs
    numBits: 4096,                                            // RSA key size
    passphrase: 'super long and hard to guess secret'         // protects the private key
};

openpgp.generateKey(options).then(function(key) {
    var privkey = key.privateKeyArmored; // '-----BEGIN PGP PRIVATE KEY BLOCK ... '
    var pubkey = key.publicKeyArmored;   // '-----BEGIN PGP PUBLIC KEY BLOCK ... '
});
'''

#### Lookup public key on HKP server
...
```

#### <a name="apidoc.element.openpgp.default.getWorker"></a>[function <span class="apidocSignatureSpan">openpgp.default.</span>getWorker ()](#apidoc.element.openpgp.default.getWorker)
- description and source-code
```javascript
function getWorker() {
  return asyncProxy;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.default.initWorker"></a>[function <span class="apidocSignatureSpan">openpgp.default.</span>initWorker ()](#apidoc.element.openpgp.default.initWorker)
- description and source-code
```javascript
function initWorker() {
  var _ref = arguments.length <= 0 || arguments[0] === undefined ? {} : arguments[0];

  var _ref$path = _ref.path;
  var path = _ref$path === undefined ? 'openpgp.worker.js' : _ref$path;
  var worker = _ref.worker;

  if (worker || typeof window !== 'undefined' && window.Worker) {
    asyncProxy = new _async_proxy2.default({ path: path, worker: worker, config: _config2.default });
    return true;
  }
}
```
- example usage
```shell
...
Here are some examples of how to use the v2.x api. For more elaborate examples and working code, please check out the [public api
 unit tests](https://github.com/openpgpjs/openpgpjs/blob/master/test/general/openpgp.js). If you're upgrading from v1.x it might
 help to check out the [documentation](https://github.com/openpgpjs/openpgpjs#documentation).

#### Set up

'''js
var openpgp = require('openpgp'); // use as CommonJS, AMD, ES6 module or via window.openpgp

openpgp.initWorker({ path:'openpgp.worker.js' }) // set the relative web worker path

openpgp.config.aead_protect = true // activate fast AES-GCM mode (not yet OpenPGP standard)
'''

#### Encrypt and decrypt *Uint8Array* data with a password

'''js
...
```

#### <a name="apidoc.element.openpgp.default.reformatKey"></a>[function <span class="apidocSignatureSpan">openpgp.default.</span>reformatKey ()](#apidoc.element.openpgp.default.reformatKey)
- description and source-code
```javascript
function reformatKey() {
  var _ref3 = arguments.length <= 0 || arguments[0] === undefined ? {} : arguments[0];

  var privateKey = _ref3.privateKey;
  var _ref3$userIds = _ref3.userIds;
  var userIds = _ref3$userIds === undefined ? [] : _ref3$userIds;
  var _ref3$passphrase = _ref3.passphrase;
  var passphrase = _ref3$passphrase === undefined ? "" : _ref3$passphrase;
  var _ref3$unlocked = _ref3.unlocked;
  var unlocked = _ref3$unlocked === undefined ? false : _ref3$unlocked;
  var _ref3$keyExpirationTi = _ref3.keyExpirationTime;
  var keyExpirationTime = _ref3$keyExpirationTi === undefined ? 0 : _ref3$keyExpirationTi;

  var options = formatUserIds({ privateKey: privateKey, userIds: userIds, passphrase: passphrase, unlocked: unlocked, keyExpirationTime
: keyExpirationTime });

  if (asyncProxy) {
    return asyncProxy.delegate('reformatKey', options);
  }

  return key.reformat(options).then(function (newKey) {
    return {

      key: newKey,
      privateKeyArmored: newKey.armor(),
      publicKeyArmored: newKey.toPublic().armor()

    };
  }).catch(onError.bind(null, 'Error reformatting keypair'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.default.sign"></a>[function <span class="apidocSignatureSpan">openpgp.default.</span>sign (_ref7)](#apidoc.element.openpgp.default.sign)
- description and source-code
```javascript
function sign(_ref7) {
  var data = _ref7.data;
  var privateKeys = _ref7.privateKeys;
  var _ref7$armor = _ref7.armor;
  var armor = _ref7$armor === undefined ? true : _ref7$armor;
  var _ref7$detached = _ref7.detached;
  var detached = _ref7$detached === undefined ? false : _ref7$detached;

  checkString(data);
  privateKeys = toArray(privateKeys);

  if (asyncProxy) {
    // use web worker if available
    return asyncProxy.delegate('sign', { data: data, privateKeys: privateKeys, armor: armor, detached: detached });
  }

  var result = {};
  return execute(function () {

    var cleartextMessage = new cleartext.CleartextMessage(data);

    if (detached) {
      var signature = cleartextMessage.signDetached(privateKeys);
      if (armor) {
        result.signature = signature.armor();
      } else {
        result.signature = signature;
      }
    } else {
      cleartextMessage.sign(privateKeys);
    }

    if (armor) {
      result.data = cleartextMessage.armor();
    } else {
      result.message = cleartextMessage;
    }
    return result;
  }, 'Error signing cleartext message');
}
```
- example usage
```shell
...

'''js
options = {
data: 'Hello, World!',                             // input as String (or Uint8Array)
privateKeys: privKeyObj // for signing
};

openpgp.sign(options).then(function(signed) {
cleartext = signed.data; // '-----BEGIN PGP SIGNED MESSAGE ... END PGP SIGNATURE-----'
});
'''

'''js
options = {
message: openpgp.cleartext.readArmored(cleartext), // parse armored message
...
```

#### <a name="apidoc.element.openpgp.default.verify"></a>[function <span class="apidocSignatureSpan">openpgp.default.</span>verify (_ref8)](#apidoc.element.openpgp.default.verify)
- description and source-code
```javascript
function verify(_ref8) {
  var message = _ref8.message;
  var publicKeys = _ref8.publicKeys;
  var _ref8$signature = _ref8.signature;
  var signature = _ref8$signature === undefined ? null : _ref8$signature;

  checkCleartextMessage(message);
  publicKeys = toArray(publicKeys);

  if (asyncProxy) {
    // use web worker if available
    return asyncProxy.delegate('verify', { message: message, publicKeys: publicKeys, signature: signature });
  }

  var result = {};
  return execute(function () {
    result.data = message.getText();

    if (signature) {
      //detached signature
      result.signatures = message.verifyDetached(signature, publicKeys);
    } else {
      result.signatures = message.verify(publicKeys);
    }
    return result;
  }, 'Error verifying cleartext signed message');
}
```
- example usage
```shell
...

'''js
options = {
    message: openpgp.cleartext.readArmored(cleartext), // parse armored message
    publicKeys: openpgp.key.readArmored(pubkey).keys   // for verification
};

openpgp.verify(options).then(function(verified) {
	validity = verified.signatures[0].valid; // true
	if (validity) {
		console.log('signed by key id ' + verified.signatures[0].keyid.toHex());
	}
});
'''
...
```



# <a name="apidoc.module.openpgp.enums"></a>[module openpgp.enums](#apidoc.module.openpgp.enums)

#### <a name="apidoc.element.openpgp.enums.read"></a>[function <span class="apidocSignatureSpan">openpgp.enums.</span>read (type, e)](#apidoc.element.openpgp.enums.read)
- description and source-code
```javascript
function read(type, e) {
  for (var i in type) {
    if (type[i] === parseInt(e)) {
      return i;
    }
  }

  throw new Error('Invalid enum value.');
}
```
- example usage
```shell
...
openpgp.encrypt(options).then(function(ciphertext) {
    encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
...
```

#### <a name="apidoc.element.openpgp.enums.write"></a>[function <span class="apidocSignatureSpan">openpgp.enums.</span>write (type, e)](#apidoc.element.openpgp.enums.write)
- description and source-code
```javascript
function write(type, e) {
  if (typeof e === 'number') {
    e = this.read(type, e);
  }

  if (type[e] !== undefined) {
    return type[e];
  } else {
    throw new Error('Invalid enum value.');
  }
}
```
- example usage
```shell
...
options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
password: 'secret stuff',                 // decrypt with password
...
```



# <a name="apidoc.module.openpgp.key"></a>[module openpgp.key](#apidoc.module.openpgp.key)

#### <a name="apidoc.element.openpgp.key.Key"></a>[function <span class="apidocSignatureSpan">openpgp.key.</span>Key (packetlist)](#apidoc.element.openpgp.key.Key)
- description and source-code
```javascript
function Key(packetlist) {
  if (!(this instanceof Key)) {
    return new Key(packetlist);
  }
  // same data as in packetlist but in structured form
  this.primaryKey = null;
  this.revocationSignature = null;
  this.directSignatures = null;
  this.users = null;
  this.subKeys = null;
  this.packetlist2structure(packetlist);
  if (!this.primaryKey || !this.users) {
    throw new Error('Invalid key: need at least key and user ID packet');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.generate"></a>[function <span class="apidocSignatureSpan">openpgp.key.</span>generate (options)](#apidoc.element.openpgp.key.generate)
- description and source-code
```javascript
function generate(options) {
  var secretKeyPacket, secretSubkeyPacket;
  return Promise.resolve().then(function () {
    options.keyType = options.keyType || _enums2.default.publicKey.rsa_encrypt_sign;
    if (options.keyType !== _enums2.default.publicKey.rsa_encrypt_sign) {
      // RSA Encrypt-Only and RSA Sign-Only are deprecated and SHOULD NOT be generated
      throw new Error('Only RSA Encrypt or Sign supported');
    }

    if (!options.passphrase) {
      // Key without passphrase is unlocked by definition
      options.unlocked = true;
    }
    if (String.prototype.isPrototypeOf(options.userIds) || typeof options.userIds === 'string') {
      options.userIds = [options.userIds];
    }

    return Promise.all([generateSecretKey(), generateSecretSubkey()]).then(function () {
      return wrapKeyObject(secretKeyPacket, secretSubkeyPacket, options);
    });
  });

  function generateSecretKey() {
    secretKeyPacket = new _packet2.default.SecretKey();
    secretKeyPacket.algorithm = _enums2.default.read(_enums2.default.publicKey, options.keyType);
    return secretKeyPacket.generate(options.numBits);
  }

  function generateSecretSubkey() {
    secretSubkeyPacket = new _packet2.default.SecretSubkey();
    secretSubkeyPacket.algorithm = _enums2.default.read(_enums2.default.publicKey, options.keyType);
    return secretSubkeyPacket.generate(options.numBits);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.getPreferredSymAlgo"></a>[function <span class="apidocSignatureSpan">openpgp.key.</span>getPreferredSymAlgo (keys)](#apidoc.element.openpgp.key.getPreferredSymAlgo)
- description and source-code
```javascript
function getPreferredSymAlgo(keys) {
  var prioMap = {};
  keys.forEach(function (key) {
    var primaryUser = key.getPrimaryUser();
    if (!primaryUser || !primaryUser.selfCertificate.preferredSymmetricAlgorithms) {
      return _config2.default.encryption_cipher;
    }
    primaryUser.selfCertificate.preferredSymmetricAlgorithms.forEach(function (algo, index) {
      var entry = prioMap[algo] || (prioMap[algo] = { prio: 0, count: 0, algo: algo });
      entry.prio += 64 >> index;
      entry.count++;
    });
  });
  var prefAlgo = { prio: 0, algo: _config2.default.encryption_cipher };
  for (var algo in prioMap) {
    try {
      if (algo !== _enums2.default.symmetric.plaintext && algo !== _enums2.default.symmetric.idea && // not implemented
      _enums2.default.read(_enums2.default.symmetric, algo) && // known algorithm
      prioMap[algo].count === keys.length && // available for all keys
      prioMap[algo].prio > prefAlgo.prio) {
        prefAlgo = prioMap[algo];
      }
    } catch (e) {}
  }
  return prefAlgo.algo;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.readArmored"></a>[function <span class="apidocSignatureSpan">openpgp.key.</span>readArmored (armoredText)](#apidoc.element.openpgp.key.readArmored)
- description and source-code
```javascript
function readArmored(armoredText) {
  var result = {};
  result.keys = [];
  try {
    var input = _armor2.default.decode(armoredText);
    if (!(input.type === _enums2.default.armor.public_key || input.type === _enums2.default.armor.private_key)) {
      throw new Error('Armored text not of type key');
    }
    var packetlist = new _packet2.default.List();
    packetlist.read(input.data);
    var keyIndex = packetlist.indexOfTag(_enums2.default.packet.publicKey, _enums2.default.packet.secretKey);
    if (keyIndex.length === 0) {
      throw new Error('No key packet found in armored text');
    }
    for (var i = 0; i < keyIndex.length; i++) {
      var oneKeyList = packetlist.slice(keyIndex[i], keyIndex[i + 1]);
      try {
        var newKey = new Key(oneKeyList);
        result.keys.push(newKey);
      } catch (e) {
        result.err = result.err || [];
        result.err.push(e);
      }
    }
  } catch (e) {
    result.err = result.err || [];
    result.err.push(e);
  }
  return result;
}
```
- example usage
```shell
...
'''js
var options, encrypted;

var pubkey = '-----BEGIN PGP PUBLIC KEY BLOCK ... END PGP PUBLIC KEY BLOCK-----';
var privkey = '-----BEGIN PGP PRIVATE KEY BLOCK ... END PGP PRIVATE KEY BLOCK-----'; //encrypted private key
var passphrase = 'secret passphrase'; //what the privKey is encrypted with

var privKeyObj = openpgp.key.readArmored(privkey).keys[0];
privKeyObj.decrypt(passphrase);

options = {
    data: 'Hello, World!',                             // input as String (or Uint8Array)
    publicKeys: openpgp.key.readArmored(pubkey).keys,  // for encryption
    privateKeys: privKeyObj // for signing (optional)
};
...
```

#### <a name="apidoc.element.openpgp.key.reformat"></a>[function <span class="apidocSignatureSpan">openpgp.key.</span>reformat (options)](#apidoc.element.openpgp.key.reformat)
- description and source-code
```javascript
function reformat(options) {
  var secretKeyPacket, secretSubkeyPacket;
  return Promise.resolve().then(function () {

    options.keyType = options.keyType || _enums2.default.publicKey.rsa_encrypt_sign;
    if (options.keyType !== _enums2.default.publicKey.rsa_encrypt_sign) {
      // RSA Encrypt-Only and RSA Sign-Only are deprecated and SHOULD NOT be generated
      throw new Error('Only RSA Encrypt or Sign supported');
    }

    if (!options.passphrase) {
      // Key without passphrase is unlocked by definition
      options.unlocked = true;
    }
    if (String.prototype.isPrototypeOf(options.userIds) || typeof options.userIds === 'string') {
      options.userIds = [options.userIds];
    }
    var packetlist = options.privateKey.toPacketlist();
    for (var i = 0; i < packetlist.length; i++) {
      if (packetlist[i].tag === _enums2.default.packet.secretKey) {
        secretKeyPacket = packetlist[i];
      } else if (packetlist[i].tag === _enums2.default.packet.secretSubkey) {
        secretSubkeyPacket = packetlist[i];
      }
    }
    return wrapKeyObject(secretKeyPacket, secretSubkeyPacket, options);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.key.Key"></a>[module openpgp.key.Key](#apidoc.module.openpgp.key.Key)

#### <a name="apidoc.element.openpgp.key.Key.Key"></a>[function <span class="apidocSignatureSpan">openpgp.key.</span>Key (packetlist)](#apidoc.element.openpgp.key.Key.Key)
- description and source-code
```javascript
function Key(packetlist) {
  if (!(this instanceof Key)) {
    return new Key(packetlist);
  }
  // same data as in packetlist but in structured form
  this.primaryKey = null;
  this.revocationSignature = null;
  this.directSignatures = null;
  this.users = null;
  this.subKeys = null;
  this.packetlist2structure(packetlist);
  if (!this.primaryKey || !this.users) {
    throw new Error('Invalid key: need at least key and user ID packet');
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.key.Key.prototype"></a>[module openpgp.key.Key.prototype](#apidoc.module.openpgp.key.Key.prototype)

#### <a name="apidoc.element.openpgp.key.Key.prototype.armor"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>armor ()](#apidoc.element.openpgp.key.Key.prototype.armor)
- description and source-code
```javascript
armor = function () {
  var type = this.isPublic() ? _enums2.default.armor.public_key : _enums2.default.armor.private_key;
  return _armor2.default.encode(type, this.toPacketlist().write());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.decrypt"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>decrypt (passphrase)](#apidoc.element.openpgp.key.Key.prototype.decrypt)
- description and source-code
```javascript
decrypt = function (passphrase) {
  if (this.isPrivate()) {
    var keys = this.getAllKeyPackets();
    for (var i = 0; i < keys.length; i++) {
      var success = keys[i].decrypt(passphrase);
      if (!success) {
        return false;
      }
    }
  } else {
    throw new Error("Nothing to decrypt in a public key");
  }
  return true;
}
```
- example usage
```shell
...
'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
'''

#### Encrypt and decrypt *String* data with PGP keys

'''js
...
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.decryptKeyPacket"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>decryptKeyPacket (keyIds, passphrase)](#apidoc.element.openpgp.key.Key.prototype.decryptKeyPacket)
- description and source-code
```javascript
decryptKeyPacket = function (keyIds, passphrase) {
  if (this.isPrivate()) {
    var keys = this.getAllKeyPackets();
    for (var i = 0; i < keys.length; i++) {
      var keyId = keys[i].getKeyId();
      for (var j = 0; j < keyIds.length; j++) {
        if (keyId.equals(keyIds[j])) {
          var success = keys[i].decrypt(passphrase);
          if (!success) {
            return false;
          }
        }
      }
    }
  } else {
    throw new Error("Nothing to decrypt in a public key");
  }
  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.encrypt"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>encrypt (passphrase)](#apidoc.element.openpgp.key.Key.prototype.encrypt)
- description and source-code
```javascript
encrypt = function (passphrase) {
  if (!this.isPrivate()) {
    throw new Error("Nothing to encrypt in a public key");
  }

  var keys = this.getAllKeyPackets();
  for (var i = 0; i < keys.length; i++) {
    keys[i].encrypt(passphrase);
    keys[i].clearPrivateMPIs();
  }
}
```
- example usage
```shell
...

options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
...
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.getAllKeyPackets"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>getAllKeyPackets ()](#apidoc.element.openpgp.key.Key.prototype.getAllKeyPackets)
- description and source-code
```javascript
getAllKeyPackets = function () {
  return [this.primaryKey].concat(this.getSubkeyPackets());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.getEncryptionKeyPacket"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>getEncryptionKeyPacket ()](#apidoc.element.openpgp.key.Key.prototype.getEncryptionKeyPacket)
- description and source-code
```javascript
getEncryptionKeyPacket = function () {
  // V4: by convention subkeys are prefered for encryption service
  // V3: keys MUST NOT have subkeys
  if (this.subKeys) {
    for (var i = 0; i < this.subKeys.length; i++) {
      if (this.subKeys[i].isValidEncryptionKey(this.primaryKey)) {
        return this.subKeys[i].subKey;
      }
    }
  }
  // if no valid subkey for encryption, evaluate primary key
  var primaryUser = this.getPrimaryUser();
  if (primaryUser && primaryUser.selfCertificate && !primaryUser.selfCertificate.isExpired() && isValidEncryptionKeyPacket(this.
primaryKey, primaryUser.selfCertificate)) {
    return this.primaryKey;
  }
  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.getExpirationTime"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>getExpirationTime ()](#apidoc.element.openpgp.key.Key.prototype.getExpirationTime)
- description and source-code
```javascript
getExpirationTime = function () {
  if (this.primaryKey.version === 3) {
    return getExpirationTime(this.primaryKey);
  }
  if (this.primaryKey.version === 4) {
    var primaryUser = this.getPrimaryUser();
    if (!primaryUser) {
      return null;
    }
    return getExpirationTime(this.primaryKey, primaryUser.selfCertificate);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.getKeyIds"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>getKeyIds ()](#apidoc.element.openpgp.key.Key.prototype.getKeyIds)
- description and source-code
```javascript
getKeyIds = function () {
  var keyIds = [];
  var keys = this.getAllKeyPackets();
  for (var i = 0; i < keys.length; i++) {
    keyIds.push(keys[i].getKeyId());
  }
  return keyIds;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.getKeyPacket"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>getKeyPacket (keyIds)](#apidoc.element.openpgp.key.Key.prototype.getKeyPacket)
- description and source-code
```javascript
getKeyPacket = function (keyIds) {
  var keys = this.getAllKeyPackets();
  for (var i = 0; i < keys.length; i++) {
    var keyId = keys[i].getKeyId();
    for (var j = 0; j < keyIds.length; j++) {
      if (keyId.equals(keyIds[j])) {
        return keys[i];
      }
    }
  }
  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.getPreferredHashAlgorithm"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>getPreferredHashAlgorithm ()](#apidoc.element.openpgp.key.Key.prototype.getPreferredHashAlgorithm)
- description and source-code
```javascript
getPreferredHashAlgorithm = function () {
  var primaryUser = this.getPrimaryUser();
  if (primaryUser && primaryUser.selfCertificate.preferredHashAlgorithms) {
    return primaryUser.selfCertificate.preferredHashAlgorithms[0];
  }
  return _config2.default.prefer_hash_algorithm;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.getPrimaryUser"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>getPrimaryUser ()](#apidoc.element.openpgp.key.Key.prototype.getPrimaryUser)
- description and source-code
```javascript
getPrimaryUser = function () {
  var primUser = [];
  for (var i = 0; i < this.users.length; i++) {
    if (!this.users[i].userId || !this.users[i].selfCertifications) {
      continue;
    }
    for (var j = 0; j < this.users[i].selfCertifications.length; j++) {
      primUser.push({ index: i, user: this.users[i], selfCertificate: this.users[i].selfCertifications[j] });
    }
  }
  // sort by primary user flag and signature creation time
  primUser = primUser.sort(function (a, b) {
    if (a.selfCertificate.isPrimaryUserID > b.selfCertificate.isPrimaryUserID) {
      return -1;
    } else if (a.selfCertificate.isPrimaryUserID < b.selfCertificate.isPrimaryUserID) {
      return 1;
    } else if (a.selfCertificate.created > b.selfCertificate.created) {
      return -1;
    } else if (a.selfCertificate.created < b.selfCertificate.created) {
      return 1;
    } else {
      return 0;
    }
  });
  // return first valid
  for (var k = 0; k < primUser.length; k++) {
    if (primUser[k].user.isValidSelfCertificate(this.primaryKey, primUser[k].selfCertificate)) {
      return primUser[k];
    }
  }
  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.getSigningKeyPacket"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>getSigningKeyPacket (keyId)](#apidoc.element.openpgp.key.Key.prototype.getSigningKeyPacket)
- description and source-code
```javascript
getSigningKeyPacket = function (keyId) {
  var primaryUser = this.getPrimaryUser();
  if (primaryUser && isValidSigningKeyPacket(this.primaryKey, primaryUser.selfCertificate) && (!keyId || this.primaryKey.getKeyId
().equals(keyId))) {
    return this.primaryKey;
  }
  if (this.subKeys) {
    for (var i = 0; i < this.subKeys.length; i++) {
      if (this.subKeys[i].isValidSigningKey(this.primaryKey) && (!keyId || this.subKeys[i].subKey.getKeyId().equals(keyId))) {
        return this.subKeys[i].subKey;
      }
    }
  }
  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.getSubkeyPackets"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>getSubkeyPackets ()](#apidoc.element.openpgp.key.Key.prototype.getSubkeyPackets)
- description and source-code
```javascript
getSubkeyPackets = function () {
  var subKeys = [];
  if (this.subKeys) {
    for (var i = 0; i < this.subKeys.length; i++) {
      subKeys.push(this.subKeys[i].subKey);
    }
  }
  return subKeys;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.getUserIds"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>getUserIds ()](#apidoc.element.openpgp.key.Key.prototype.getUserIds)
- description and source-code
```javascript
getUserIds = function () {
  var userids = [];
  for (var i = 0; i < this.users.length; i++) {
    if (this.users[i].userId) {
      userids.push(_util2.default.Uint8Array2str(this.users[i].userId.write()));
    }
  }
  return userids;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.isPrivate"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>isPrivate ()](#apidoc.element.openpgp.key.Key.prototype.isPrivate)
- description and source-code
```javascript
isPrivate = function () {
  return this.primaryKey.tag === _enums2.default.packet.secretKey;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.isPublic"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>isPublic ()](#apidoc.element.openpgp.key.Key.prototype.isPublic)
- description and source-code
```javascript
isPublic = function () {
  return this.primaryKey.tag === _enums2.default.packet.publicKey;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.packetlist2structure"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>packetlist2structure (packetlist)](#apidoc.element.openpgp.key.Key.prototype.packetlist2structure)
- description and source-code
```javascript
packetlist2structure = function (packetlist) {
  var user, primaryKeyId, subKey;
  for (var i = 0; i < packetlist.length; i++) {
    switch (packetlist[i].tag) {
      case _enums2.default.packet.publicKey:
      case _enums2.default.packet.secretKey:
        this.primaryKey = packetlist[i];
        primaryKeyId = this.primaryKey.getKeyId();
        break;
      case _enums2.default.packet.userid:
      case _enums2.default.packet.userAttribute:
        user = new User(packetlist[i]);
        if (!this.users) {
          this.users = [];
        }
        this.users.push(user);
        break;
      case _enums2.default.packet.publicSubkey:
      case _enums2.default.packet.secretSubkey:
        user = null;
        if (!this.subKeys) {
          this.subKeys = [];
        }
        subKey = new SubKey(packetlist[i]);
        this.subKeys.push(subKey);
        break;
      case _enums2.default.packet.signature:
        switch (packetlist[i].signatureType) {
          case _enums2.default.signature.cert_generic:
          case _enums2.default.signature.cert_persona:
          case _enums2.default.signature.cert_casual:
          case _enums2.default.signature.cert_positive:
            if (!user) {
              _util2.default.print_debug('Dropping certification signatures without preceding user packet');
              continue;
            }
            if (packetlist[i].issuerKeyId.equals(primaryKeyId)) {
              if (!user.selfCertifications) {
                user.selfCertifications = [];
              }
              user.selfCertifications.push(packetlist[i]);
            } else {
              if (!user.otherCertifications) {
                user.otherCertifications = [];
              }
              user.otherCertifications.push(packetlist[i]);
            }
            break;
          case _enums2.default.signature.cert_revocation:
            if (user) {
              if (!user.revocationCertifications) {
                user.revocationCertifications = [];
              }
              user.revocationCertifications.push(packetlist[i]);
            } else {
              if (!this.directSignatures) {
                this.directSignatures = [];
              }
              this.directSignatures.push(packetlist[i]);
            }
            break;
          case _enums2.default.signature.key:
            if (!this.directSignatures) {
              this.directSignatures = [];
            }
            this.directSignatures.push(packetlist[i]);
            break;
          case _enums2.default.signature.subkey_binding:
            if (!subKey) {
              _util2.default.print_debug('Dropping subkey binding signature without preceding subkey packet');
              continue;
            }
            subKey.bindingSignature = packetlist[i];
            break;
          case _enums2.default.signature.key_revocation:
            this.revocationSignature = packetlist[i];
            break;
          case _enums2.default.signature.subkey_revocation:
            if (!subKey) {
              _util2.default.print_debug('Dropping subkey revocation signature without preceding subkey packet');
              continue;
            }
            subKey.revocationSignature = packetlist[i];
            break;
        }
        break;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.revoke"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>revoke ()](#apidoc.element.openpgp.key.Key.prototype.revoke)
- description and source-code
```javascript
revoke = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.signAllUsers"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>signAllUsers (privateKeys)](#apidoc.element.openpgp.key.Key.prototype.signAllUsers)
- description and source-code
```javascript
signAllUsers = function (privateKeys) {
  var _this = this;

  var users = this.users.map(function (user) {
    return user.sign(_this.primaryKey, privateKeys);
  });
  var key = new Key(this.toPacketlist());
  key.users = users;
  return key;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.signPrimaryUser"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>signPrimaryUser (privateKeys)](#apidoc.element.openpgp.key.Key.prototype.signPrimaryUser)
- description and source-code
```javascript
signPrimaryUser = function (privateKeys) {
  var _ref = this.getPrimaryUser() || {};

  var index = _ref.index;
  var user = _ref.user;

  if (!user) {
    throw new Error('Could not find primary user');
  }
  user = user.sign(this.primaryKey, privateKeys);
  var key = new Key(this.toPacketlist());
  key.users[index] = user;
  return key;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.toPacketlist"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>toPacketlist ()](#apidoc.element.openpgp.key.Key.prototype.toPacketlist)
- description and source-code
```javascript
toPacketlist = function () {
  var packetlist = new _packet2.default.List();
  packetlist.push(this.primaryKey);
  packetlist.push(this.revocationSignature);
  packetlist.concat(this.directSignatures);
  var i;
  for (i = 0; i < this.users.length; i++) {
    packetlist.concat(this.users[i].toPacketlist());
  }
  if (this.subKeys) {
    for (i = 0; i < this.subKeys.length; i++) {
      packetlist.concat(this.subKeys[i].toPacketlist());
    }
  }
  return packetlist;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.toPublic"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>toPublic ()](#apidoc.element.openpgp.key.Key.prototype.toPublic)
- description and source-code
```javascript
toPublic = function () {
  var packetlist = new _packet2.default.List();
  var keyPackets = this.toPacketlist();
  var bytes;
  for (var i = 0; i < keyPackets.length; i++) {
    switch (keyPackets[i].tag) {
      case _enums2.default.packet.secretKey:
        bytes = keyPackets[i].writePublicKey();
        var pubKeyPacket = new _packet2.default.PublicKey();
        pubKeyPacket.read(bytes);
        packetlist.push(pubKeyPacket);
        break;
      case _enums2.default.packet.secretSubkey:
        bytes = keyPackets[i].writePublicKey();
        var pubSubkeyPacket = new _packet2.default.PublicSubkey();
        pubSubkeyPacket.read(bytes);
        packetlist.push(pubSubkeyPacket);
        break;
      default:
        packetlist.push(keyPackets[i]);
    }
  }
  return new Key(packetlist);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.update"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>update (key)](#apidoc.element.openpgp.key.Key.prototype.update)
- description and source-code
```javascript
update = function (key) {
  var that = this;
  if (key.verifyPrimaryKey() === _enums2.default.keyStatus.invalid) {
    return;
  }
  if (this.primaryKey.getFingerprint() !== key.primaryKey.getFingerprint()) {
    throw new Error('Key update method: fingerprints of keys not equal');
  }
  if (this.isPublic() && key.isPrivate()) {
    // check for equal subkey packets
    var equal = (this.subKeys && this.subKeys.length) === (key.subKeys && key.subKeys.length) && (!this.subKeys || this.subKeys.
every(function (destSubKey) {
      return key.subKeys.some(function (srcSubKey) {
        return destSubKey.subKey.getFingerprint() === srcSubKey.subKey.getFingerprint();
      });
    }));
    if (!equal) {
      throw new Error('Cannot update public key with private key if subkey mismatch');
    }
    this.primaryKey = key.primaryKey;
  }
  // revocation signature
  if (!this.revocationSignature && key.revocationSignature && !key.revocationSignature.isExpired() && (key.revocationSignature.verified
 || key.revocationSignature.verify(key.primaryKey, { key: key.primaryKey }))) {
    this.revocationSignature = key.revocationSignature;
  }
  // direct signatures
  mergeSignatures(key, this, 'directSignatures');
  // users
  key.users.forEach(function (srcUser) {
    var found = false;
    for (var i = 0; i < that.users.length; i++) {
      if (srcUser.userId && srcUser.userId.userid === that.users[i].userId.userid || srcUser.userAttribute && srcUser.userAttribute
.equals(that.users[i].userAttribute)) {
        that.users[i].update(srcUser, that.primaryKey);
        found = true;
        break;
      }
    }
    if (!found) {
      that.users.push(srcUser);
    }
  });
  // subkeys
  if (key.subKeys) {
    key.subKeys.forEach(function (srcSubKey) {
      var found = false;
      for (var i = 0; i < that.subKeys.length; i++) {
        if (srcSubKey.subKey.getFingerprint() === that.subKeys[i].subKey.getFingerprint()) {
          that.subKeys[i].update(srcSubKey, that.primaryKey);
          found = true;
          break;
        }
      }
      if (!found) {
        that.subKeys.push(srcSubKey);
      }
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.verifyAllUsers"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>verifyAllUsers (keys)](#apidoc.element.openpgp.key.Key.prototype.verifyAllUsers)
- description and source-code
```javascript
verifyAllUsers = function (keys) {
  var _this2 = this;

  return this.users.reduce(function (signatures, user) {
    return signatures.concat(user.verifyAllSignatures(_this2.primaryKey, keys).map(function (signature) {
      return {
        userid: user.userId.userid,
        keyid: signature.keyid,
        valid: signature.valid
      };
    }));
  }, []);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.verifyPrimaryKey"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>verifyPrimaryKey ()](#apidoc.element.openpgp.key.Key.prototype.verifyPrimaryKey)
- description and source-code
```javascript
verifyPrimaryKey = function () {
  // check revocation signature
  if (this.revocationSignature && !this.revocationSignature.isExpired() && (this.revocationSignature.verified || this.revocationSignature
.verify(this.primaryKey, { key: this.primaryKey }))) {
    return _enums2.default.keyStatus.revoked;
  }
  // check V3 expiration time
  if (this.primaryKey.version === 3 && this.primaryKey.expirationTimeV3 !== 0 && Date.now() > this.primaryKey.created.getTime() +
this.primaryKey.expirationTimeV3 * 24 * 3600 * 1000) {
    return _enums2.default.keyStatus.expired;
  }
  // check for at least one self signature. Self signature of user ID not mandatory
  // See {@link http://tools.ietf.org/html/rfc4880#section-11.1}
  var selfSigned = false;
  for (var i = 0; i < this.users.length; i++) {
    if (this.users[i].userId && this.users[i].selfCertifications) {
      selfSigned = true;
    }
  }
  if (!selfSigned) {
    return _enums2.default.keyStatus.no_self_cert;
  }
  // check for valid self signature
  var primaryUser = this.getPrimaryUser();
  if (!primaryUser) {
    return _enums2.default.keyStatus.invalid;
  }
  // check V4 expiration time
  if (this.primaryKey.version === 4 && primaryUser.selfCertificate.keyNeverExpires === false && Date.now() > this.primaryKey.created
.getTime() + primaryUser.selfCertificate.keyExpirationTime * 1000) {
    return _enums2.default.keyStatus.expired;
  }
  return _enums2.default.keyStatus.valid;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.key.Key.prototype.verifyPrimaryUser"></a>[function <span class="apidocSignatureSpan">openpgp.key.Key.prototype.</span>verifyPrimaryUser (keys)](#apidoc.element.openpgp.key.Key.prototype.verifyPrimaryUser)
- description and source-code
```javascript
verifyPrimaryUser = function (keys) {
  var _ref2 = this.getPrimaryUser() || {};

  var user = _ref2.user;

  if (!user) {
    throw new Error('Could not find primary user');
  }
  return user.verifyAllSignatures(this.primaryKey, keys);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.message"></a>[module openpgp.message](#apidoc.module.openpgp.message)

#### <a name="apidoc.element.openpgp.message.Message"></a>[function <span class="apidocSignatureSpan">openpgp.message.</span>Message (packetlist)](#apidoc.element.openpgp.message.Message)
- description and source-code
```javascript
function Message(packetlist) {
  if (!(this instanceof Message)) {
    return new Message(packetlist);
  }
  this.packets = packetlist || new _packet2.default.List();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.message.encryptSessionKey"></a>[function <span class="apidocSignatureSpan">openpgp.message.</span>encryptSessionKey (sessionKey, symAlgo, publicKeys, passwords)](#apidoc.element.openpgp.message.encryptSessionKey)
- description and source-code
```javascript
function encryptSessionKey(sessionKey, symAlgo, publicKeys, passwords) {
  var packetlist = new _packet2.default.List();

  if (publicKeys) {
    publicKeys.forEach(function (key) {
      var encryptionKeyPacket = key.getEncryptionKeyPacket();
      if (encryptionKeyPacket) {
        var pkESKeyPacket = new _packet2.default.PublicKeyEncryptedSessionKey();
        pkESKeyPacket.publicKeyId = encryptionKeyPacket.getKeyId();
        pkESKeyPacket.publicKeyAlgorithm = encryptionKeyPacket.algorithm;
        pkESKeyPacket.sessionKey = sessionKey;
        pkESKeyPacket.sessionKeyAlgorithm = symAlgo;
        pkESKeyPacket.encrypt(encryptionKeyPacket);
        delete pkESKeyPacket.sessionKey; // delete plaintext session key after encryption
        packetlist.push(pkESKeyPacket);
      } else {
        throw new Error('Could not find valid key packet for encryption in key ' + key.primaryKey.getKeyId().toHex());
      }
    });
  }

  if (passwords) {
    passwords.forEach(function (password) {
      var symEncryptedSessionKeyPacket = new _packet2.default.SymEncryptedSessionKey();
      symEncryptedSessionKeyPacket.sessionKey = sessionKey;
      symEncryptedSessionKeyPacket.sessionKeyAlgorithm = symAlgo;
      symEncryptedSessionKeyPacket.encrypt(password);
      delete symEncryptedSessionKeyPacket.sessionKey; // delete plaintext session key after encryption
      packetlist.push(symEncryptedSessionKeyPacket);
    });
  }

  return new Message(packetlist);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.message.fromBinary"></a>[function <span class="apidocSignatureSpan">openpgp.message.</span>fromBinary (bytes, filename)](#apidoc.element.openpgp.message.fromBinary)
- description and source-code
```javascript
function fromBinary(bytes, filename) {
  if (!_util2.default.isUint8Array(bytes)) {
    throw new Error('Data must be in the form of a Uint8Array');
  }

  var literalDataPacket = new _packet2.default.Literal();
  if (filename) {
    literalDataPacket.setFilename(filename);
  }
  literalDataPacket.setBytes(bytes, _enums2.default.read(_enums2.default.literal, _enums2.default.literal.binary));
  if (filename !== undefined) {
    literalDataPacket.setFilename(filename);
  }
  var literalDataPacketlist = new _packet2.default.List();
  literalDataPacketlist.push(literalDataPacket);
  return new Message(literalDataPacketlist);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.message.fromText"></a>[function <span class="apidocSignatureSpan">openpgp.message.</span>fromText (text, filename)](#apidoc.element.openpgp.message.fromText)
- description and source-code
```javascript
function fromText(text, filename) {
  var literalDataPacket = new _packet2.default.Literal();
  // text will be converted to UTF8
  literalDataPacket.setText(text);
  if (filename !== undefined) {
    literalDataPacket.setFilename(filename);
  }
  var literalDataPacketlist = new _packet2.default.List();
  literalDataPacketlist.push(literalDataPacket);
  return new Message(literalDataPacketlist);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.message.read"></a>[function <span class="apidocSignatureSpan">openpgp.message.</span>read (input)](#apidoc.element.openpgp.message.read)
- description and source-code
```javascript
function read(input) {
  var packetlist = new _packet2.default.List();
  packetlist.read(input);
  return new Message(packetlist);
}
```
- example usage
```shell
...
openpgp.encrypt(options).then(function(ciphertext) {
    encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
...
```

#### <a name="apidoc.element.openpgp.message.readArmored"></a>[function <span class="apidocSignatureSpan">openpgp.message.</span>readArmored (armoredText)](#apidoc.element.openpgp.message.readArmored)
- description and source-code
```javascript
function readArmored(armoredText) {
  //TODO how do we want to handle bad text? Exception throwing
  //TODO don't accept non-message armored texts
  var input = _armor2.default.decode(armoredText).data;
  return read(input);
}
```
- example usage
```shell
...
'''js
var options, encrypted;

var pubkey = '-----BEGIN PGP PUBLIC KEY BLOCK ... END PGP PUBLIC KEY BLOCK-----';
var privkey = '-----BEGIN PGP PRIVATE KEY BLOCK ... END PGP PRIVATE KEY BLOCK-----'; //encrypted private key
var passphrase = 'secret passphrase'; //what the privKey is encrypted with

var privKeyObj = openpgp.key.readArmored(privkey).keys[0];
privKeyObj.decrypt(passphrase);

options = {
    data: 'Hello, World!',                             // input as String (or Uint8Array)
    publicKeys: openpgp.key.readArmored(pubkey).keys,  // for encryption
    privateKeys: privKeyObj // for signing (optional)
};
...
```

#### <a name="apidoc.element.openpgp.message.readSignedContent"></a>[function <span class="apidocSignatureSpan">openpgp.message.</span>readSignedContent (content, detachedSignature)](#apidoc.element.openpgp.message.readSignedContent)
- description and source-code
```javascript
function readSignedContent(content, detachedSignature) {
  var literalDataPacket = new _packet2.default.Literal();
  literalDataPacket.setBytes(_util2.default.str2Uint8Array(content), _enums2.default.read(_enums2.default.literal, _enums2.default
.literal.binary));
  var packetlist = new _packet2.default.List();
  packetlist.push(literalDataPacket);
  var input = _armor2.default.decode(detachedSignature).data;
  packetlist.read(input);
  return new Message(packetlist);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.message.Message"></a>[module openpgp.message.Message](#apidoc.module.openpgp.message.Message)

#### <a name="apidoc.element.openpgp.message.Message.Message"></a>[function <span class="apidocSignatureSpan">openpgp.message.</span>Message (packetlist)](#apidoc.element.openpgp.message.Message.Message)
- description and source-code
```javascript
function Message(packetlist) {
  if (!(this instanceof Message)) {
    return new Message(packetlist);
  }
  this.packets = packetlist || new _packet2.default.List();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.message.Message.prototype"></a>[module openpgp.message.Message.prototype](#apidoc.module.openpgp.message.Message.prototype)

#### <a name="apidoc.element.openpgp.message.Message.prototype.armor"></a>[function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>armor ()](#apidoc.element.openpgp.message.Message.prototype.armor)
- description and source-code
```javascript
armor = function () {
  return _armor2.default.encode(_enums2.default.armor.message, this.packets.write());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.message.Message.prototype.decrypt"></a>[function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>decrypt (privateKey, sessionKey, password)](#apidoc.element.openpgp.message.Message.prototype.decrypt)
- description and source-code
```javascript
decrypt = function (privateKey, sessionKey, password) {
  var _this = this;

  return Promise.resolve().then(function () {
    var keyObj = sessionKey || _this.decryptSessionKey(privateKey, password);
    if (!keyObj || !_util2.default.isUint8Array(keyObj.data) || !_util2.default.isString(keyObj.algorithm)) {
      throw new Error('Invalid session key for decryption.');
    }

    var symEncryptedPacketlist = _this.packets.filterByTag(_enums2.default.packet.symmetricallyEncrypted, _enums2.default.packet
.symEncryptedIntegrityProtected, _enums2.default.packet.symEncryptedAEADProtected);

    if (symEncryptedPacketlist.length === 0) {
      return;
    }

    var symEncryptedPacket = symEncryptedPacketlist[0];
    return symEncryptedPacket.decrypt(keyObj.algorithm, keyObj.data).then(function () {
      var resultMsg = new Message(symEncryptedPacket.packets);
      symEncryptedPacket.packets = new _packet2.default.List(); // remove packets after decryption
      return resultMsg;
    });
  });
}
```
- example usage
```shell
...
'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
'''

#### Encrypt and decrypt *String* data with PGP keys

'''js
...
```

#### <a name="apidoc.element.openpgp.message.Message.prototype.decryptSessionKey"></a>[function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>decryptSessionKey (privateKey, password)](#apidoc.element.openpgp.message.Message.prototype.decryptSessionKey)
- description and source-code
```javascript
decryptSessionKey = function (privateKey, password) {
  var keyPacket;

  if (password) {
    var symEncryptedSessionKeyPacketlist = this.packets.filterByTag(_enums2.default.packet.symEncryptedSessionKey);
    var symLength = symEncryptedSessionKeyPacketlist.length;
    for (var i = 0; i < symLength; i++) {
      keyPacket = symEncryptedSessionKeyPacketlist[i];
      try {
        keyPacket.decrypt(password);
        break;
      } catch (err) {
        if (i === symLength - 1) {
          throw err;
        }
      }
    }
    if (!keyPacket) {
      throw new Error('No symmetrically encrypted session key packet found.');
    }
  } else if (privateKey) {
    var encryptionKeyIds = this.getEncryptionKeyIds();
    if (!encryptionKeyIds.length) {
      // nothing to decrypt
      return;
    }
    var privateKeyPacket = privateKey.getKeyPacket(encryptionKeyIds);
    if (!privateKeyPacket.isDecrypted) {
      throw new Error('Private key is not decrypted.');
    }
    var pkESKeyPacketlist = this.packets.filterByTag(_enums2.default.packet.publicKeyEncryptedSessionKey);
    for (var j = 0; j < pkESKeyPacketlist.length; j++) {
      if (pkESKeyPacketlist[j].publicKeyId.equals(privateKeyPacket.getKeyId())) {
        keyPacket = pkESKeyPacketlist[j];
        keyPacket.decrypt(privateKeyPacket);
        break;
      }
    }
  } else {
    throw new Error('No key or password specified.');
  }

  if (keyPacket) {
    return {
      data: keyPacket.sessionKey,
      algorithm: keyPacket.sessionKeyAlgorithm
    };
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.message.Message.prototype.encrypt"></a>[function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>encrypt (keys, passwords)](#apidoc.element.openpgp.message.Message.prototype.encrypt)
- description and source-code
```javascript
encrypt = function (keys, passwords) {
  var _this2 = this;

  var symAlgo = void 0,
      msg = void 0,
      symEncryptedPacket = void 0;
  return Promise.resolve().then(function () {
    if (keys) {
      symAlgo = keyModule.getPreferredSymAlgo(keys);
    } else if (passwords) {
      symAlgo = _config2.default.encryption_cipher;
    } else {
      throw new Error('No keys or passwords');
    }

    var sessionKey = _crypto2.default.generateSessionKey(_enums2.default.read(_enums2.default.symmetric, symAlgo));
    msg = encryptSessionKey(sessionKey, _enums2.default.read(_enums2.default.symmetric, symAlgo), keys, passwords);

    if (_config2.default.aead_protect) {
      symEncryptedPacket = new _packet2.default.SymEncryptedAEADProtected();
    } else if (_config2.default.integrity_protect) {
      symEncryptedPacket = new _packet2.default.SymEncryptedIntegrityProtected();
    } else {
      symEncryptedPacket = new _packet2.default.SymmetricallyEncrypted();
    }
    symEncryptedPacket.packets = _this2.packets;

    return symEncryptedPacket.encrypt(_enums2.default.read(_enums2.default.symmetric, symAlgo), sessionKey);
  }).then(function () {
    msg.packets.push(symEncryptedPacket);
    symEncryptedPacket.packets = new _packet2.default.List(); // remove packets after encryption
    return msg;
  });
}
```
- example usage
```shell
...

options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
...
```

#### <a name="apidoc.element.openpgp.message.Message.prototype.getEncryptionKeyIds"></a>[function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>getEncryptionKeyIds ()](#apidoc.element.openpgp.message.Message.prototype.getEncryptionKeyIds)
- description and source-code
```javascript
getEncryptionKeyIds = function () {
  var keyIds = [];
  var pkESKeyPacketlist = this.packets.filterByTag(_enums2.default.packet.publicKeyEncryptedSessionKey);
  pkESKeyPacketlist.forEach(function (packet) {
    keyIds.push(packet.publicKeyId);
  });
  return keyIds;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.message.Message.prototype.getFilename"></a>[function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>getFilename ()](#apidoc.element.openpgp.message.Message.prototype.getFilename)
- description and source-code
```javascript
getFilename = function () {
  var literal = this.packets.findPacket(_enums2.default.packet.literal);
  return literal && literal.getFilename() || null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.message.Message.prototype.getLiteralData"></a>[function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>getLiteralData ()](#apidoc.element.openpgp.message.Message.prototype.getLiteralData)
- description and source-code
```javascript
getLiteralData = function () {
  var literal = this.packets.findPacket(_enums2.default.packet.literal);
  return literal && literal.data || null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.message.Message.prototype.getSigningKeyIds"></a>[function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>getSigningKeyIds ()](#apidoc.element.openpgp.message.Message.prototype.getSigningKeyIds)
- description and source-code
```javascript
getSigningKeyIds = function () {
  var keyIds = [];
  var msg = this.unwrapCompressed();
  // search for one pass signatures
  var onePassSigList = msg.packets.filterByTag(_enums2.default.packet.onePassSignature);
  onePassSigList.forEach(function (packet) {
    keyIds.push(packet.signingKeyId);
  });
  // if nothing found look for signature packets
  if (!keyIds.length) {
    var signatureList = msg.packets.filterByTag(_enums2.default.packet.signature);
    signatureList.forEach(function (packet) {
      keyIds.push(packet.issuerKeyId);
    });
  }
  return keyIds;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.message.Message.prototype.getText"></a>[function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>getText ()](#apidoc.element.openpgp.message.Message.prototype.getText)
- description and source-code
```javascript
getText = function () {
  var literal = this.packets.findPacket(_enums2.default.packet.literal);
  if (literal) {
    return literal.getText();
  } else {
    return null;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.message.Message.prototype.sign"></a>[function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>sign ()](#apidoc.element.openpgp.message.Message.prototype.sign)
- description and source-code
```javascript
sign = function () {
  var privateKeys = arguments.length <= 0 || arguments[0] === undefined ? [] : arguments[0];
  var signature = arguments.length <= 1 || arguments[1] === undefined ? null : arguments[1];


  var packetlist = new _packet2.default.List();

  var literalDataPacket = this.packets.findPacket(_enums2.default.packet.literal);
  if (!literalDataPacket) {
    throw new Error('No literal data packet to sign.');
  }

  var literalFormat = _enums2.default.write(_enums2.default.literal, literalDataPacket.format);
  var signatureType = literalFormat === _enums2.default.literal.binary ? _enums2.default.signature.binary : _enums2.default.signature
.text;
  var i, signingKeyPacket, existingSigPacketlist, onePassSig;

  if (signature) {
    existingSigPacketlist = signature.packets.filterByTag(_enums2.default.packet.signature);
    if (existingSigPacketlist.length) {
      for (i = existingSigPacketlist.length - 1; i >= 0; i--) {
        var sigPacket = existingSigPacketlist[i];
        onePassSig = new _packet2.default.OnePassSignature();
        onePassSig.type = signatureType;
        onePassSig.hashAlgorithm = _config2.default.prefer_hash_algorithm;
        onePassSig.publicKeyAlgorithm = sigPacket.publicKeyAlgorithm;
        onePassSig.signingKeyId = sigPacket.issuerKeyId;
        if (!privateKeys.length && i === 0) {
          onePassSig.flags = 1;
        }
        packetlist.push(onePassSig);
      }
    }
  }
  for (i = 0; i < privateKeys.length; i++) {
    if (privateKeys[i].isPublic()) {
      throw new Error('Need private key for signing');
    }
    onePassSig = new _packet2.default.OnePassSignature();
    onePassSig.type = signatureType;
    //TODO get preferred hashg algo from key signature
    onePassSig.hashAlgorithm = _config2.default.prefer_hash_algorithm;
    signingKeyPacket = privateKeys[i].getSigningKeyPacket();
    if (!signingKeyPacket) {
      throw new Error('Could not find valid key packet for signing in key ' + privateKeys[i].primaryKey.getKeyId().toHex());
    }
    onePassSig.publicKeyAlgorithm = signingKeyPacket.algorithm;
    onePassSig.signingKeyId = signingKeyPacket.getKeyId();
    if (i === privateKeys.length - 1) {
      onePassSig.flags = 1;
    }
    packetlist.push(onePassSig);
  }

  packetlist.push(literalDataPacket);

  for (i = privateKeys.length - 1; i >= 0; i--) {
    var signaturePacket = new _packet2.default.Signature();
    signaturePacket.signatureType = signatureType;
    signaturePacket.hashAlgorithm = _config2.default.prefer_hash_algorithm;
    signaturePacket.publicKeyAlgorithm = signingKeyPacket.algorithm;
    if (!signingKeyPacket.isDecrypted) {
      throw new Error('Private key is not decrypted.');
    }
    signaturePacket.sign(signingKeyPacket, literalDataPacket);
    packetlist.push(signaturePacket);
  }

  if (signature) {
    packetlist.concat(existingSigPacketlist);
  }

  return new Message(packetlist);
}
```
- example usage
```shell
...

'''js
options = {
data: 'Hello, World!',                             // input as String (or Uint8Array)
privateKeys: privKeyObj // for signing
};

openpgp.sign(options).then(function(signed) {
cleartext = signed.data; // '-----BEGIN PGP SIGNED MESSAGE ... END PGP SIGNATURE-----'
});
'''

'''js
options = {
message: openpgp.cleartext.readArmored(cleartext), // parse armored message
...
```

#### <a name="apidoc.element.openpgp.message.Message.prototype.signDetached"></a>[function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>signDetached ()](#apidoc.element.openpgp.message.Message.prototype.signDetached)
- description and source-code
```javascript
signDetached = function () {
  var privateKeys = arguments.length <= 0 || arguments[0] === undefined ? [] : arguments[0];
  var signature = arguments.length <= 1 || arguments[1] === undefined ? null : arguments[1];


  var packetlist = new _packet2.default.List();

  var literalDataPacket = this.packets.findPacket(_enums2.default.packet.literal);
  if (!literalDataPacket) {
    throw new Error('No literal data packet to sign.');
  }

  var literalFormat = _enums2.default.write(_enums2.default.literal, literalDataPacket.format);
  var signatureType = literalFormat === _enums2.default.literal.binary ? _enums2.default.signature.binary : _enums2.default.signature
.text;

  for (var i = 0; i < privateKeys.length; i++) {
    var signingKeyPacket = privateKeys[i].getSigningKeyPacket();
    var signaturePacket = new _packet2.default.Signature();
    signaturePacket.signatureType = signatureType;
    signaturePacket.hashAlgorithm = _config2.default.prefer_hash_algorithm;
    signaturePacket.publicKeyAlgorithm = signingKeyPacket.algorithm;
    if (!signingKeyPacket.isDecrypted) {
      throw new Error('Private key is not decrypted.');
    }
    signaturePacket.sign(signingKeyPacket, literalDataPacket);
    packetlist.push(signaturePacket);
  }
  if (signature) {
    var existingSigPacketlist = signature.packets.filterByTag(_enums2.default.packet.signature);
    packetlist.concat(existingSigPacketlist);
  }

  return new sigModule.Signature(packetlist);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.message.Message.prototype.unwrapCompressed"></a>[function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>unwrapCompressed ()](#apidoc.element.openpgp.message.Message.prototype.unwrapCompressed)
- description and source-code
```javascript
unwrapCompressed = function () {
  var compressed = this.packets.filterByTag(_enums2.default.packet.compressed);
  if (compressed.length) {
    return new Message(compressed[0].packets);
  } else {
    return this;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.message.Message.prototype.verify"></a>[function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>verify (keys)](#apidoc.element.openpgp.message.Message.prototype.verify)
- description and source-code
```javascript
verify = function (keys) {
  var msg = this.unwrapCompressed();
  var literalDataList = msg.packets.filterByTag(_enums2.default.packet.literal);
  if (literalDataList.length !== 1) {
    throw new Error('Can only verify message with one literal data packet.');
  }
  var signatureList = msg.packets.filterByTag(_enums2.default.packet.signature);
  return createVerificationObjects(signatureList, literalDataList, keys);
}
```
- example usage
```shell
...

'''js
options = {
    message: openpgp.cleartext.readArmored(cleartext), // parse armored message
    publicKeys: openpgp.key.readArmored(pubkey).keys   // for verification
};

openpgp.verify(options).then(function(verified) {
	validity = verified.signatures[0].valid; // true
	if (validity) {
		console.log('signed by key id ' + verified.signatures[0].keyid.toHex());
	}
});
'''
...
```

#### <a name="apidoc.element.openpgp.message.Message.prototype.verifyDetached"></a>[function <span class="apidocSignatureSpan">openpgp.message.Message.prototype.</span>verifyDetached (signature, keys)](#apidoc.element.openpgp.message.Message.prototype.verifyDetached)
- description and source-code
```javascript
verifyDetached = function (signature, keys) {
  var msg = this.unwrapCompressed();
  var literalDataList = msg.packets.filterByTag(_enums2.default.packet.literal);
  if (literalDataList.length !== 1) {
    throw new Error('Can only verify message with one literal data packet.');
  }
  var signatureList = signature.packets;
  return createVerificationObjects(signatureList, literalDataList, keys);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet"></a>[module openpgp.packet](#apidoc.module.openpgp.packet)

#### <a name="apidoc.element.openpgp.packet.Compressed"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>Compressed ()](#apidoc.element.openpgp.packet.Compressed)
- description and source-code
```javascript
function Compressed() {
<span class="apidocCodeCommentSpan">  /**
   * Packet type
   * @type {module:enums.packet}
   */
</span>  this.tag = _enums2.default.packet.compressed;
  /**
   * List of packets
   * @type {module:packet/packetlist}
   */
  this.packets = null;
  /**
   * Compression algorithm
   * @type {compression}
   */
  this.algorithm = 'zip';

  /**
   * Compressed packet data
   * @type {String}
   */
  this.compressed = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.List"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>List ()](#apidoc.element.openpgp.packet.List)
- description and source-code
```javascript
function Packetlist() {
<span class="apidocCodeCommentSpan">  /** The number of packets contained within the list.
   * @readonly
   * @type {Integer} */
</span>  this.length = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Literal"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>Literal ()](#apidoc.element.openpgp.packet.Literal)
- description and source-code
```javascript
function Literal() {
  this.tag = _enums2.default.packet.literal;
  this.format = 'utf8'; // default format for literal data packets
  this.date = new Date();
  this.data = new Uint8Array(0); // literal data representation
  this.filename = 'msg.txt';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Marker"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>Marker ()](#apidoc.element.openpgp.packet.Marker)
- description and source-code
```javascript
function Marker() {
  this.tag = _enums2.default.packet.marker;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.OnePassSignature"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>OnePassSignature ()](#apidoc.element.openpgp.packet.OnePassSignature)
- description and source-code
```javascript
function OnePassSignature() {
  this.tag = _enums2.default.packet.onePassSignature; // The packet type
  this.version = null; // A one-octet version number.  The current version is 3.
  this.type = null; // A one-octet signature type.  Signature types are described in {@link http://tools.ietf.org/html/rfc4880#section
-5.2.1|RFC4880 Section 5.2.1}.
  this.hashAlgorithm = null; // A one-octet number describing the hash algorithm used. (See {@link http://tools.ietf.org/html/rfc4880
#section-9.4|RFC4880 9.4})
  this.publicKeyAlgorithm = null; // A one-octet number describing the public-key algorithm used. (See {@link http://tools.ietf.
org/html/rfc4880#section-9.1|RFC4880 9.1})
  this.signingKeyId = null; // An eight-octet number holding the Key ID of the signing key.
  this.flags = null; //  A one-octet number holding a flag showing whether the signature is nested.  A zero value indicates that
 the next packet is another One-Pass Signature packet that describes another signature to be applied to the same message data.
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.PublicKey"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>PublicKey ()](#apidoc.element.openpgp.packet.PublicKey)
- description and source-code
```javascript
function PublicKey() {
  this.tag = _enums2.default.packet.publicKey;
  this.version = 4;
<span class="apidocCodeCommentSpan">  /** Key creation date.
   * @type {Date} */
</span>  this.created = new Date();
  /** A list of multiprecision integers
   * @type {module:type/mpi} */
  this.mpi = [];
  /** Public key algorithm
   * @type {module:enums.publicKey} */
  this.algorithm = 'rsa_sign';
  // time in days (V3 only)
  this.expirationTimeV3 = 0;
  /**
   * Fingerprint in lowercase hex
   * @type {String}
   */
  this.fingerprint = null;
  /**
   * Keyid
   * @type {module:type/keyid}
   */
  this.keyid = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>PublicKeyEncryptedSessionKey ()](#apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey)
- description and source-code
```javascript
function PublicKeyEncryptedSessionKey() {
  this.tag = _enums2.default.packet.publicKeyEncryptedSessionKey;
  this.version = 3;

  this.publicKeyId = new _keyid2.default();
  this.publicKeyAlgorithm = 'rsa_encrypt';

  this.sessionKey = null;
  this.sessionKeyAlgorithm = 'aes256';

<span class="apidocCodeCommentSpan">  /** @type {Array<module:type/mpi>} */
</span>  this.encrypted = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.PublicSubkey"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>PublicSubkey ()](#apidoc.element.openpgp.packet.PublicSubkey)
- description and source-code
```javascript
function PublicSubkey() {
  _public_key2.default.call(this);
  this.tag = _enums2.default.packet.publicSubkey;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.SecretKey"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>SecretKey ()](#apidoc.element.openpgp.packet.SecretKey)
- description and source-code
```javascript
function SecretKey() {
  _public_key2.default.call(this);
  this.tag = _enums2.default.packet.secretKey;
  // encrypted secret-key data
  this.encrypted = null;
  // indicator if secret-key data is available in decrypted form
  this.isDecrypted = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.SecretSubkey"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>SecretSubkey ()](#apidoc.element.openpgp.packet.SecretSubkey)
- description and source-code
```javascript
function SecretSubkey() {
  _secret_key2.default.call(this);
  this.tag = _enums2.default.packet.secretSubkey;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Signature"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>Signature ()](#apidoc.element.openpgp.packet.Signature)
- description and source-code
```javascript
function Signature() {
  this.tag = _enums2.default.packet.signature;
  this.version = 4;
  this.signatureType = null;
  this.hashAlgorithm = null;
  this.publicKeyAlgorithm = null;

  this.signatureData = null;
  this.unhashedSubpackets = null;
  this.signedHashValue = null;

  this.created = new Date();
  this.signatureExpirationTime = null;
  this.signatureNeverExpires = true;
  this.exportable = null;
  this.trustLevel = null;
  this.trustAmount = null;
  this.regularExpression = null;
  this.revocable = null;
  this.keyExpirationTime = null;
  this.keyNeverExpires = null;
  this.preferredSymmetricAlgorithms = null;
  this.revocationKeyClass = null;
  this.revocationKeyAlgorithm = null;
  this.revocationKeyFingerprint = null;
  this.issuerKeyId = new _keyid2.default();
  this.notation = null;
  this.preferredHashAlgorithms = null;
  this.preferredCompressionAlgorithms = null;
  this.keyServerPreferences = null;
  this.preferredKeyServer = null;
  this.isPrimaryUserID = null;
  this.policyURI = null;
  this.keyFlags = null;
  this.signersUserId = null;
  this.reasonForRevocationFlag = null;
  this.reasonForRevocationString = null;
  this.features = null;
  this.signatureTargetPublicKeyAlgorithm = null;
  this.signatureTargetHashAlgorithm = null;
  this.signatureTargetHash = null;
  this.embeddedSignature = null;

  this.verified = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.SymEncryptedAEADProtected"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>SymEncryptedAEADProtected ()](#apidoc.element.openpgp.packet.SymEncryptedAEADProtected)
- description and source-code
```javascript
function SymEncryptedAEADProtected() {
  this.tag = _enums2.default.packet.symEncryptedAEADProtected;
  this.version = VERSION;
  this.iv = null;
  this.encrypted = null;
  this.packets = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.SymEncryptedIntegrityProtected"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>SymEncryptedIntegrityProtected ()](#apidoc.element.openpgp.packet.SymEncryptedIntegrityProtected)
- description and source-code
```javascript
function SymEncryptedIntegrityProtected() {
  this.tag = _enums2.default.packet.symEncryptedIntegrityProtected;
  this.version = VERSION;
<span class="apidocCodeCommentSpan">  /** The encrypted payload. */
</span>  this.encrypted = null; // string
  /**
   * If after decrypting the packet this is set to true,
   * a modification has been detected and thus the contents
   * should be discarded.
   * @type {Boolean}
   */
  this.modification = false;
  this.packets = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.SymEncryptedSessionKey"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>SymEncryptedSessionKey ()](#apidoc.element.openpgp.packet.SymEncryptedSessionKey)
- description and source-code
```javascript
function SymEncryptedSessionKey() {
  this.tag = _enums2.default.packet.symEncryptedSessionKey;
  this.version = 4;
  this.sessionKey = null;
  this.sessionKeyEncryptionAlgorithm = null;
  this.sessionKeyAlgorithm = 'aes256';
  this.encrypted = null;
  this.s2k = new _s2k2.default();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.SymmetricallyEncrypted"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>SymmetricallyEncrypted ()](#apidoc.element.openpgp.packet.SymmetricallyEncrypted)
- description and source-code
```javascript
function SymmetricallyEncrypted() {
  this.tag = _enums2.default.packet.symmetricallyEncrypted;
  this.encrypted = null;
<span class="apidocCodeCommentSpan">  /** Decrypted packets contained within.
   * @type {module:packet/packetlist} */
</span>  this.packets = null;
  this.ignore_mdc_error = _config2.default.ignore_mdc_error;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Trust"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>Trust ()](#apidoc.element.openpgp.packet.Trust)
- description and source-code
```javascript
function Trust() {
  this.tag = _enums2.default.packet.trust;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.UserAttribute"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>UserAttribute ()](#apidoc.element.openpgp.packet.UserAttribute)
- description and source-code
```javascript
function UserAttribute() {
  this.tag = _enums2.default.packet.userAttribute;
  this.attributes = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Userid"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>Userid ()](#apidoc.element.openpgp.packet.Userid)
- description and source-code
```javascript
function Userid() {
  this.tag = _enums2.default.packet.userid;
<span class="apidocCodeCommentSpan">  /** A string containing the user id. Usually in the form
   * John Doe <john@example.com>
   * @type {String}
   */
</span>  this.userid = '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.fromStructuredClone"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>fromStructuredClone (packetClone)](#apidoc.element.openpgp.packet.fromStructuredClone)
- description and source-code
```javascript
function fromStructuredClone(packetClone) {
  var tagName = _enums2.default.read(_enums2.default.packet, packetClone.tag);
  var packet = newPacketFromTag(tagName);
  for (var attr in packetClone) {
    if (packetClone.hasOwnProperty(attr)) {
      packet[attr] = packetClone[attr];
    }
  }
  if (packet.postCloneTypeFix) {
    packet.postCloneTypeFix();
  }
  return packet;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.newPacketFromTag"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>newPacketFromTag (tag)](#apidoc.element.openpgp.packet.newPacketFromTag)
- description and source-code
```javascript
function newPacketFromTag(tag) {
  return new packets[packetClassFromTagName(tag)]();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet.Compressed"></a>[module openpgp.packet.Compressed](#apidoc.module.openpgp.packet.Compressed)

#### <a name="apidoc.element.openpgp.packet.Compressed.Compressed"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>Compressed ()](#apidoc.element.openpgp.packet.Compressed.Compressed)
- description and source-code
```javascript
function Compressed() {
<span class="apidocCodeCommentSpan">  /**
   * Packet type
   * @type {module:enums.packet}
   */
</span>  this.tag = _enums2.default.packet.compressed;
  /**
   * List of packets
   * @type {module:packet/packetlist}
   */
  this.packets = null;
  /**
   * Compression algorithm
   * @type {compression}
   */
  this.algorithm = 'zip';

  /**
   * Compressed packet data
   * @type {String}
   */
  this.compressed = null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet.Compressed.prototype"></a>[module openpgp.packet.Compressed.prototype](#apidoc.module.openpgp.packet.Compressed.prototype)

#### <a name="apidoc.element.openpgp.packet.Compressed.prototype.compress"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Compressed.prototype.</span>compress ()](#apidoc.element.openpgp.packet.Compressed.prototype.compress)
- description and source-code
```javascript
compress = function () {
  var uncompressed, deflate;
  uncompressed = this.packets.write();

  switch (this.algorithm) {

    case 'uncompressed':
      // - Uncompressed
      this.compressed = uncompressed;
      break;

    case 'zip':
      // - ZIP [RFC1951]
      deflate = new _rawdeflateMin2.default.Zlib.RawDeflate(uncompressed);
      this.compressed = deflate.compress();
      break;

    case 'zlib':
      // - ZLIB [RFC1950]
      deflate = new _zlibMin2.default.Zlib.Deflate(uncompressed);
      this.compressed = deflate.compress();
      break;

    case 'bzip2':
      //  - BZip2 [BZ2]
      // TODO: need to implement this
      throw new Error("Compression algorithm BZip2 [BZ2] is not implemented.");

    default:
      throw new Error("Compression algorithm unknown :" + this.type);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Compressed.prototype.decompress"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Compressed.prototype.</span>decompress ()](#apidoc.element.openpgp.packet.Compressed.prototype.decompress)
- description and source-code
```javascript
decompress = function () {
  var decompressed, inflate;

  switch (this.algorithm) {
    case 'uncompressed':
      decompressed = this.compressed;
      break;

    case 'zip':
      inflate = new _rawinflateMin2.default.Zlib.RawInflate(this.compressed);
      decompressed = inflate.decompress();
      break;

    case 'zlib':
      inflate = new _zlibMin2.default.Zlib.Inflate(this.compressed);
      decompressed = inflate.decompress();
      break;

    case 'bzip2':
      // TODO: need to implement this
      throw new Error('Compression algorithm BZip2 [BZ2] is not implemented.');

    default:
      throw new Error("Compression algorithm unknown :" + this.algorithm);
  }

  this.packets.read(decompressed);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Compressed.prototype.read"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Compressed.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.Compressed.prototype.read)
- description and source-code
```javascript
read = function (bytes) {
  // One octet that gives the algorithm used to compress the packet.
  this.algorithm = _enums2.default.read(_enums2.default.compression, bytes[0]);

  // Compressed data, which makes up the remainder of the packet.
  this.compressed = bytes.subarray(1, bytes.length);

  this.decompress();
}
```
- example usage
```shell
...
openpgp.encrypt(options).then(function(ciphertext) {
    encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
...
```

#### <a name="apidoc.element.openpgp.packet.Compressed.prototype.write"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Compressed.prototype.</span>write ()](#apidoc.element.openpgp.packet.Compressed.prototype.write)
- description and source-code
```javascript
write = function () {
  if (this.compressed === null) {
    this.compress();
  }

  return _util2.default.concatUint8Array(new Uint8Array([_enums2.default.write(_enums2.default.compression, this.algorithm)]), this
.compressed);
}
```
- example usage
```shell
...
options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
password: 'secret stuff',                 // decrypt with password
...
```



# <a name="apidoc.module.openpgp.packet.List"></a>[module openpgp.packet.List](#apidoc.module.openpgp.packet.List)

#### <a name="apidoc.element.openpgp.packet.List.List"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>List ()](#apidoc.element.openpgp.packet.List.List)
- description and source-code
```javascript
function Packetlist() {
<span class="apidocCodeCommentSpan">  /** The number of packets contained within the list.
   * @readonly
   * @type {Integer} */
</span>  this.length = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.List.fromStructuredClone"></a>[function <span class="apidocSignatureSpan">openpgp.packet.List.</span>fromStructuredClone (packetlistClone)](#apidoc.element.openpgp.packet.List.fromStructuredClone)
- description and source-code
```javascript
fromStructuredClone = function (packetlistClone) {
  var packetlist = new Packetlist();
  for (var i = 0; i < packetlistClone.length; i++) {
    packetlist.push(packets.fromStructuredClone(packetlistClone[i]));
    if (packetlist[i].packets.length !== 0) {
      packetlist[i].packets = this.fromStructuredClone(packetlist[i].packets);
    } else {
      packetlist[i].packets = new Packetlist();
    }
  }
  return packetlist;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet.List.prototype"></a>[module openpgp.packet.List.prototype](#apidoc.module.openpgp.packet.List.prototype)

#### <a name="apidoc.element.openpgp.packet.List.prototype.concat"></a>[function <span class="apidocSignatureSpan">openpgp.packet.List.prototype.</span>concat (packetlist)](#apidoc.element.openpgp.packet.List.prototype.concat)
- description and source-code
```javascript
concat = function (packetlist) {
  if (packetlist) {
    for (var i = 0; i < packetlist.length; i++) {
      this.push(packetlist[i]);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.List.prototype.filter"></a>[function <span class="apidocSignatureSpan">openpgp.packet.List.prototype.</span>filter (callback)](#apidoc.element.openpgp.packet.List.prototype.filter)
- description and source-code
```javascript
filter = function (callback) {

  var filtered = new Packetlist();

  for (var i = 0; i < this.length; i++) {
    if (callback(this[i], i, this)) {
      filtered.push(this[i]);
    }
  }

  return filtered;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.List.prototype.filterByTag"></a>[function <span class="apidocSignatureSpan">openpgp.packet.List.prototype.</span>filterByTag ()](#apidoc.element.openpgp.packet.List.prototype.filterByTag)
- description and source-code
```javascript
filterByTag = function () {
  var args = Array.prototype.slice.call(arguments);
  var filtered = new Packetlist();
  var that = this;

  function handle(packetType) {
    return that[i].tag === packetType;
  }
  for (var i = 0; i < this.length; i++) {
    if (args.some(handle)) {
      filtered.push(this[i]);
    }
  }

  return filtered;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.List.prototype.findPacket"></a>[function <span class="apidocSignatureSpan">openpgp.packet.List.prototype.</span>findPacket (type)](#apidoc.element.openpgp.packet.List.prototype.findPacket)
- description and source-code
```javascript
findPacket = function (type) {
  var packetlist = this.filterByTag(type);
  if (packetlist.length) {
    return packetlist[0];
  } else {
    var found = null;
    for (var i = 0; i < this.length; i++) {
      if (this[i].packets.length) {
        found = this[i].packets.findPacket(type);
        if (found) {
          return found;
        }
      }
    }
  }
  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.List.prototype.forEach"></a>[function <span class="apidocSignatureSpan">openpgp.packet.List.prototype.</span>forEach (callback)](#apidoc.element.openpgp.packet.List.prototype.forEach)
- description and source-code
```javascript
forEach = function (callback) {
  for (var i = 0; i < this.length; i++) {
    callback(this[i]);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.List.prototype.indexOfTag"></a>[function <span class="apidocSignatureSpan">openpgp.packet.List.prototype.</span>indexOfTag ()](#apidoc.element.openpgp.packet.List.prototype.indexOfTag)
- description and source-code
```javascript
indexOfTag = function () {
  var args = Array.prototype.slice.call(arguments);
  var tagIndex = [];
  var that = this;

  function handle(packetType) {
    return that[i].tag === packetType;
  }
  for (var i = 0; i < this.length; i++) {
    if (args.some(handle)) {
      tagIndex.push(i);
    }
  }
  return tagIndex;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.List.prototype.pop"></a>[function <span class="apidocSignatureSpan">openpgp.packet.List.prototype.</span>pop ()](#apidoc.element.openpgp.packet.List.prototype.pop)
- description and source-code
```javascript
pop = function () {
  if (this.length === 0) {
    return;
  }

  var packet = this[this.length - 1];
  delete this[this.length - 1];
  this.length--;

  return packet;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.List.prototype.push"></a>[function <span class="apidocSignatureSpan">openpgp.packet.List.prototype.</span>push (packet)](#apidoc.element.openpgp.packet.List.prototype.push)
- description and source-code
```javascript
push = function (packet) {
  if (!packet) {
    return;
  }

  packet.packets = packet.packets || new Packetlist();

  this[this.length] = packet;
  this.length++;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.List.prototype.read"></a>[function <span class="apidocSignatureSpan">openpgp.packet.List.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.List.prototype.read)
- description and source-code
```javascript
read = function (bytes) {
  var i = 0;

  while (i < bytes.length) {
    var parsed = _packet2.default.read(bytes, i, bytes.length - i);
    i = parsed.offset;

    var pushed = false;
    try {
      var tag = _enums2.default.read(_enums2.default.packet, parsed.tag);
      var packet = packets.newPacketFromTag(tag);
      this.push(packet);
      pushed = true;
      packet.read(parsed.packet);
    } catch (e) {
      if (!_config2.default.tolerant || parsed.tag == _enums2.default.packet.symmetricallyEncrypted || parsed.tag == _enums2.default
.packet.literal || parsed.tag == _enums2.default.packet.compressed) {
        throw e;
      }
      if (pushed) {
        this.pop(); // drop unsupported packet
      }
    }
  }
}
```
- example usage
```shell
...
openpgp.encrypt(options).then(function(ciphertext) {
    encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
...
```

#### <a name="apidoc.element.openpgp.packet.List.prototype.slice"></a>[function <span class="apidocSignatureSpan">openpgp.packet.List.prototype.</span>slice (begin, end)](#apidoc.element.openpgp.packet.List.prototype.slice)
- description and source-code
```javascript
slice = function (begin, end) {
  if (!end) {
    end = this.length;
  }
  var part = new Packetlist();
  for (var i = begin; i < end; i++) {
    part.push(this[i]);
  }
  return part;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.List.prototype.write"></a>[function <span class="apidocSignatureSpan">openpgp.packet.List.prototype.</span>write ()](#apidoc.element.openpgp.packet.List.prototype.write)
- description and source-code
```javascript
write = function () {
  var arr = [];

  for (var i = 0; i < this.length; i++) {
    var packetbytes = this[i].write();
    arr.push(_packet2.default.writeHeader(this[i].tag, packetbytes.length));
    arr.push(packetbytes);
  }

  return _util2.default.concatUint8Array(arr);
}
```
- example usage
```shell
...
options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
password: 'secret stuff',                 // decrypt with password
...
```



# <a name="apidoc.module.openpgp.packet.Literal"></a>[module openpgp.packet.Literal](#apidoc.module.openpgp.packet.Literal)

#### <a name="apidoc.element.openpgp.packet.Literal.Literal"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>Literal ()](#apidoc.element.openpgp.packet.Literal.Literal)
- description and source-code
```javascript
function Literal() {
  this.tag = _enums2.default.packet.literal;
  this.format = 'utf8'; // default format for literal data packets
  this.date = new Date();
  this.data = new Uint8Array(0); // literal data representation
  this.filename = 'msg.txt';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet.Literal.prototype"></a>[module openpgp.packet.Literal.prototype](#apidoc.module.openpgp.packet.Literal.prototype)

#### <a name="apidoc.element.openpgp.packet.Literal.prototype.getBytes"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Literal.prototype.</span>getBytes ()](#apidoc.element.openpgp.packet.Literal.prototype.getBytes)
- description and source-code
```javascript
getBytes = function () {
  return this.data;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Literal.prototype.getFilename"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Literal.prototype.</span>getFilename ()](#apidoc.element.openpgp.packet.Literal.prototype.getFilename)
- description and source-code
```javascript
getFilename = function () {
  return this.filename;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Literal.prototype.getText"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Literal.prototype.</span>getText ()](#apidoc.element.openpgp.packet.Literal.prototype.getText)
- description and source-code
```javascript
getText = function () {
  // decode UTF8
  var text = _util2.default.decode_utf8(_util2.default.Uint8Array2str(this.data));
  // normalize EOL to \n
  return text.replace(/\r\n/g, '\n');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Literal.prototype.read"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Literal.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.Literal.prototype.read)
- description and source-code
```javascript
read = function (bytes) {
  // - A one-octet field that describes how the data is formatted.
  var format = _enums2.default.read(_enums2.default.literal, bytes[0]);

  var filename_len = bytes[1];
  this.filename = _util2.default.decode_utf8(_util2.default.Uint8Array2str(bytes.subarray(2, 2 + filename_len)));

  this.date = _util2.default.readDate(bytes.subarray(2 + filename_len, 2 + filename_len + 4));

  var data = bytes.subarray(6 + filename_len, bytes.length);

  this.setBytes(data, format);
}
```
- example usage
```shell
...
openpgp.encrypt(options).then(function(ciphertext) {
    encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
...
```

#### <a name="apidoc.element.openpgp.packet.Literal.prototype.setBytes"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Literal.prototype.</span>setBytes (bytes, format)](#apidoc.element.openpgp.packet.Literal.prototype.setBytes)
- description and source-code
```javascript
setBytes = function (bytes, format) {
  this.format = format;
  this.data = bytes;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Literal.prototype.setFilename"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Literal.prototype.</span>setFilename (filename)](#apidoc.element.openpgp.packet.Literal.prototype.setFilename)
- description and source-code
```javascript
setFilename = function (filename) {
  this.filename = filename;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Literal.prototype.setText"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Literal.prototype.</span>setText (text)](#apidoc.element.openpgp.packet.Literal.prototype.setText)
- description and source-code
```javascript
setText = function (text) {
  // normalize EOL to \r\n
  text = text.replace(/\r\n/g, '\n').replace(/\r/g, '\n').replace(/\n/g, '\r\n');
  // encode UTF8
  this.data = this.format === 'utf8' ? _util2.default.str2Uint8Array(_util2.default.encode_utf8(text)) : _util2.default.str2Uint8Array
(text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Literal.prototype.write"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Literal.prototype.</span>write ()](#apidoc.element.openpgp.packet.Literal.prototype.write)
- description and source-code
```javascript
write = function () {
  var filename = _util2.default.str2Uint8Array(_util2.default.encode_utf8(this.filename));
  var filename_length = new Uint8Array([filename.length]);

  var format = new Uint8Array([_enums2.default.write(_enums2.default.literal, this.format)]);
  var date = _util2.default.writeDate(this.date);
  var data = this.getBytes();

  return _util2.default.concatUint8Array([format, filename_length, filename, date, data]);
}
```
- example usage
```shell
...
options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
password: 'secret stuff',                 // decrypt with password
...
```



# <a name="apidoc.module.openpgp.packet.Marker"></a>[module openpgp.packet.Marker](#apidoc.module.openpgp.packet.Marker)

#### <a name="apidoc.element.openpgp.packet.Marker.Marker"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>Marker ()](#apidoc.element.openpgp.packet.Marker.Marker)
- description and source-code
```javascript
function Marker() {
  this.tag = _enums2.default.packet.marker;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet.Marker.prototype"></a>[module openpgp.packet.Marker.prototype](#apidoc.module.openpgp.packet.Marker.prototype)

#### <a name="apidoc.element.openpgp.packet.Marker.prototype.read"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Marker.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.Marker.prototype.read)
- description and source-code
```javascript
read = function (bytes) {
  if (bytes[0] === 0x50 && // P
  bytes[1] === 0x47 && // G
  bytes[2] === 0x50) {
    // P
    return true;
  }
  // marker packet does not contain "PGP"
  return false;
}
```
- example usage
```shell
...
openpgp.encrypt(options).then(function(ciphertext) {
    encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
...
```



# <a name="apidoc.module.openpgp.packet.OnePassSignature"></a>[module openpgp.packet.OnePassSignature](#apidoc.module.openpgp.packet.OnePassSignature)

#### <a name="apidoc.element.openpgp.packet.OnePassSignature.OnePassSignature"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>OnePassSignature ()](#apidoc.element.openpgp.packet.OnePassSignature.OnePassSignature)
- description and source-code
```javascript
function OnePassSignature() {
  this.tag = _enums2.default.packet.onePassSignature; // The packet type
  this.version = null; // A one-octet version number.  The current version is 3.
  this.type = null; // A one-octet signature type.  Signature types are described in {@link http://tools.ietf.org/html/rfc4880#section
-5.2.1|RFC4880 Section 5.2.1}.
  this.hashAlgorithm = null; // A one-octet number describing the hash algorithm used. (See {@link http://tools.ietf.org/html/rfc4880
#section-9.4|RFC4880 9.4})
  this.publicKeyAlgorithm = null; // A one-octet number describing the public-key algorithm used. (See {@link http://tools.ietf.
org/html/rfc4880#section-9.1|RFC4880 9.1})
  this.signingKeyId = null; // An eight-octet number holding the Key ID of the signing key.
  this.flags = null; //  A one-octet number holding a flag showing whether the signature is nested.  A zero value indicates that
 the next packet is another One-Pass Signature packet that describes another signature to be applied to the same message data.
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet.OnePassSignature.prototype"></a>[module openpgp.packet.OnePassSignature.prototype](#apidoc.module.openpgp.packet.OnePassSignature.prototype)

#### <a name="apidoc.element.openpgp.packet.OnePassSignature.prototype.postCloneTypeFix"></a>[function <span class="apidocSignatureSpan">openpgp.packet.OnePassSignature.prototype.</span>postCloneTypeFix ()](#apidoc.element.openpgp.packet.OnePassSignature.prototype.postCloneTypeFix)
- description and source-code
```javascript
postCloneTypeFix = function () {
  this.signingKeyId = _keyid2.default.fromClone(this.signingKeyId);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.OnePassSignature.prototype.read"></a>[function <span class="apidocSignatureSpan">openpgp.packet.OnePassSignature.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.OnePassSignature.prototype.read)
- description and source-code
```javascript
read = function (bytes) {
  var mypos = 0;
  // A one-octet version number.  The current version is 3.
  this.version = bytes[mypos++];

  // A one-octet signature type.  Signature types are described in
  //   Section 5.2.1.
  this.type = _enums2.default.read(_enums2.default.signature, bytes[mypos++]);

  // A one-octet number describing the hash algorithm used.
  this.hashAlgorithm = _enums2.default.read(_enums2.default.hash, bytes[mypos++]);

  // A one-octet number describing the public-key algorithm used.
  this.publicKeyAlgorithm = _enums2.default.read(_enums2.default.publicKey, bytes[mypos++]);

  // An eight-octet number holding the Key ID of the signing key.
  this.signingKeyId = new _keyid2.default();
  this.signingKeyId.read(bytes.subarray(mypos, mypos + 8));
  mypos += 8;

  // A one-octet number holding a flag showing whether the signature
  //   is nested.  A zero value indicates that the next packet is
  //   another One-Pass Signature packet that describes another
  //   signature to be applied to the same message data.
  this.flags = bytes[mypos++];
  return this;
}
```
- example usage
```shell
...
openpgp.encrypt(options).then(function(ciphertext) {
    encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
...
```

#### <a name="apidoc.element.openpgp.packet.OnePassSignature.prototype.write"></a>[function <span class="apidocSignatureSpan">openpgp.packet.OnePassSignature.prototype.</span>write ()](#apidoc.element.openpgp.packet.OnePassSignature.prototype.write)
- description and source-code
```javascript
write = function () {

  var start = new Uint8Array([3, _enums2.default.write(_enums2.default.signature, this.type), _enums2.default.write(_enums2.default
.hash, this.hashAlgorithm), _enums2.default.write(_enums2.default.publicKey, this.publicKeyAlgorithm)]);

  var end = new Uint8Array([this.flags]);

  return _util2.default.concatUint8Array([start, this.signingKeyId.write(), end]);
}
```
- example usage
```shell
...
options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
password: 'secret stuff',                 // decrypt with password
...
```



# <a name="apidoc.module.openpgp.packet.PublicKey"></a>[module openpgp.packet.PublicKey](#apidoc.module.openpgp.packet.PublicKey)

#### <a name="apidoc.element.openpgp.packet.PublicKey.PublicKey"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>PublicKey ()](#apidoc.element.openpgp.packet.PublicKey.PublicKey)
- description and source-code
```javascript
function PublicKey() {
  this.tag = _enums2.default.packet.publicKey;
  this.version = 4;
<span class="apidocCodeCommentSpan">  /** Key creation date.
   * @type {Date} */
</span>  this.created = new Date();
  /** A list of multiprecision integers
   * @type {module:type/mpi} */
  this.mpi = [];
  /** Public key algorithm
   * @type {module:enums.publicKey} */
  this.algorithm = 'rsa_sign';
  // time in days (V3 only)
  this.expirationTimeV3 = 0;
  /**
   * Fingerprint in lowercase hex
   * @type {String}
   */
  this.fingerprint = null;
  /**
   * Keyid
   * @type {module:type/keyid}
   */
  this.keyid = null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet.PublicKey.prototype"></a>[module openpgp.packet.PublicKey.prototype](#apidoc.module.openpgp.packet.PublicKey.prototype)

#### <a name="apidoc.element.openpgp.packet.PublicKey.prototype.getBitSize"></a>[function <span class="apidocSignatureSpan">openpgp.packet.PublicKey.prototype.</span>getBitSize ()](#apidoc.element.openpgp.packet.PublicKey.prototype.getBitSize)
- description and source-code
```javascript
getBitSize = function () {
  return this.mpi[0].byteLength() * 8;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.PublicKey.prototype.getFingerprint"></a>[function <span class="apidocSignatureSpan">openpgp.packet.PublicKey.prototype.</span>getFingerprint ()](#apidoc.element.openpgp.packet.PublicKey.prototype.getFingerprint)
- description and source-code
```javascript
getFingerprint = function () {
  if (this.fingerprint) {
    return this.fingerprint;
  }
  var toHash = '';
  if (this.version === 4) {
    toHash = this.writeOld();
    this.fingerprint = _util2.default.Uint8Array2str(_crypto2.default.hash.sha1(toHash));
  } else if (this.version === 3) {
    var mpicount = _crypto2.default.getPublicMpiCount(this.algorithm);
    for (var i = 0; i < mpicount; i++) {
      toHash += this.mpi[i].toBytes();
    }
    this.fingerprint = _util2.default.Uint8Array2str(_crypto2.default.hash.md5(_util2.default.str2Uint8Array(toHash)));
  }
  this.fingerprint = _util2.default.hexstrdump(this.fingerprint);
  return this.fingerprint;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.PublicKey.prototype.getKeyId"></a>[function <span class="apidocSignatureSpan">openpgp.packet.PublicKey.prototype.</span>getKeyId ()](#apidoc.element.openpgp.packet.PublicKey.prototype.getKeyId)
- description and source-code
```javascript
getKeyId = function () {
  if (this.keyid) {
    return this.keyid;
  }
  this.keyid = new _keyid2.default();
  if (this.version === 4) {
    this.keyid.read(_util2.default.str2Uint8Array(_util2.default.hex2bin(this.getFingerprint()).substr(12, 8)));
  } else if (this.version === 3) {
    var arr = this.mpi[0].write();
    this.keyid.read(arr.subarray(arr.length - 8, arr.length));
  }
  return this.keyid;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.PublicKey.prototype.postCloneTypeFix"></a>[function <span class="apidocSignatureSpan">openpgp.packet.PublicKey.prototype.</span>postCloneTypeFix ()](#apidoc.element.openpgp.packet.PublicKey.prototype.postCloneTypeFix)
- description and source-code
```javascript
postCloneTypeFix = function () {
  for (var i = 0; i < this.mpi.length; i++) {
    this.mpi[i] = _mpi2.default.fromClone(this.mpi[i]);
  }
  if (this.keyid) {
    this.keyid = _keyid2.default.fromClone(this.keyid);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.PublicKey.prototype.read"></a>[function <span class="apidocSignatureSpan">openpgp.packet.PublicKey.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.PublicKey.prototype.read)
- description and source-code
```javascript
read = function (bytes) {
  var pos = 0;
  // A one-octet version number (3 or 4).
  this.version = bytes[pos++];

  if (this.version === 3 || this.version === 4) {
    // - A four-octet number denoting the time that the key was created.
    this.created = _util2.default.readDate(bytes.subarray(pos, pos + 4));
    pos += 4;

    if (this.version === 3) {
      // - A two-octet number denoting the time in days that this key is
      //   valid.  If this number is zero, then it does not expire.
      this.expirationTimeV3 = _util2.default.readNumber(bytes.subarray(pos, pos + 2));
      pos += 2;
    }

    // - A one-octet number denoting the public-key algorithm of this key.
    this.algorithm = _enums2.default.read(_enums2.default.publicKey, bytes[pos++]);

    var mpicount = _crypto2.default.getPublicMpiCount(this.algorithm);
    this.mpi = [];

    var bmpi = bytes.subarray(pos, bytes.length);
    var p = 0;

    for (var i = 0; i < mpicount && p < bmpi.length; i++) {

      this.mpi[i] = new _mpi2.default();

      p += this.mpi[i].read(bmpi.subarray(p, bmpi.length));

      if (p > bmpi.length) {
        throw new Error('Error reading MPI @:' + p);
      }
    }

    return p + 6;
  } else {
    throw new Error('Version ' + this.version + ' of the key packet is unsupported.');
  }
}
```
- example usage
```shell
...
openpgp.encrypt(options).then(function(ciphertext) {
    encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
...
```

#### <a name="apidoc.element.openpgp.packet.PublicKey.prototype.readPublicKey"></a>[function <span class="apidocSignatureSpan">openpgp.packet.PublicKey.prototype.</span>readPublicKey (bytes)](#apidoc.element.openpgp.packet.PublicKey.prototype.readPublicKey)
- description and source-code
```javascript
readPublicKey = function (bytes) {
  var pos = 0;
  // A one-octet version number (3 or 4).
  this.version = bytes[pos++];

  if (this.version === 3 || this.version === 4) {
    // - A four-octet number denoting the time that the key was created.
    this.created = _util2.default.readDate(bytes.subarray(pos, pos + 4));
    pos += 4;

    if (this.version === 3) {
      // - A two-octet number denoting the time in days that this key is
      //   valid.  If this number is zero, then it does not expire.
      this.expirationTimeV3 = _util2.default.readNumber(bytes.subarray(pos, pos + 2));
      pos += 2;
    }

    // - A one-octet number denoting the public-key algorithm of this key.
    this.algorithm = _enums2.default.read(_enums2.default.publicKey, bytes[pos++]);

    var mpicount = _crypto2.default.getPublicMpiCount(this.algorithm);
    this.mpi = [];

    var bmpi = bytes.subarray(pos, bytes.length);
    var p = 0;

    for (var i = 0; i < mpicount && p < bmpi.length; i++) {

      this.mpi[i] = new _mpi2.default();

      p += this.mpi[i].read(bmpi.subarray(p, bmpi.length));

      if (p > bmpi.length) {
        throw new Error('Error reading MPI @:' + p);
      }
    }

    return p + 6;
  } else {
    throw new Error('Version ' + this.version + ' of the key packet is unsupported.');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.PublicKey.prototype.write"></a>[function <span class="apidocSignatureSpan">openpgp.packet.PublicKey.prototype.</span>write ()](#apidoc.element.openpgp.packet.PublicKey.prototype.write)
- description and source-code
```javascript
write = function () {

  var arr = [];
  // Version
  arr.push(new Uint8Array([this.version]));
  arr.push(_util2.default.writeDate(this.created));
  if (this.version === 3) {
    arr.push(_util2.default.writeNumber(this.expirationTimeV3, 2));
  }
  arr.push(new Uint8Array([_enums2.default.write(_enums2.default.publicKey, this.algorithm)]));

  var mpicount = _crypto2.default.getPublicMpiCount(this.algorithm);

  for (var i = 0; i < mpicount; i++) {
    arr.push(this.mpi[i].write());
  }

  return _util2.default.concatUint8Array(arr);
}
```
- example usage
```shell
...
options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
password: 'secret stuff',                 // decrypt with password
...
```

#### <a name="apidoc.element.openpgp.packet.PublicKey.prototype.writeOld"></a>[function <span class="apidocSignatureSpan">openpgp.packet.PublicKey.prototype.</span>writeOld ()](#apidoc.element.openpgp.packet.PublicKey.prototype.writeOld)
- description and source-code
```javascript
writeOld = function () {
  var bytes = this.writePublicKey();

  return _util2.default.concatUint8Array([new Uint8Array([0x99]), _util2.default.writeNumber(bytes.length, 2), bytes]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.PublicKey.prototype.writePublicKey"></a>[function <span class="apidocSignatureSpan">openpgp.packet.PublicKey.prototype.</span>writePublicKey ()](#apidoc.element.openpgp.packet.PublicKey.prototype.writePublicKey)
- description and source-code
```javascript
writePublicKey = function () {

  var arr = [];
  // Version
  arr.push(new Uint8Array([this.version]));
  arr.push(_util2.default.writeDate(this.created));
  if (this.version === 3) {
    arr.push(_util2.default.writeNumber(this.expirationTimeV3, 2));
  }
  arr.push(new Uint8Array([_enums2.default.write(_enums2.default.publicKey, this.algorithm)]));

  var mpicount = _crypto2.default.getPublicMpiCount(this.algorithm);

  for (var i = 0; i < mpicount; i++) {
    arr.push(this.mpi[i].write());
  }

  return _util2.default.concatUint8Array(arr);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet.PublicKeyEncryptedSessionKey"></a>[module openpgp.packet.PublicKeyEncryptedSessionKey](#apidoc.module.openpgp.packet.PublicKeyEncryptedSessionKey)

#### <a name="apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey.PublicKeyEncryptedSessionKey"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>PublicKeyEncryptedSessionKey ()](#apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey.PublicKeyEncryptedSessionKey)
- description and source-code
```javascript
function PublicKeyEncryptedSessionKey() {
  this.tag = _enums2.default.packet.publicKeyEncryptedSessionKey;
  this.version = 3;

  this.publicKeyId = new _keyid2.default();
  this.publicKeyAlgorithm = 'rsa_encrypt';

  this.sessionKey = null;
  this.sessionKeyAlgorithm = 'aes256';

<span class="apidocCodeCommentSpan">  /** @type {Array<module:type/mpi>} */
</span>  this.encrypted = [];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet.PublicKeyEncryptedSessionKey.prototype"></a>[module openpgp.packet.PublicKeyEncryptedSessionKey.prototype](#apidoc.module.openpgp.packet.PublicKeyEncryptedSessionKey.prototype)

#### <a name="apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey.prototype.decrypt"></a>[function <span class="apidocSignatureSpan">openpgp.packet.PublicKeyEncryptedSessionKey.prototype.</span>decrypt (key)](#apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey.prototype.decrypt)
- description and source-code
```javascript
decrypt = function (key) {
  var result = _crypto2.default.publicKeyDecrypt(this.publicKeyAlgorithm, key.mpi, this.encrypted).toBytes();

  var checksum = _util2.default.readNumber(_util2.default.str2Uint8Array(result.substr(result.length - 2)));

  var decoded = _crypto2.default.pkcs1.eme.decode(result);

  key = _util2.default.str2Uint8Array(decoded.substring(1, decoded.length - 2));

  if (checksum !== _util2.default.calc_checksum(key)) {
    throw new Error('Checksum mismatch');
  } else {
    this.sessionKey = key;
    this.sessionKeyAlgorithm = _enums2.default.read(_enums2.default.symmetric, decoded.charCodeAt(0));
  }
}
```
- example usage
```shell
...
'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
'''

#### Encrypt and decrypt *String* data with PGP keys

'''js
...
```

#### <a name="apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey.prototype.encrypt"></a>[function <span class="apidocSignatureSpan">openpgp.packet.PublicKeyEncryptedSessionKey.prototype.</span>encrypt (key)](#apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey.prototype.encrypt)
- description and source-code
```javascript
encrypt = function (key) {
  var data = String.fromCharCode(_enums2.default.write(_enums2.default.symmetric, this.sessionKeyAlgorithm));

  data += _util2.default.Uint8Array2str(this.sessionKey);
  var checksum = _util2.default.calc_checksum(this.sessionKey);
  data += _util2.default.Uint8Array2str(_util2.default.writeNumber(checksum, 2));

  var mpi = new _mpi2.default();
  mpi.fromBytes(_crypto2.default.pkcs1.eme.encode(data, key.mpi[0].byteLength()));

  this.encrypted = _crypto2.default.publicKeyEncrypt(this.publicKeyAlgorithm, key.mpi, mpi);
}
```
- example usage
```shell
...

options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
...
```

#### <a name="apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey.prototype.postCloneTypeFix"></a>[function <span class="apidocSignatureSpan">openpgp.packet.PublicKeyEncryptedSessionKey.prototype.</span>postCloneTypeFix ()](#apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey.prototype.postCloneTypeFix)
- description and source-code
```javascript
postCloneTypeFix = function () {
  this.publicKeyId = _keyid2.default.fromClone(this.publicKeyId);
  for (var i = 0; i < this.encrypted.length; i++) {
    this.encrypted[i] = _mpi2.default.fromClone(this.encrypted[i]);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey.prototype.read"></a>[function <span class="apidocSignatureSpan">openpgp.packet.PublicKeyEncryptedSessionKey.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey.prototype.read)
- description and source-code
```javascript
read = function (bytes) {

  this.version = bytes[0];
  this.publicKeyId.read(bytes.subarray(1, bytes.length));
  this.publicKeyAlgorithm = _enums2.default.read(_enums2.default.publicKey, bytes[9]);

  var i = 10;

  var integerCount = function (algo) {
    switch (algo) {
      case 'rsa_encrypt':
      case 'rsa_encrypt_sign':
        return 1;

      case 'elgamal':
        return 2;

      default:
        throw new Error("Invalid algorithm.");
    }
  }(this.publicKeyAlgorithm);

  this.encrypted = [];

  for (var j = 0; j < integerCount; j++) {
    var mpi = new _mpi2.default();
    i += mpi.read(bytes.subarray(i, bytes.length));
    this.encrypted.push(mpi);
  }
}
```
- example usage
```shell
...
openpgp.encrypt(options).then(function(ciphertext) {
    encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
...
```

#### <a name="apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey.prototype.write"></a>[function <span class="apidocSignatureSpan">openpgp.packet.PublicKeyEncryptedSessionKey.prototype.</span>write ()](#apidoc.element.openpgp.packet.PublicKeyEncryptedSessionKey.prototype.write)
- description and source-code
```javascript
write = function () {

  var arr = [new Uint8Array([this.version]), this.publicKeyId.write(), new Uint8Array([_enums2.default.write(_enums2.default.publicKey
, this.publicKeyAlgorithm)])];

  for (var i = 0; i < this.encrypted.length; i++) {
    arr.push(this.encrypted[i].write());
  }

  return _util2.default.concatUint8Array(arr);
}
```
- example usage
```shell
...
options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
password: 'secret stuff',                 // decrypt with password
...
```



# <a name="apidoc.module.openpgp.packet.PublicSubkey"></a>[module openpgp.packet.PublicSubkey](#apidoc.module.openpgp.packet.PublicSubkey)

#### <a name="apidoc.element.openpgp.packet.PublicSubkey.PublicSubkey"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>PublicSubkey ()](#apidoc.element.openpgp.packet.PublicSubkey.PublicSubkey)
- description and source-code
```javascript
function PublicSubkey() {
  _public_key2.default.call(this);
  this.tag = _enums2.default.packet.publicSubkey;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet.PublicSubkey.prototype"></a>[module openpgp.packet.PublicSubkey.prototype](#apidoc.module.openpgp.packet.PublicSubkey.prototype)

#### <a name="apidoc.element.openpgp.packet.PublicSubkey.prototype.constructor"></a>[function <span class="apidocSignatureSpan">openpgp.packet.PublicSubkey.prototype.</span>constructor ()](#apidoc.element.openpgp.packet.PublicSubkey.prototype.constructor)
- description and source-code
```javascript
function PublicSubkey() {
  _public_key2.default.call(this);
  this.tag = _enums2.default.packet.publicSubkey;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet.SecretKey"></a>[module openpgp.packet.SecretKey](#apidoc.module.openpgp.packet.SecretKey)

#### <a name="apidoc.element.openpgp.packet.SecretKey.SecretKey"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>SecretKey ()](#apidoc.element.openpgp.packet.SecretKey.SecretKey)
- description and source-code
```javascript
function SecretKey() {
  _public_key2.default.call(this);
  this.tag = _enums2.default.packet.secretKey;
  // encrypted secret-key data
  this.encrypted = null;
  // indicator if secret-key data is available in decrypted form
  this.isDecrypted = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet.SecretKey.prototype"></a>[module openpgp.packet.SecretKey.prototype](#apidoc.module.openpgp.packet.SecretKey.prototype)

#### <a name="apidoc.element.openpgp.packet.SecretKey.prototype.clearPrivateMPIs"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SecretKey.prototype.</span>clearPrivateMPIs ()](#apidoc.element.openpgp.packet.SecretKey.prototype.clearPrivateMPIs)
- description and source-code
```javascript
clearPrivateMPIs = function () {
  if (!this.encrypted) {
    throw new Error('If secret key is not encrypted, clearing private MPIs is irreversible.');
  }
  this.mpi = this.mpi.slice(0, _crypto2.default.getPublicMpiCount(this.algorithm));
  this.isDecrypted = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.SecretKey.prototype.constructor"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SecretKey.prototype.</span>constructor ()](#apidoc.element.openpgp.packet.SecretKey.prototype.constructor)
- description and source-code
```javascript
function SecretKey() {
  _public_key2.default.call(this);
  this.tag = _enums2.default.packet.secretKey;
  // encrypted secret-key data
  this.encrypted = null;
  // indicator if secret-key data is available in decrypted form
  this.isDecrypted = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.SecretKey.prototype.decrypt"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SecretKey.prototype.</span>decrypt (passphrase)](#apidoc.element.openpgp.packet.SecretKey.prototype.decrypt)
- description and source-code
```javascript
decrypt = function (passphrase) {
  if (this.isDecrypted) {
    return true;
  }

  var i = 0,
      symmetric,
      key;

  var s2k_usage = this.encrypted[i++];

  // - [Optional] If string-to-key usage octet was 255 or 254, a one-
  //   octet symmetric encryption algorithm.
  if (s2k_usage === 255 || s2k_usage === 254) {
    symmetric = this.encrypted[i++];
    symmetric = _enums2.default.read(_enums2.default.symmetric, symmetric);

    // - [Optional] If string-to-key usage octet was 255 or 254, a
    //   string-to-key specifier.  The length of the string-to-key
    //   specifier is implied by its type, as described above.
    var s2k = new _s2k2.default();
    i += s2k.read(this.encrypted.subarray(i, this.encrypted.length));

    key = produceEncryptionKey(s2k, passphrase, symmetric);
  } else {
    symmetric = s2k_usage;
    symmetric = _enums2.default.read(_enums2.default.symmetric, symmetric);
    key = _crypto2.default.hash.md5(passphrase);
  }

  // - [Optional] If secret data is encrypted (string-to-key usage octet
  //   not zero), an Initial Vector (IV) of the same length as the
  //   cipher's block size.
  var iv = this.encrypted.subarray(i, i + _crypto2.default.cipher[symmetric].blockSize);

  i += iv.length;

  var cleartext,
      ciphertext = this.encrypted.subarray(i, this.encrypted.length);

  cleartext = _crypto2.default.cfb.normalDecrypt(symmetric, key, ciphertext, iv);

  var hash = s2k_usage === 254 ? 'sha1' : 'mod';

  var parsedMPI = parse_cleartext_mpi(hash, cleartext, this.algorithm);
  if (parsedMPI instanceof Error) {
    return false;
  }
  this.mpi = this.mpi.concat(parsedMPI);
  this.isDecrypted = true;
  this.encrypted = null;
  return true;
}
```
- example usage
```shell
...
'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
'''

#### Encrypt and decrypt *String* data with PGP keys

'''js
...
```

#### <a name="apidoc.element.openpgp.packet.SecretKey.prototype.encrypt"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SecretKey.prototype.</span>encrypt (passphrase)](#apidoc.element.openpgp.packet.SecretKey.prototype.encrypt)
- description and source-code
```javascript
encrypt = function (passphrase) {
  if (this.isDecrypted && !passphrase) {
    this.encrypted = null;
    return;
  } else if (!passphrase) {
    throw new Error('The key must be decrypted before removing passphrase protection.');
  }

  var s2k = new _s2k2.default(),
      symmetric = 'aes256',
      cleartext = write_cleartext_mpi('sha1', this.algorithm, this.mpi),
      key = produceEncryptionKey(s2k, passphrase, symmetric),
      blockLen = _crypto2.default.cipher[symmetric].blockSize,
      iv = _crypto2.default.random.getRandomBytes(blockLen);

  var arr = [new Uint8Array([254, _enums2.default.write(_enums2.default.symmetric, symmetric)])];
  arr.push(s2k.write());
  arr.push(iv);
  arr.push(_crypto2.default.cfb.normalEncrypt(symmetric, key, cleartext, iv));

  this.encrypted = _util2.default.concatUint8Array(arr);
}
```
- example usage
```shell
...

options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
...
```

#### <a name="apidoc.element.openpgp.packet.SecretKey.prototype.generate"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SecretKey.prototype.</span>generate (bits)](#apidoc.element.openpgp.packet.SecretKey.prototype.generate)
- description and source-code
```javascript
generate = function (bits) {
  var self = this;

  return _crypto2.default.generateMpi(self.algorithm, bits).then(function (mpi) {
    self.mpi = mpi;
    self.isDecrypted = true;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.SecretKey.prototype.read"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SecretKey.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.SecretKey.prototype.read)
- description and source-code
```javascript
read = function (bytes) {
  // - A Public-Key or Public-Subkey packet, as described above.
  var len = this.readPublicKey(bytes);

  bytes = bytes.subarray(len, bytes.length);

  // - One octet indicating string-to-key usage conventions.  Zero
  //   indicates that the secret-key data is not encrypted.  255 or 254
  //   indicates that a string-to-key specifier is being given.  Any
  //   other value is a symmetric-key encryption algorithm identifier.
  var isEncrypted = bytes[0];

  if (isEncrypted) {
    this.encrypted = bytes;
  } else {
    // - Plain or encrypted multiprecision integers comprising the secret
    //   key data.  These algorithm-specific fields are as described
    //   below.
    var parsedMPI = parse_cleartext_mpi('mod', bytes.subarray(1, bytes.length), this.algorithm);
    if (parsedMPI instanceof Error) {
      throw parsedMPI;
    }
    this.mpi = this.mpi.concat(parsedMPI);
    this.isDecrypted = true;
  }
}
```
- example usage
```shell
...
openpgp.encrypt(options).then(function(ciphertext) {
    encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
...
```

#### <a name="apidoc.element.openpgp.packet.SecretKey.prototype.write"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SecretKey.prototype.</span>write ()](#apidoc.element.openpgp.packet.SecretKey.prototype.write)
- description and source-code
```javascript
write = function () {
  var arr = [this.writePublicKey()];

  if (!this.encrypted) {
    arr.push(new Uint8Array([0]));
    arr.push(write_cleartext_mpi('mod', this.algorithm, this.mpi));
  } else {
    arr.push(this.encrypted);
  }

  return _util2.default.concatUint8Array(arr);
}
```
- example usage
```shell
...
options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
password: 'secret stuff',                 // decrypt with password
...
```



# <a name="apidoc.module.openpgp.packet.SecretSubkey"></a>[module openpgp.packet.SecretSubkey](#apidoc.module.openpgp.packet.SecretSubkey)

#### <a name="apidoc.element.openpgp.packet.SecretSubkey.SecretSubkey"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>SecretSubkey ()](#apidoc.element.openpgp.packet.SecretSubkey.SecretSubkey)
- description and source-code
```javascript
function SecretSubkey() {
  _secret_key2.default.call(this);
  this.tag = _enums2.default.packet.secretSubkey;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet.SecretSubkey.prototype"></a>[module openpgp.packet.SecretSubkey.prototype](#apidoc.module.openpgp.packet.SecretSubkey.prototype)

#### <a name="apidoc.element.openpgp.packet.SecretSubkey.prototype.constructor"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SecretSubkey.prototype.</span>constructor ()](#apidoc.element.openpgp.packet.SecretSubkey.prototype.constructor)
- description and source-code
```javascript
function SecretSubkey() {
  _secret_key2.default.call(this);
  this.tag = _enums2.default.packet.secretSubkey;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet.Signature"></a>[module openpgp.packet.Signature](#apidoc.module.openpgp.packet.Signature)

#### <a name="apidoc.element.openpgp.packet.Signature.Signature"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>Signature ()](#apidoc.element.openpgp.packet.Signature.Signature)
- description and source-code
```javascript
function Signature() {
  this.tag = _enums2.default.packet.signature;
  this.version = 4;
  this.signatureType = null;
  this.hashAlgorithm = null;
  this.publicKeyAlgorithm = null;

  this.signatureData = null;
  this.unhashedSubpackets = null;
  this.signedHashValue = null;

  this.created = new Date();
  this.signatureExpirationTime = null;
  this.signatureNeverExpires = true;
  this.exportable = null;
  this.trustLevel = null;
  this.trustAmount = null;
  this.regularExpression = null;
  this.revocable = null;
  this.keyExpirationTime = null;
  this.keyNeverExpires = null;
  this.preferredSymmetricAlgorithms = null;
  this.revocationKeyClass = null;
  this.revocationKeyAlgorithm = null;
  this.revocationKeyFingerprint = null;
  this.issuerKeyId = new _keyid2.default();
  this.notation = null;
  this.preferredHashAlgorithms = null;
  this.preferredCompressionAlgorithms = null;
  this.keyServerPreferences = null;
  this.preferredKeyServer = null;
  this.isPrimaryUserID = null;
  this.policyURI = null;
  this.keyFlags = null;
  this.signersUserId = null;
  this.reasonForRevocationFlag = null;
  this.reasonForRevocationString = null;
  this.features = null;
  this.signatureTargetPublicKeyAlgorithm = null;
  this.signatureTargetHashAlgorithm = null;
  this.signatureTargetHash = null;
  this.embeddedSignature = null;

  this.verified = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet.Signature.prototype"></a>[module openpgp.packet.Signature.prototype](#apidoc.module.openpgp.packet.Signature.prototype)

#### <a name="apidoc.element.openpgp.packet.Signature.prototype.calculateTrailer"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Signature.prototype.</span>calculateTrailer ()](#apidoc.element.openpgp.packet.Signature.prototype.calculateTrailer)
- description and source-code
```javascript
calculateTrailer = function () {
  // calculating the trailer
  // V3 signatures don't have a trailer
  if (this.version === 3) {
    return new Uint8Array(0);
  }
  var first = new Uint8Array([4, 0xFF]); //Version, ?
  return _util2.default.concatUint8Array([first, _util2.default.writeNumber(this.signatureData.length, 4)]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Signature.prototype.isExpired"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Signature.prototype.</span>isExpired ()](#apidoc.element.openpgp.packet.Signature.prototype.isExpired)
- description and source-code
```javascript
isExpired = function () {
  if (!this.signatureNeverExpires) {
    return Date.now() > this.created.getTime() + this.signatureExpirationTime * 1000;
  }
  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Signature.prototype.postCloneTypeFix"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Signature.prototype.</span>postCloneTypeFix ()](#apidoc.element.openpgp.packet.Signature.prototype.postCloneTypeFix)
- description and source-code
```javascript
postCloneTypeFix = function () {
  this.issuerKeyId = _keyid2.default.fromClone(this.issuerKeyId);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Signature.prototype.read"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Signature.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.Signature.prototype.read)
- description and source-code
```javascript
read = function (bytes) {
  var _this = this;

  var i = 0;
  this.version = bytes[i++];
  // switch on version (3 and 4)
  var sigpos;
  var sigDataLength;

  (function () {
    switch (_this.version) {
      case 3:
        // One-octet length of following hashed material. MUST be 5.
        if (bytes[i++] !== 5) {
          _util2.default.print_debug("packet/signature.js\n" + 'invalid One-octet length of following hashed material.' + 'MUST
be 5. @:' + (i - 1));
        }

        sigpos = i;
        // One-octet signature type.

        _this.signatureType = bytes[i++];

        // Four-octet creation time.
        _this.created = _util2.default.readDate(bytes.subarray(i, i + 4));
        i += 4;

        // storing data appended to data which gets verified
        _this.signatureData = bytes.subarray(sigpos, i);

        // Eight-octet Key ID of signer.
        _this.issuerKeyId.read(bytes.subarray(i, i + 8));
        i += 8;

        // One-octet public-key algorithm.
        _this.publicKeyAlgorithm = bytes[i++];

        // One-octet hash algorithm.
        _this.hashAlgorithm = bytes[i++];
        break;
      case 4:
        _this.signatureType = bytes[i++];
        _this.publicKeyAlgorithm = bytes[i++];
        _this.hashAlgorithm = bytes[i++];

        var subpackets = function subpackets(bytes) {
          // Two-octet scalar octet count for following subpacket data.
          var subpacket_length = _util2.default.readNumber(bytes.subarray(0, 2));

          var i = 2;

          // subpacket data set (zero or more subpackets)
          while (i < 2 + subpacket_length) {

            var len = _packet2.default.readSimpleLength(bytes.subarray(i, bytes.length));
            i += len.offset;

            this.read_sub_packet(bytes.subarray(i, i + len.len));

            i += len.len;
          }

          return i;
        };

        // hashed subpackets


        i += subpackets.call(_this, bytes.subarray(i, bytes.length), true);

        // A V4 signature hashes the packet body
        // starting from its first field, the version number, through the end
        // of the hashed subpacket data.  Thus, the fields hashed are the
        // signature version, the signature type, the public-key algorithm, the
        // hash algorithm, the hashed subpacket length, and the hashed
        // subpacket body.
        _this.signatureData = bytes.subarray(0, i);
        sigDataLength = i;

        // unhashed subpackets

        i += subpackets.call(_this, bytes.subarray(i, bytes.length), false);
        _this.unhashedSubpackets = bytes.subarray(sigDataLength, i);

        break;
      default:
        throw new Error('Version ' + _this.version + ' of the signature is unsupported.');
    }

    // Two-octet field holding left 16 bits of signed hash value.
  })();

  this.signedHashValue = bytes.subarray(i, i + 2);
  i += 2;

  this.signature = bytes.subarray(i, bytes.length);
}
```
- example usage
```shell
...
openpgp.encrypt(options).then(function(ciphertext) {
    encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
...
```

#### <a name="apidoc.element.openpgp.packet.Signature.prototype.read_sub_packet"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Signature.prototype.</span>read_sub_packet (bytes)](#apidoc.element.openpgp.packet.Signature.prototype.read_sub_packet)
- description and source-code
```javascript
read_sub_packet = function (bytes) {
  var mypos = 0;

  function read_array(prop, bytes) {
    this[prop] = [];

    for (var i = 0; i < bytes.length; i++) {
      this[prop].push(bytes[i]);
    }
  }

  // The leftwost bit denotes a "critical" packet, but we ignore it.
  var type = bytes[mypos++] & 0x7F;
  var seconds;

  // subpacket type
  switch (type) {
    case 2:
      // Signature Creation Time
      this.created = _util2.default.readDate(bytes.subarray(mypos, bytes.length));
      break;
    case 3:
      // Signature Expiration Time in seconds
      seconds = _util2.default.readNumber(bytes.subarray(mypos, bytes.length));

      this.signatureNeverExpires = seconds === 0;
      this.signatureExpirationTime = seconds;

      break;
    case 4:
      // Exportable Certification
      this.exportable = bytes[mypos++] === 1;
      break;
    case 5:
      // Trust Signature
      this.trustLevel = bytes[mypos++];
      this.trustAmount = bytes[mypos++];
      break;
    case 6:
      // Regular Expression
      this.regularExpression = bytes[mypos];
      break;
    case 7:
      // Revocable
      this.revocable = bytes[mypos++] === 1;
      break;
    case 9:
      // Key Expiration Time in seconds
      seconds = _util2.default.readNumber(bytes.subarray(mypos, bytes.length));

      this.keyExpirationTime = seconds;
      this.keyNeverExpires = seconds === 0;

      break;
    case 11:
      // Preferred Symmetric Algorithms
      read_array.call(this, 'preferredSymmetricAlgorithms', bytes.subarray(mypos, bytes.length));
      break;
    case 12:
      // Revocation Key
      // (1 octet of class, 1 octet of public-key algorithm ID, 20
      // octets of
      // fingerprint)
      this.revocationKeyClass = bytes[mypos++];
      this.revocationKeyAlgorithm = bytes[mypos++];
      this.revocationKeyFingerprint = bytes.subarray(mypos, 20);
      break;

    case 16:
      // Issuer
      this.issuerKeyId.read(bytes.subarray(mypos, bytes.length));
      break;

    case 20:
      // Notation Data
      // We don't know how to handle anything but a text flagged data.
      if (bytes[mypos] === 0x80) {

        // We extract key/value tuple from the byte stream.
        mypos += 4;
        var m = _util2.default.readNumber(bytes.subarray(mypos, mypos + 2));
        mypos += 2;
        var n = _util2.default.readNumber(bytes.subarray(mypos, mypos + 2));
        mypos += 2;

        var name = _util2.default.Uint8Array2str(bytes.subarray(mypos, mypos + m)),
            value = _util2.default.Uint8Array2str(bytes.subarray(mypos + m, mypos + m + n));

        this.notation = this.notation || {};
        this.notation[name] = value;
      } else {
        _util2.default.print_debug("Unsupported notation flag " + bytes[mypos]);
      }
      break;
    case 21:
      // Preferred Hash Algorithms
      read_array.call(this, 'preferredHashAlgorithms', bytes.subarray(mypos, bytes.length));
      break;
    case 22:
      // Preferred Compression Algorithms
      read_array.call(this, 'preferredCompressionAlgorithms', bytes.subarray(mypos, bytes.length));
      break;
    case 23:
      // Key Server Preferences
      read_array.call(this, 'keyServerPreferencess', bytes.subarray(mypos, bytes.length));
      break;
    case 24:
      // Preferred Key Server
      this.preferredKeyServer = _util2.default.Uint8Array2str(bytes.subarray(mypos, bytes.length));
      break;
    case 25:
      // Primary User ID
      this.isPrimaryUserID = bytes[mypos++] !== 0;
      break;
    case 26:
      // Policy URI
      this.policyURI = _util2.default.Uint8Array2str(bytes.subarray(mypos, bytes.length));
      break;
    case 27:
      // Key Flags
      read_array.call(this, 'keyFlags', bytes.subarray(mypos, bytes.length));
      break;
    case 28:
      // Signer's User ID
      this.signersUserId += _util2.default.Uint8Array2str(bytes.subarray(mypos, bytes.length));
      break;
    case 29:
      // Reason for Revocation
      this.reasonForRevocationFlag = bytes[mypos++];
      this.reasonForRevocationString = _util2.default.Uint8Array2str(bytes.subarra ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Signature.prototype.sign"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Signature.prototype.</span>sign (key, data)](#apidoc.element.openpgp.packet.Signature.prototype.sign)
- description and source-code
```javascript
sign = function (key, data) {
  var signatureType = _enums2.default.write(_enums2.default.signature, this.signatureType),
      publicKeyAlgorithm = _enums2.default.write(_enums2.default.publicKey, this.publicKeyAlgorithm),
      hashAlgorithm = _enums2.default.write(_enums2.default.hash, this.hashAlgorithm);

  var arr = [new Uint8Array([4, signatureType, publicKeyAlgorithm, hashAlgorithm])];

  this.issuerKeyId = key.getKeyId();

  // Add hashed subpackets
  arr.push(this.write_all_sub_packets());

  this.signatureData = _util2.default.concatUint8Array(arr);

  var trailer = this.calculateTrailer();

  var toHash = null;

  switch (this.version) {
    case 3:
      toHash = _util2.default.concatUint8Array([this.toSign(signatureType, data), new Uint8Array([signatureType]), _util2.default
.writeDate(this.created)]);
      break;
    case 4:
      toHash = _util2.default.concatUint8Array([this.toSign(signatureType, data), this.signatureData, trailer]);
      break;
    default:
      throw new Error('Version ' + this.version + ' of the signature is unsupported.');
  }

  var hash = _crypto2.default.hash.digest(hashAlgorithm, toHash);

  this.signedHashValue = hash.subarray(0, 2);

  this.signature = _crypto2.default.signature.sign(hashAlgorithm, publicKeyAlgorithm, key.mpi, toHash);
}
```
- example usage
```shell
...

'''js
options = {
data: 'Hello, World!',                             // input as String (or Uint8Array)
privateKeys: privKeyObj // for signing
};

openpgp.sign(options).then(function(signed) {
cleartext = signed.data; // '-----BEGIN PGP SIGNED MESSAGE ... END PGP SIGNATURE-----'
});
'''

'''js
options = {
message: openpgp.cleartext.readArmored(cleartext), // parse armored message
...
```

#### <a name="apidoc.element.openpgp.packet.Signature.prototype.toSign"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Signature.prototype.</span>toSign (type, data)](#apidoc.element.openpgp.packet.Signature.prototype.toSign)
- description and source-code
```javascript
toSign = function (type, data) {
  var t = _enums2.default.signature;

  switch (type) {
    case t.binary:
    case t.text:
      return data.getBytes();

    case t.standalone:
      return new Uint8Array(0);

    case t.cert_generic:
    case t.cert_persona:
    case t.cert_casual:
    case t.cert_positive:
    case t.cert_revocation:
      var packet, tag;

      if (data.userid !== undefined) {
        tag = 0xB4;
        packet = data.userid;
      } else if (data.userattribute !== undefined) {
        tag = 0xD1;
        packet = data.userattribute;
      } else {
        throw new Error('Either a userid or userattribute packet needs to be ' + 'supplied for certification.');
      }

      var bytes = packet.write();

      if (this.version === 4) {
        return _util2.default.concatUint8Array([this.toSign(t.key, data), new Uint8Array([tag]), _util2.default.writeNumber(bytes
.length, 4), bytes]);
      } else if (this.version === 3) {
        return _util2.default.concatUint8Array([this.toSign(t.key, data), bytes]);
      }
      break;

    case t.subkey_binding:
    case t.subkey_revocation:
    case t.key_binding:
      return _util2.default.concatUint8Array([this.toSign(t.key, data), this.toSign(t.key, {
        key: data.bind
      })]);

    case t.key:
      if (data.key === undefined) {
        throw new Error('Key packet is required for this signature.');
      }
      return data.key.writeOld();

    case t.key_revocation:
      return this.toSign(t.key, data);
    case t.timestamp:
      return new Uint8Array(0);
    case t.third_party:
      throw new Error('Not implemented');
    default:
      throw new Error('Unknown signature type.');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.Signature.prototype.verify"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Signature.prototype.</span>verify (key, data)](#apidoc.element.openpgp.packet.Signature.prototype.verify)
- description and source-code
```javascript
verify = function (key, data) {
  var signatureType = _enums2.default.write(_enums2.default.signature, this.signatureType),
      publicKeyAlgorithm = _enums2.default.write(_enums2.default.publicKey, this.publicKeyAlgorithm),
      hashAlgorithm = _enums2.default.write(_enums2.default.hash, this.hashAlgorithm);

  var bytes = this.toSign(signatureType, data),
      trailer = this.calculateTrailer();

  var mpicount = 0;
  // Algorithm-Specific Fields for RSA signatures:
  //      - multiprecision number (MPI) of RSA signature value m**d mod n.
  if (publicKeyAlgorithm > 0 && publicKeyAlgorithm < 4) {
    mpicount = 1;
  }
  //    Algorithm-Specific Fields for DSA signatures:
  //      - MPI of DSA value r.
  //      - MPI of DSA value s.
  else if (publicKeyAlgorithm === 17) {
      mpicount = 2;
    }

  var mpi = [],
      i = 0;
  for (var j = 0; j < mpicount; j++) {
    mpi[j] = new _mpi2.default();
    i += mpi[j].read(this.signature.subarray(i, this.signature.length));
  }

  this.verified = _crypto2.default.signature.verify(publicKeyAlgorithm, hashAlgorithm, mpi, key.mpi, _util2.default.concatUint8Array
([bytes, this.signatureData, trailer]));

  return this.verified;
}
```
- example usage
```shell
...

'''js
options = {
    message: openpgp.cleartext.readArmored(cleartext), // parse armored message
    publicKeys: openpgp.key.readArmored(pubkey).keys   // for verification
};

openpgp.verify(options).then(function(verified) {
	validity = verified.signatures[0].valid; // true
	if (validity) {
		console.log('signed by key id ' + verified.signatures[0].keyid.toHex());
	}
});
'''
...
```

#### <a name="apidoc.element.openpgp.packet.Signature.prototype.write"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Signature.prototype.</span>write ()](#apidoc.element.openpgp.packet.Signature.prototype.write)
- description and source-code
```javascript
write = function () {
  var arr = [];
  switch (this.version) {
    case 3:
      arr.push(new Uint8Array([3, 5])); // version, One-octet length of following hashed material.  MUST be 5
      arr.push(new Uint8Array([this.signatureType]));
      arr.push(_util2.default.writeDate(this.created));
      arr.push(this.issuerKeyId.write());
      arr.push(new Uint8Array([_enums2.default.write(_enums2.default.publicKey, this.publicKeyAlgorithm), _enums2.default.write(
_enums2.default.hash, this.hashAlgorithm)]));
      break;
    case 4:
      arr.push(this.signatureData);
      arr.push(this.unhashedSubpackets ? this.unhashedSubpackets : _util2.default.writeNumber(0, 2));
      break;
  }
  arr.push(this.signedHashValue);
  arr.push(this.signature);
  return _util2.default.concatUint8Array(arr);
}
```
- example usage
```shell
...
options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
password: 'secret stuff',                 // decrypt with password
...
```

#### <a name="apidoc.element.openpgp.packet.Signature.prototype.write_all_sub_packets"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Signature.prototype.</span>write_all_sub_packets ()](#apidoc.element.openpgp.packet.Signature.prototype.write_all_sub_packets)
- description and source-code
```javascript
write_all_sub_packets = function () {
  var sub = _enums2.default.signatureSubpacket;
  var arr = [];
  var bytes;
  if (this.created !== null) {
    arr.push(write_sub_packet(sub.signature_creation_time, _util2.default.writeDate(this.created)));
  }
  if (this.signatureExpirationTime !== null) {
    arr.push(write_sub_packet(sub.signature_expiration_time, _util2.default.writeNumber(this.signatureExpirationTime, 4)));
  }
  if (this.exportable !== null) {
    arr.push(write_sub_packet(sub.exportable_certification, new Uint8Array([this.exportable ? 1 : 0])));
  }
  if (this.trustLevel !== null) {
    bytes = new Uint8Array([this.trustLevel, this.trustAmount]);
    arr.push(write_sub_packet(sub.trust_signature, bytes));
  }
  if (this.regularExpression !== null) {
    arr.push(write_sub_packet(sub.regular_expression, this.regularExpression));
  }
  if (this.revocable !== null) {
    arr.push(write_sub_packet(sub.revocable, new Uint8Array([this.revocable ? 1 : 0])));
  }
  if (this.keyExpirationTime !== null) {
    arr.push(write_sub_packet(sub.key_expiration_time, _util2.default.writeNumber(this.keyExpirationTime, 4)));
  }
  if (this.preferredSymmetricAlgorithms !== null) {
    bytes = _util2.default.str2Uint8Array(_util2.default.bin2str(this.preferredSymmetricAlgorithms));
    arr.push(write_sub_packet(sub.preferred_symmetric_algorithms, bytes));
  }
  if (this.revocationKeyClass !== null) {

    bytes = new Uint8Array([this.revocationKeyClass, this.revocationKeyAlgorithm]);
    bytes = _util2.default.concatUint8Array([bytes, this.revocationKeyFingerprint]);
    arr.push(write_sub_packet(sub.revocation_key, bytes));
  }
  if (!this.issuerKeyId.isNull()) {
    arr.push(write_sub_packet(sub.issuer, this.issuerKeyId.write()));
  }
  if (this.notation !== null) {
    for (var name in this.notation) {
      if (this.notation.hasOwnProperty(name)) {
        var value = this.notation[name];
        bytes = [new Uint8Array([0x80, 0, 0, 0])];
        // 2 octets of name length
        bytes.push(_util2.default.writeNumber(name.length, 2));
        // 2 octets of value length
        bytes.push(_util2.default.writeNumber(value.length, 2));
        bytes.push(_util2.default.str2Uint8Array(name + value));
        bytes = _util2.default.concatUint8Array(bytes);
        arr.push(write_sub_packet(sub.notation_data, bytes));
      }
    }
  }
  if (this.preferredHashAlgorithms !== null) {
    bytes = _util2.default.str2Uint8Array(_util2.default.bin2str(this.preferredHashAlgorithms));
    arr.push(write_sub_packet(sub.preferred_hash_algorithms, bytes));
  }
  if (this.preferredCompressionAlgorithms !== null) {
    bytes = _util2.default.str2Uint8Array(_util2.default.bin2str(this.preferredCompressionAlgorithms));
    arr.push(write_sub_packet(sub.preferred_compression_algorithms, bytes));
  }
  if (this.keyServerPreferences !== null) {
    bytes = _util2.default.str2Uint8Array(_util2.default.bin2str(this.keyServerPreferences));
    arr.push(write_sub_packet(sub.key_server_preferences, bytes));
  }
  if (this.preferredKeyServer !== null) {
    arr.push(write_sub_packet(sub.preferred_key_server, _util2.default.str2Uint8Array(this.preferredKeyServer)));
  }
  if (this.isPrimaryUserID !== null) {
    arr.push(write_sub_packet(sub.primary_user_id, new Uint8Array([this.isPrimaryUserID ? 1 : 0])));
  }
  if (this.policyURI !== null) {
    arr.push(write_sub_packet(sub.policy_uri, _util2.default.str2Uint8Array(this.policyURI)));
  }
  if (this.keyFlags !== null) {
    bytes = _util2.default.str2Uint8Array(_util2.default.bin2str(this.keyFlags));
    arr.push(write_sub_packet(sub.key_flags, bytes));
  }
  if (this.signersUserId !== null) {
    arr.push(write_sub_packet(sub.signers_user_id, _util2.default.str2Uint8Array(this.signersUserId)));
  }
  if (this.reasonForRevocationFlag !== null) {
    bytes = _util2.default.str2Uint8Array(String.fromCharCode(this.reasonForRevocationFlag) + this.reasonForRevocationString);
    arr.push(write_sub_packet(sub.reason_for_revocation, bytes));
  }
  if (this.features !== null) {
    bytes = _util2.default.str2Uint8Array(_util2.default ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet.SymEncryptedAEADProtected"></a>[module openpgp.packet.SymEncryptedAEADProtected](#apidoc.module.openpgp.packet.SymEncryptedAEADProtected)

#### <a name="apidoc.element.openpgp.packet.SymEncryptedAEADProtected.SymEncryptedAEADProtected"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>SymEncryptedAEADProtected ()](#apidoc.element.openpgp.packet.SymEncryptedAEADProtected.SymEncryptedAEADProtected)
- description and source-code
```javascript
function SymEncryptedAEADProtected() {
  this.tag = _enums2.default.packet.symEncryptedAEADProtected;
  this.version = VERSION;
  this.iv = null;
  this.encrypted = null;
  this.packets = null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet.SymEncryptedAEADProtected.prototype"></a>[module openpgp.packet.SymEncryptedAEADProtected.prototype](#apidoc.module.openpgp.packet.SymEncryptedAEADProtected.prototype)

#### <a name="apidoc.element.openpgp.packet.SymEncryptedAEADProtected.prototype.decrypt"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedAEADProtected.prototype.</span>decrypt (sessionKeyAlgorithm, key)](#apidoc.element.openpgp.packet.SymEncryptedAEADProtected.prototype.decrypt)
- description and source-code
```javascript
decrypt = function (sessionKeyAlgorithm, key) {
  var _this = this;

  return _crypto2.default.gcm.decrypt(sessionKeyAlgorithm, this.encrypted, key, this.iv).then(function (decrypted) {
    _this.packets.read(decrypted);
  });
}
```
- example usage
```shell
...
'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
'''

#### Encrypt and decrypt *String* data with PGP keys

'''js
...
```

#### <a name="apidoc.element.openpgp.packet.SymEncryptedAEADProtected.prototype.encrypt"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedAEADProtected.prototype.</span>encrypt (sessionKeyAlgorithm, key)](#apidoc.element.openpgp.packet.SymEncryptedAEADProtected.prototype.encrypt)
- description and source-code
```javascript
encrypt = function (sessionKeyAlgorithm, key) {
  var _this2 = this;

  this.iv = _crypto2.default.random.getRandomValues(new Uint8Array(IV_LEN)); // generate new random IV
  return _crypto2.default.gcm.encrypt(sessionKeyAlgorithm, this.packets.write(), key, this.iv).then(function (encrypted) {
    _this2.encrypted = encrypted;
  });
}
```
- example usage
```shell
...

options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
...
```

#### <a name="apidoc.element.openpgp.packet.SymEncryptedAEADProtected.prototype.read"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedAEADProtected.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.SymEncryptedAEADProtected.prototype.read)
- description and source-code
```javascript
read = function (bytes) {
  var offset = 0;
  if (bytes[offset] !== VERSION) {
    // The only currently defined value is 1.
    throw new Error('Invalid packet version.');
  }
  offset++;
  this.iv = bytes.subarray(offset, IV_LEN + offset);
  offset += IV_LEN;
  this.encrypted = bytes.subarray(offset, bytes.length);
}
```
- example usage
```shell
...
openpgp.encrypt(options).then(function(ciphertext) {
    encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
...
```

#### <a name="apidoc.element.openpgp.packet.SymEncryptedAEADProtected.prototype.write"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedAEADProtected.prototype.</span>write ()](#apidoc.element.openpgp.packet.SymEncryptedAEADProtected.prototype.write)
- description and source-code
```javascript
write = function () {
  return _util2.default.concatUint8Array([new Uint8Array([this.version]), this.iv, this.encrypted]);
}
```
- example usage
```shell
...
options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
password: 'secret stuff',                 // decrypt with password
...
```



# <a name="apidoc.module.openpgp.packet.SymEncryptedIntegrityProtected"></a>[module openpgp.packet.SymEncryptedIntegrityProtected](#apidoc.module.openpgp.packet.SymEncryptedIntegrityProtected)

#### <a name="apidoc.element.openpgp.packet.SymEncryptedIntegrityProtected.SymEncryptedIntegrityProtected"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>SymEncryptedIntegrityProtected ()](#apidoc.element.openpgp.packet.SymEncryptedIntegrityProtected.SymEncryptedIntegrityProtected)
- description and source-code
```javascript
function SymEncryptedIntegrityProtected() {
  this.tag = _enums2.default.packet.symEncryptedIntegrityProtected;
  this.version = VERSION;
<span class="apidocCodeCommentSpan">  /** The encrypted payload. */
</span>  this.encrypted = null; // string
  /**
   * If after decrypting the packet this is set to true,
   * a modification has been detected and thus the contents
   * should be discarded.
   * @type {Boolean}
   */
  this.modification = false;
  this.packets = null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet.SymEncryptedIntegrityProtected.prototype"></a>[module openpgp.packet.SymEncryptedIntegrityProtected.prototype](#apidoc.module.openpgp.packet.SymEncryptedIntegrityProtected.prototype)

#### <a name="apidoc.element.openpgp.packet.SymEncryptedIntegrityProtected.prototype.decrypt"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedIntegrityProtected.prototype.</span>decrypt (sessionKeyAlgorithm, key)](#apidoc.element.openpgp.packet.SymEncryptedIntegrityProtected.prototype.decrypt)
- description and source-code
```javascript
decrypt = function (sessionKeyAlgorithm, key) {
  var decrypted = void 0;
  if (sessionKeyAlgorithm.substr(0, 3) === 'aes') {
    // AES optimizations. Native code for node, asmCrypto for browser.
    decrypted = aesDecrypt(sessionKeyAlgorithm, this.encrypted, key);
  } else {
    decrypted = _crypto2.default.cfb.decrypt(sessionKeyAlgorithm, key, this.encrypted, false);
  }

  // there must be a modification detection code packet as the
  // last packet and everything gets hashed except the hash itself
  var prefix = _crypto2.default.cfb.mdc(sessionKeyAlgorithm, key, this.encrypted);
  var bytes = decrypted.subarray(0, decrypted.length - 20);
  var tohash = _util2.default.concatUint8Array([prefix, bytes]);
  this.hash = _util2.default.Uint8Array2str(_crypto2.default.hash.sha1(tohash));
  var mdc = _util2.default.Uint8Array2str(decrypted.subarray(decrypted.length - 20, decrypted.length));

  if (this.hash !== mdc) {
    throw new Error('Modification detected.');
  } else {
    this.packets.read(decrypted.subarray(0, decrypted.length - 22));
  }

  return Promise.resolve();
}
```
- example usage
```shell
...
'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
'''

#### Encrypt and decrypt *String* data with PGP keys

'''js
...
```

#### <a name="apidoc.element.openpgp.packet.SymEncryptedIntegrityProtected.prototype.encrypt"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedIntegrityProtected.prototype.</span>encrypt (sessionKeyAlgorithm, key)](#apidoc.element.openpgp.packet.SymEncryptedIntegrityProtected.prototype.encrypt)
- description and source-code
```javascript
encrypt = function (sessionKeyAlgorithm, key) {
  var bytes = this.packets.write();
  var prefixrandom = _crypto2.default.getPrefixRandom(sessionKeyAlgorithm);
  var repeat = new Uint8Array([prefixrandom[prefixrandom.length - 2], prefixrandom[prefixrandom.length - 1]]);
  var prefix = _util2.default.concatUint8Array([prefixrandom, repeat]);
  var mdc = new Uint8Array([0xD3, 0x14]); // modification detection code packet

  var tohash = _util2.default.concatUint8Array([bytes, mdc]);
  var hash = _crypto2.default.hash.sha1(_util2.default.concatUint8Array([prefix, tohash]));
  tohash = _util2.default.concatUint8Array([tohash, hash]);

  if (sessionKeyAlgorithm.substr(0, 3) === 'aes') {
    // AES optimizations. Native code for node, asmCrypto for browser.
    this.encrypted = aesEncrypt(sessionKeyAlgorithm, prefix, tohash, key);
  } else {
    this.encrypted = _crypto2.default.cfb.encrypt(prefixrandom, sessionKeyAlgorithm, tohash, key, false);
    this.encrypted = this.encrypted.subarray(0, prefix.length + tohash.length);
  }

  return Promise.resolve();
}
```
- example usage
```shell
...

options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
...
```

#### <a name="apidoc.element.openpgp.packet.SymEncryptedIntegrityProtected.prototype.read"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedIntegrityProtected.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.SymEncryptedIntegrityProtected.prototype.read)
- description and source-code
```javascript
read = function (bytes) {
  // - A one-octet version number. The only currently defined value is 1.
  if (bytes[0] !== VERSION) {
    throw new Error('Invalid packet version.');
  }

  // - Encrypted data, the output of the selected symmetric-key cipher
  //   operating in Cipher Feedback mode with shift amount equal to the
  //   block size of the cipher (CFB-n where n is the block size).
  this.encrypted = bytes.subarray(1, bytes.length);
}
```
- example usage
```shell
...
openpgp.encrypt(options).then(function(ciphertext) {
    encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
...
```

#### <a name="apidoc.element.openpgp.packet.SymEncryptedIntegrityProtected.prototype.write"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedIntegrityProtected.prototype.</span>write ()](#apidoc.element.openpgp.packet.SymEncryptedIntegrityProtected.prototype.write)
- description and source-code
```javascript
write = function () {
  return _util2.default.concatUint8Array([new Uint8Array([VERSION]), this.encrypted]);
}
```
- example usage
```shell
...
options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
password: 'secret stuff',                 // decrypt with password
...
```



# <a name="apidoc.module.openpgp.packet.SymEncryptedSessionKey"></a>[module openpgp.packet.SymEncryptedSessionKey](#apidoc.module.openpgp.packet.SymEncryptedSessionKey)

#### <a name="apidoc.element.openpgp.packet.SymEncryptedSessionKey.SymEncryptedSessionKey"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>SymEncryptedSessionKey ()](#apidoc.element.openpgp.packet.SymEncryptedSessionKey.SymEncryptedSessionKey)
- description and source-code
```javascript
function SymEncryptedSessionKey() {
  this.tag = _enums2.default.packet.symEncryptedSessionKey;
  this.version = 4;
  this.sessionKey = null;
  this.sessionKeyEncryptionAlgorithm = null;
  this.sessionKeyAlgorithm = 'aes256';
  this.encrypted = null;
  this.s2k = new _s2k2.default();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet.SymEncryptedSessionKey.prototype"></a>[module openpgp.packet.SymEncryptedSessionKey.prototype](#apidoc.module.openpgp.packet.SymEncryptedSessionKey.prototype)

#### <a name="apidoc.element.openpgp.packet.SymEncryptedSessionKey.prototype.decrypt"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedSessionKey.prototype.</span>decrypt (passphrase)](#apidoc.element.openpgp.packet.SymEncryptedSessionKey.prototype.decrypt)
- description and source-code
```javascript
decrypt = function (passphrase) {
  var algo = this.sessionKeyEncryptionAlgorithm !== null ? this.sessionKeyEncryptionAlgorithm : this.sessionKeyAlgorithm;

  var length = _crypto2.default.cipher[algo].keySize;
  var key = this.s2k.produce_key(passphrase, length);

  if (this.encrypted === null) {
    this.sessionKey = key;
  } else {
    var decrypted = _crypto2.default.cfb.normalDecrypt(algo, key, this.encrypted, null);

    this.sessionKeyAlgorithm = _enums2.default.read(_enums2.default.symmetric, decrypted[0]);

    this.sessionKey = decrypted.subarray(1, decrypted.length);
  }
}
```
- example usage
```shell
...
'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
'''

#### Encrypt and decrypt *String* data with PGP keys

'''js
...
```

#### <a name="apidoc.element.openpgp.packet.SymEncryptedSessionKey.prototype.encrypt"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedSessionKey.prototype.</span>encrypt (passphrase)](#apidoc.element.openpgp.packet.SymEncryptedSessionKey.prototype.encrypt)
- description and source-code
```javascript
encrypt = function (passphrase) {
  var algo = this.sessionKeyEncryptionAlgorithm !== null ? this.sessionKeyEncryptionAlgorithm : this.sessionKeyAlgorithm;

  this.sessionKeyEncryptionAlgorithm = algo;

  var length = _crypto2.default.cipher[algo].keySize;
  var key = this.s2k.produce_key(passphrase, length);

  var algo_enum = new Uint8Array([_enums2.default.write(_enums2.default.symmetric, this.sessionKeyAlgorithm)]);

  var private_key;
  if (this.sessionKey === null) {
    this.sessionKey = _crypto2.default.getRandomBytes(_crypto2.default.cipher[this.sessionKeyAlgorithm].keySize);
  }
  private_key = _util2.default.concatUint8Array([algo_enum, this.sessionKey]);

  this.encrypted = _crypto2.default.cfb.normalEncrypt(algo, key, private_key, null);
}
```
- example usage
```shell
...

options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
...
```

#### <a name="apidoc.element.openpgp.packet.SymEncryptedSessionKey.prototype.postCloneTypeFix"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedSessionKey.prototype.</span>postCloneTypeFix ()](#apidoc.element.openpgp.packet.SymEncryptedSessionKey.prototype.postCloneTypeFix)
- description and source-code
```javascript
postCloneTypeFix = function () {
  this.s2k = _s2k2.default.fromClone(this.s2k);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.SymEncryptedSessionKey.prototype.read"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedSessionKey.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.SymEncryptedSessionKey.prototype.read)
- description and source-code
```javascript
read = function (bytes) {
  // A one-octet version number. The only currently defined version is 4.
  this.version = bytes[0];

  // A one-octet number describing the symmetric algorithm used.
  var algo = _enums2.default.read(_enums2.default.symmetric, bytes[1]);

  // A string-to-key (S2K) specifier, length as defined above.
  var s2klength = this.s2k.read(bytes.subarray(2, bytes.length));

  // Optionally, the encrypted session key itself, which is decrypted
  // with the string-to-key object.
  var done = s2klength + 2;

  if (done < bytes.length) {
    this.encrypted = bytes.subarray(done, bytes.length);
    this.sessionKeyEncryptionAlgorithm = algo;
  } else {
    this.sessionKeyAlgorithm = algo;
  }
}
```
- example usage
```shell
...
openpgp.encrypt(options).then(function(ciphertext) {
    encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
...
```

#### <a name="apidoc.element.openpgp.packet.SymEncryptedSessionKey.prototype.write"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SymEncryptedSessionKey.prototype.</span>write ()](#apidoc.element.openpgp.packet.SymEncryptedSessionKey.prototype.write)
- description and source-code
```javascript
write = function () {
  var algo = this.encrypted === null ? this.sessionKeyAlgorithm : this.sessionKeyEncryptionAlgorithm;

  var bytes = _util2.default.concatUint8Array([new Uint8Array([this.version, _enums2.default.write(_enums2.default.symmetric, algo
)]), this.s2k.write()]);

  if (this.encrypted !== null) {
    bytes = _util2.default.concatUint8Array([bytes, this.encrypted]);
  }
  return bytes;
}
```
- example usage
```shell
...
options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
password: 'secret stuff',                 // decrypt with password
...
```



# <a name="apidoc.module.openpgp.packet.SymmetricallyEncrypted"></a>[module openpgp.packet.SymmetricallyEncrypted](#apidoc.module.openpgp.packet.SymmetricallyEncrypted)

#### <a name="apidoc.element.openpgp.packet.SymmetricallyEncrypted.SymmetricallyEncrypted"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>SymmetricallyEncrypted ()](#apidoc.element.openpgp.packet.SymmetricallyEncrypted.SymmetricallyEncrypted)
- description and source-code
```javascript
function SymmetricallyEncrypted() {
  this.tag = _enums2.default.packet.symmetricallyEncrypted;
  this.encrypted = null;
<span class="apidocCodeCommentSpan">  /** Decrypted packets contained within.
   * @type {module:packet/packetlist} */
</span>  this.packets = null;
  this.ignore_mdc_error = _config2.default.ignore_mdc_error;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet.SymmetricallyEncrypted.prototype"></a>[module openpgp.packet.SymmetricallyEncrypted.prototype](#apidoc.module.openpgp.packet.SymmetricallyEncrypted.prototype)

#### <a name="apidoc.element.openpgp.packet.SymmetricallyEncrypted.prototype.decrypt"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SymmetricallyEncrypted.prototype.</span>decrypt (sessionKeyAlgorithm, key)](#apidoc.element.openpgp.packet.SymmetricallyEncrypted.prototype.decrypt)
- description and source-code
```javascript
decrypt = function (sessionKeyAlgorithm, key) {
  var decrypted = _crypto2.default.cfb.decrypt(sessionKeyAlgorithm, key, this.encrypted, true);
  // for modern cipher (blocklength != 64 bit, except for Twofish) MDC is required
  if (!this.ignore_mdc_error && (sessionKeyAlgorithm === 'aes128' || sessionKeyAlgorithm === 'aes192' || sessionKeyAlgorithm === '
aes256')) {
    throw new Error('Decryption failed due to missing MDC in combination with modern cipher.');
  }
  this.packets.read(decrypted);

  return Promise.resolve();
}
```
- example usage
```shell
...
'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
'''

#### Encrypt and decrypt *String* data with PGP keys

'''js
...
```

#### <a name="apidoc.element.openpgp.packet.SymmetricallyEncrypted.prototype.encrypt"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SymmetricallyEncrypted.prototype.</span>encrypt (algo, key)](#apidoc.element.openpgp.packet.SymmetricallyEncrypted.prototype.encrypt)
- description and source-code
```javascript
encrypt = function (algo, key) {
  var data = this.packets.write();

  this.encrypted = _crypto2.default.cfb.encrypt(_crypto2.default.getPrefixRandom(algo), algo, data, key, true);

  return Promise.resolve();
}
```
- example usage
```shell
...

options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
...
```

#### <a name="apidoc.element.openpgp.packet.SymmetricallyEncrypted.prototype.read"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SymmetricallyEncrypted.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.SymmetricallyEncrypted.prototype.read)
- description and source-code
```javascript
read = function (bytes) {
  this.encrypted = bytes;
}
```
- example usage
```shell
...
openpgp.encrypt(options).then(function(ciphertext) {
    encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
...
```

#### <a name="apidoc.element.openpgp.packet.SymmetricallyEncrypted.prototype.write"></a>[function <span class="apidocSignatureSpan">openpgp.packet.SymmetricallyEncrypted.prototype.</span>write ()](#apidoc.element.openpgp.packet.SymmetricallyEncrypted.prototype.write)
- description and source-code
```javascript
write = function () {
  return this.encrypted;
}
```
- example usage
```shell
...
options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
password: 'secret stuff',                 // decrypt with password
...
```



# <a name="apidoc.module.openpgp.packet.Trust"></a>[module openpgp.packet.Trust](#apidoc.module.openpgp.packet.Trust)

#### <a name="apidoc.element.openpgp.packet.Trust.Trust"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>Trust ()](#apidoc.element.openpgp.packet.Trust.Trust)
- description and source-code
```javascript
function Trust() {
  this.tag = _enums2.default.packet.trust;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet.Trust.prototype"></a>[module openpgp.packet.Trust.prototype](#apidoc.module.openpgp.packet.Trust.prototype)

#### <a name="apidoc.element.openpgp.packet.Trust.prototype.read"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Trust.prototype.</span>read ()](#apidoc.element.openpgp.packet.Trust.prototype.read)
- description and source-code
```javascript
read = function () {}
```
- example usage
```shell
...
openpgp.encrypt(options).then(function(ciphertext) {
    encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
...
```



# <a name="apidoc.module.openpgp.packet.UserAttribute"></a>[module openpgp.packet.UserAttribute](#apidoc.module.openpgp.packet.UserAttribute)

#### <a name="apidoc.element.openpgp.packet.UserAttribute.UserAttribute"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>UserAttribute ()](#apidoc.element.openpgp.packet.UserAttribute.UserAttribute)
- description and source-code
```javascript
function UserAttribute() {
  this.tag = _enums2.default.packet.userAttribute;
  this.attributes = [];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet.UserAttribute.prototype"></a>[module openpgp.packet.UserAttribute.prototype](#apidoc.module.openpgp.packet.UserAttribute.prototype)

#### <a name="apidoc.element.openpgp.packet.UserAttribute.prototype.equals"></a>[function <span class="apidocSignatureSpan">openpgp.packet.UserAttribute.prototype.</span>equals (usrAttr)](#apidoc.element.openpgp.packet.UserAttribute.prototype.equals)
- description and source-code
```javascript
equals = function (usrAttr) {
  if (!usrAttr || !(usrAttr instanceof UserAttribute)) {
    return false;
  }
  return this.attributes.every(function (attr, index) {
    return attr === usrAttr.attributes[index];
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.UserAttribute.prototype.read"></a>[function <span class="apidocSignatureSpan">openpgp.packet.UserAttribute.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.UserAttribute.prototype.read)
- description and source-code
```javascript
read = function (bytes) {
  var i = 0;
  while (i < bytes.length) {
    var len = _packet2.default.readSimpleLength(bytes.subarray(i, bytes.length));
    i += len.offset;

    this.attributes.push(_util2.default.Uint8Array2str(bytes.subarray(i, i + len.len)));
    i += len.len;
  }
}
```
- example usage
```shell
...
openpgp.encrypt(options).then(function(ciphertext) {
    encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
...
```

#### <a name="apidoc.element.openpgp.packet.UserAttribute.prototype.write"></a>[function <span class="apidocSignatureSpan">openpgp.packet.UserAttribute.prototype.</span>write ()](#apidoc.element.openpgp.packet.UserAttribute.prototype.write)
- description and source-code
```javascript
write = function () {
  var arr = [];
  for (var i = 0; i < this.attributes.length; i++) {
    arr.push(_packet2.default.writeSimpleLength(this.attributes[i].length));
    arr.push(_util2.default.str2Uint8Array(this.attributes[i]));
  }
  return _util2.default.concatUint8Array(arr);
}
```
- example usage
```shell
...
options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
password: 'secret stuff',                 // decrypt with password
...
```



# <a name="apidoc.module.openpgp.packet.Userid"></a>[module openpgp.packet.Userid](#apidoc.module.openpgp.packet.Userid)

#### <a name="apidoc.element.openpgp.packet.Userid.Userid"></a>[function <span class="apidocSignatureSpan">openpgp.packet.</span>Userid ()](#apidoc.element.openpgp.packet.Userid.Userid)
- description and source-code
```javascript
function Userid() {
  this.tag = _enums2.default.packet.userid;
<span class="apidocCodeCommentSpan">  /** A string containing the user id. Usually in the form
   * John Doe <john@example.com>
   * @type {String}
   */
</span>  this.userid = '';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.packet.Userid.prototype"></a>[module openpgp.packet.Userid.prototype](#apidoc.module.openpgp.packet.Userid.prototype)

#### <a name="apidoc.element.openpgp.packet.Userid.prototype.read"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Userid.prototype.</span>read (bytes)](#apidoc.element.openpgp.packet.Userid.prototype.read)
- description and source-code
```javascript
read = function (bytes) {
  this.userid = _util2.default.decode_utf8(_util2.default.Uint8Array2str(bytes));
}
```
- example usage
```shell
...
openpgp.encrypt(options).then(function(ciphertext) {
    encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
...
```

#### <a name="apidoc.element.openpgp.packet.Userid.prototype.write"></a>[function <span class="apidocSignatureSpan">openpgp.packet.Userid.prototype.</span>write ()](#apidoc.element.openpgp.packet.Userid.prototype.write)
- description and source-code
```javascript
write = function () {
  return _util2.default.str2Uint8Array(_util2.default.encode_utf8(this.userid));
}
```
- example usage
```shell
...
options = {
data: new Uint8Array([0x01, 0x01, 0x01]), // input as Uint8Array (or String)
passwords: ['secret stuff'],              // multiple passwords possible
armor: false                              // don't ASCII armor (for Uint8Array output)
};

openpgp.encrypt(options).then(function(ciphertext) {
encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
message: openpgp.message.read(encrypted), // parse encrypted bytes
password: 'secret stuff',                 // decrypt with password
...
```



# <a name="apidoc.module.openpgp.packet.clone"></a>[module openpgp.packet.clone](#apidoc.module.openpgp.packet.clone)

#### <a name="apidoc.element.openpgp.packet.clone.clonePackets"></a>[function <span class="apidocSignatureSpan">openpgp.packet.clone.</span>clonePackets (options)](#apidoc.element.openpgp.packet.clone.clonePackets)
- description and source-code
```javascript
function clonePackets(options) {
  if (options.publicKeys) {
    options.publicKeys = options.publicKeys.map(function (key) {
      return key.toPacketlist();
    });
  }
  if (options.privateKeys) {
    options.privateKeys = options.privateKeys.map(function (key) {
      return key.toPacketlist();
    });
  }
  if (options.privateKey) {
    options.privateKey = options.privateKey.toPacketlist();
  }
  if (options.key) {
    options.key = options.key.toPacketlist();
  }
  if (options.message) {
    //could be either a Message or CleartextMessage object
    if (options.message instanceof message.Message) {
      options.message = options.message.packets;
    } else if (options.message instanceof cleartext.CleartextMessage) {
      options.message.signature = options.message.signature.packets;
    }
  }
  if (options.signature && options.signature instanceof signature.Signature) {
    options.signature = options.signature.packets;
  }
  if (options.signatures) {
    options.signatures = options.signatures.map(function (sig) {
      return verificationObjectToClone(sig);
    });
  }
  return options;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.packet.clone.parseClonedPackets"></a>[function <span class="apidocSignatureSpan">openpgp.packet.clone.</span>parseClonedPackets (options, method)](#apidoc.element.openpgp.packet.clone.parseClonedPackets)
- description and source-code
```javascript
function parseClonedPackets(options, method) {
  if (options.publicKeys) {
    options.publicKeys = options.publicKeys.map(packetlistCloneToKey);
  }
  if (options.privateKeys) {
    options.privateKeys = options.privateKeys.map(packetlistCloneToKey);
  }
  if (options.privateKey) {
    options.privateKey = packetlistCloneToKey(options.privateKey);
  }
  if (options.key) {
    options.key = packetlistCloneToKey(options.key);
  }
  if (options.message && (method === 'sign' || method === 'verify')) {
    // sign and verify support only CleartextMessage
    options.message = packetlistCloneToCleartextMessage(options.message);
  } else if (options.message) {
    options.message = packetlistCloneToMessage(options.message);
  }
  if (options.signatures) {
    options.signatures = options.signatures.map(packetlistCloneToSignatures);
  }
  if (options.signature) {
    options.signature = packetlistCloneToSignature(options.signature);
  }
  return options;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.signature"></a>[module openpgp.signature](#apidoc.module.openpgp.signature)

#### <a name="apidoc.element.openpgp.signature.Signature"></a>[function <span class="apidocSignatureSpan">openpgp.signature.</span>Signature (packetlist)](#apidoc.element.openpgp.signature.Signature)
- description and source-code
```javascript
function Signature(packetlist) {
  if (!(this instanceof Signature)) {
    return new Signature(packetlist);
  }
  this.packets = packetlist || new _packet2.default.List();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.signature.read"></a>[function <span class="apidocSignatureSpan">openpgp.signature.</span>read (input)](#apidoc.element.openpgp.signature.read)
- description and source-code
```javascript
function read(input) {
  var packetlist = new _packet2.default.List();
  packetlist.read(input);
  return new Signature(packetlist);
}
```
- example usage
```shell
...
openpgp.encrypt(options).then(function(ciphertext) {
    encrypted = ciphertext.message.packets.write(); // get raw encrypted packets as Uint8Array
});
'''

'''js
options = {
    message: openpgp.message.read(encrypted), // parse encrypted bytes
    password: 'secret stuff',                 // decrypt with password
    format: 'binary'                          // output as Uint8Array
};

openpgp.decrypt(options).then(function(plaintext) {
    return plaintext.data // Uint8Array([0x01, 0x01, 0x01])
});
...
```

#### <a name="apidoc.element.openpgp.signature.readArmored"></a>[function <span class="apidocSignatureSpan">openpgp.signature.</span>readArmored (armoredText)](#apidoc.element.openpgp.signature.readArmored)
- description and source-code
```javascript
function readArmored(armoredText) {
  var input = _armor2.default.decode(armoredText).data;
  return read(input);
}
```
- example usage
```shell
...
'''js
var options, encrypted;

var pubkey = '-----BEGIN PGP PUBLIC KEY BLOCK ... END PGP PUBLIC KEY BLOCK-----';
var privkey = '-----BEGIN PGP PRIVATE KEY BLOCK ... END PGP PRIVATE KEY BLOCK-----'; //encrypted private key
var passphrase = 'secret passphrase'; //what the privKey is encrypted with

var privKeyObj = openpgp.key.readArmored(privkey).keys[0];
privKeyObj.decrypt(passphrase);

options = {
    data: 'Hello, World!',                             // input as String (or Uint8Array)
    publicKeys: openpgp.key.readArmored(pubkey).keys,  // for encryption
    privateKeys: privKeyObj // for signing (optional)
};
...
```



# <a name="apidoc.module.openpgp.signature.Signature"></a>[module openpgp.signature.Signature](#apidoc.module.openpgp.signature.Signature)

#### <a name="apidoc.element.openpgp.signature.Signature.Signature"></a>[function <span class="apidocSignatureSpan">openpgp.signature.</span>Signature (packetlist)](#apidoc.element.openpgp.signature.Signature.Signature)
- description and source-code
```javascript
function Signature(packetlist) {
  if (!(this instanceof Signature)) {
    return new Signature(packetlist);
  }
  this.packets = packetlist || new _packet2.default.List();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.signature.Signature.prototype"></a>[module openpgp.signature.Signature.prototype](#apidoc.module.openpgp.signature.Signature.prototype)

#### <a name="apidoc.element.openpgp.signature.Signature.prototype.armor"></a>[function <span class="apidocSignatureSpan">openpgp.signature.Signature.prototype.</span>armor ()](#apidoc.element.openpgp.signature.Signature.prototype.armor)
- description and source-code
```javascript
armor = function () {
  return _armor2.default.encode(_enums2.default.armor.signature, this.packets.write());
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.openpgp.util"></a>[module openpgp.util](#apidoc.module.openpgp.util)

#### <a name="apidoc.element.openpgp.util.Uint8Array2str"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>Uint8Array2str (bin)](#apidoc.element.openpgp.util.Uint8Array2str)
- description and source-code
```javascript
function Uint8Array2str(bin) {
  if (!Uint8Array.prototype.isPrototypeOf(bin)) {
    throw new Error('Uint8Array2str: Data must be in the form of a Uint8Array');
  }

  var result = [],
      bs = 16384,
      j = bin.length;

  for (var i = 0; i < j; i += bs) {
    result.push(String.fromCharCode.apply(String, bin.subarray(i, i + bs < j ? i + bs : j)));
  }
  return result.join('');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.bin2str"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>bin2str (bin)](#apidoc.element.openpgp.util.bin2str)
- description and source-code
```javascript
function bin2str(bin) {
  var result = [];
  for (var i = 0; i < bin.length; i++) {
    result[i] = String.fromCharCode(bin[i]);
  }
  return result.join('');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.calc_checksum"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>calc_checksum (text)](#apidoc.element.openpgp.util.calc_checksum)
- description and source-code
```javascript
function calc_checksum(text) {
  var checksum = {
    s: 0,
    add: function add(sadd) {
      this.s = (this.s + sadd) % 65536;
    }
  };
  for (var i = 0; i < text.length; i++) {
    checksum.add(text[i]);
  }
  return checksum.s;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.collectBuffers"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>collectBuffers (obj, collection)](#apidoc.element.openpgp.util.collectBuffers)
- description and source-code
```javascript
function collectBuffers(obj, collection) {
  if (!obj) {
    return;
  }
  if (this.isUint8Array(obj) && collection.indexOf(obj.buffer) === -1) {
    collection.push(obj.buffer);
    return;
  }
  if (Object.prototype.isPrototypeOf(obj)) {
    for (var key in obj) {
      // recursively search all children
      this.collectBuffers(obj[key], collection);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.concatUint8Array"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>concatUint8Array (arrays)](#apidoc.element.openpgp.util.concatUint8Array)
- description and source-code
```javascript
function concatUint8Array(arrays) {
  var totalLength = 0;
  arrays.forEach(function (element) {
    if (!Uint8Array.prototype.isPrototypeOf(element)) {
      throw new Error('concatUint8Array: Data must be in the form of a Uint8Array');
    }

    totalLength += element.length;
  });

  var result = new Uint8Array(totalLength);
  var pos = 0;
  arrays.forEach(function (element) {
    result.set(element, pos);
    pos += element.length;
  });

  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.copyUint8Array"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>copyUint8Array (array)](#apidoc.element.openpgp.util.copyUint8Array)
- description and source-code
```javascript
function copyUint8Array(array) {
  if (!Uint8Array.prototype.isPrototypeOf(array)) {
    throw new Error('Data must be in the form of a Uint8Array');
  }

  var copy = new Uint8Array(array.length);
  copy.set(array);
  return copy;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.decode_utf8"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>decode_utf8 (utf8)](#apidoc.element.openpgp.util.decode_utf8)
- description and source-code
```javascript
function decode_utf8(utf8) {
  if (typeof utf8 !== 'string') {
    throw new Error('Parameter "utf8" is not of type string');
  }
  try {
    return decodeURIComponent(escape(utf8));
  } catch (e) {
    return utf8;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.detectNode"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>detectNode ()](#apidoc.element.openpgp.util.detectNode)
- description and source-code
```javascript
function detectNode() {
  return typeof window === 'undefined';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.encode_utf8"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>encode_utf8 (str)](#apidoc.element.openpgp.util.encode_utf8)
- description and source-code
```javascript
function encode_utf8(str) {
  return unescape(encodeURIComponent(str));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.equalsUint8Array"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>equalsUint8Array (array1, array2)](#apidoc.element.openpgp.util.equalsUint8Array)
- description and source-code
```javascript
function equalsUint8Array(array1, array2) {
  if (!Uint8Array.prototype.isPrototypeOf(array1) || !Uint8Array.prototype.isPrototypeOf(array2)) {
    throw new Error('Data must be in the form of a Uint8Array');
  }

  if (array1.length !== array2.length) {
    return false;
  }

  for (var i = 0; i < array1.length; i++) {
    if (array1[i] !== array2[i]) {
      return false;
    }
  }
  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.getLeftNBits"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>getLeftNBits (string, bitcount)](#apidoc.element.openpgp.util.getLeftNBits)
- description and source-code
```javascript
function getLeftNBits(string, bitcount) {
  var rest = bitcount % 8;
  if (rest === 0) {
    return string.substring(0, bitcount / 8);
  }
  var bytes = (bitcount - rest) / 8 + 1;
  var result = string.substring(0, bytes);
  return this.shiftRight(result, 8 - rest); // +String.fromCharCode(string.charCodeAt(bytes -1) << (8-rest) & 0xFF);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.getNodeBuffer"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>getNodeBuffer ()](#apidoc.element.openpgp.util.getNodeBuffer)
- description and source-code
```javascript
function getNodeBuffer() {
  if (!this.detectNode()) {
    return;
  }

  return _dereq_('buffer').Buffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.getNodeCrypto"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>getNodeCrypto ()](#apidoc.element.openpgp.util.getNodeCrypto)
- description and source-code
```javascript
function getNodeCrypto() {
  if (!this.detectNode() || !_config2.default.use_native) {
    return;
  }

  return _dereq_('crypto');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.getTransferables"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>getTransferables (obj)](#apidoc.element.openpgp.util.getTransferables)
- description and source-code
```javascript
function getTransferables(obj) {
  if (_config2.default.zero_copy && Object.prototype.isPrototypeOf(obj)) {
    var transferables = [];
    this.collectBuffers(obj, transferables);
    return transferables.length ? transferables : undefined;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.getWebCrypto"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>getWebCrypto ()](#apidoc.element.openpgp.util.getWebCrypto)
- description and source-code
```javascript
function getWebCrypto() {
  if (!_config2.default.use_native) {
    return;
  }

  return typeof window !== 'undefined' && window.crypto && window.crypto.subtle;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.getWebCryptoAll"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>getWebCryptoAll ()](#apidoc.element.openpgp.util.getWebCryptoAll)
- description and source-code
```javascript
function getWebCryptoAll() {
  if (!_config2.default.use_native) {
    return;
  }

  if (typeof window !== 'undefined') {
    if (window.crypto) {
      return window.crypto.subtle || window.crypto.webkitSubtle;
    }
    if (window.msCrypto) {
      return window.msCrypto.subtle;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.get_hashAlgorithmString"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>get_hashAlgorithmString (algo)](#apidoc.element.openpgp.util.get_hashAlgorithmString)
- description and source-code
```javascript
function get_hashAlgorithmString(algo) {
  switch (algo) {
    case 1:
      return "MD5";
    case 2:
      return "SHA1";
    case 3:
      return "RIPEMD160";
    case 8:
      return "SHA256";
    case 9:
      return "SHA384";
    case 10:
      return "SHA512";
    case 11:
      return "SHA224";
  }
  return "unknown";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.hex2bin"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>hex2bin (hex)](#apidoc.element.openpgp.util.hex2bin)
- description and source-code
```javascript
function hex2bin(hex) {
  var str = '';
  for (var i = 0; i < hex.length; i += 2) {
    str += String.fromCharCode(parseInt(hex.substr(i, 2), 16));
  }
  return str;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.hexdump"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>hexdump (str)](#apidoc.element.openpgp.util.hexdump)
- description and source-code
```javascript
function hexdump(str) {
  var r = [];
  var e = str.length;
  var c = 0;
  var h;
  var i = 0;
  while (c < e) {
    h = str.charCodeAt(c++).toString(16);
    while (h.length < 2) {
      h = "0" + h;
    }
    r.push(" " + h);
    i++;
    if (i % 32 === 0) {
      r.push("\n           ");
    }
  }
  return r.join('');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.hexidump"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>hexidump (str)](#apidoc.element.openpgp.util.hexidump)
- description and source-code
```javascript
function hexidump(str) {
  var r = [];
  var e = str.length;
  var c = 0;
  var h;
  while (c < e) {
    h = str[c++].toString(16);
    while (h.length < 2) {
      h = "0" + h;
    }
    r.push("" + h);
  }
  return r.join('');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.hexstrdump"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>hexstrdump (str)](#apidoc.element.openpgp.util.hexstrdump)
- description and source-code
```javascript
function hexstrdump(str) {
  if (str === null) {
    return "";
  }
  var r = [];
  var e = str.length;
  var c = 0;
  var h;
  while (c < e) {
    h = str.charCodeAt(c++).toString(16);
    while (h.length < 2) {
      h = "0" + h;
    }
    r.push("" + h);
  }
  return r.join('');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.isArray"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>isArray (data)](#apidoc.element.openpgp.util.isArray)
- description and source-code
```javascript
function isArray(data) {
  return Array.prototype.isPrototypeOf(data);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.isEmailAddress"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>isEmailAddress (data)](#apidoc.element.openpgp.util.isEmailAddress)
- description and source-code
```javascript
function isEmailAddress(data) {
  if (!this.isString(data)) {
    return false;
  }
  var re = /^(([^<>()[\]\\.,;:\s@\"]+(\.[^<>()[\]\\.,;:\s@\"]+)*)|(\".+\"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([
a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/;
  return re.test(data);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.isString"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>isString (data)](#apidoc.element.openpgp.util.isString)
- description and source-code
```javascript
function isString(data) {
  return typeof data === 'string' || String.prototype.isPrototypeOf(data);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.isUint8Array"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>isUint8Array (data)](#apidoc.element.openpgp.util.isUint8Array)
- description and source-code
```javascript
function isUint8Array(data) {
  return Uint8Array.prototype.isPrototypeOf(data);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.isUserId"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>isUserId (data)](#apidoc.element.openpgp.util.isUserId)
- description and source-code
```javascript
function isUserId(data) {
  if (!this.isString(data)) {
    return false;
  }
  return (/</.test(data) && />$/.test(data)
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.print_debug"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>print_debug (str)](#apidoc.element.openpgp.util.print_debug)
- description and source-code
```javascript
function print_debug(str) {
  if (_config2.default.debug) {
    console.log(str);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.print_debug_hexstr_dump"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>print_debug_hexstr_dump (str, strToHex)](#apidoc.element.openpgp.util.print_debug_hexstr_dump)
- description and source-code
```javascript
function print_debug_hexstr_dump(str, strToHex) {
  if (_config2.default.debug) {
    str = str + this.hexstrdump(strToHex);
    console.log(str);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.promisify"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>promisify (fn)](#apidoc.element.openpgp.util.promisify)
- description and source-code
```javascript
function promisify(fn) {
  return function () {
    var args = arguments;
    return new Promise(function (resolve) {
      var result = fn.apply(null, args);
      resolve(result);
    });
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.promisifyIE11Op"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>promisifyIE11Op (cryptoOp, errmsg)](#apidoc.element.openpgp.util.promisifyIE11Op)
- description and source-code
```javascript
function promisifyIE11Op(cryptoOp, errmsg) {
  return new Promise(function (resolve, reject) {
    cryptoOp.onerror = function () {
      reject(new Error(errmsg));
    };
    cryptoOp.oncomplete = function (e) {
      resolve(e.target.result);
    };
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.readDate"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>readDate (bytes)](#apidoc.element.openpgp.util.readDate)
- description and source-code
```javascript
function readDate(bytes) {
  var n = this.readNumber(bytes);
  var d = new Date();
  d.setTime(n * 1000);
  return d;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.readNumber"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>readNumber (bytes)](#apidoc.element.openpgp.util.readNumber)
- description and source-code
```javascript
function readNumber(bytes) {
  var n = 0;

  for (var i = 0; i < bytes.length; i++) {
    n <<= 8;
    n += bytes[i];
  }

  return n;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.shiftRight"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>shiftRight (value, bitcount)](#apidoc.element.openpgp.util.shiftRight)
- description and source-code
```javascript
function shiftRight(value, bitcount) {
  var temp = this.str2bin(value);
  if (bitcount % 8 !== 0) {
    for (var i = temp.length - 1; i >= 0; i--) {
      temp[i] >>= bitcount % 8;
      if (i > 0) {
        temp[i] |= temp[i - 1] << 8 - bitcount % 8 & 0xFF;
      }
    }
  } else {
    return value;
  }
  return this.bin2str(temp);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.str2Uint8Array"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>str2Uint8Array (str)](#apidoc.element.openpgp.util.str2Uint8Array)
- description and source-code
```javascript
function str2Uint8Array(str) {
  if (typeof str !== 'string' && !String.prototype.isPrototypeOf(str)) {
    throw new Error('str2Uint8Array: Data must be in the form of a string');
  }

  var result = new Uint8Array(str.length);
  for (var i = 0; i < str.length; i++) {
    result[i] = str.charCodeAt(i);
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.str2bin"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>str2bin (str)](#apidoc.element.openpgp.util.str2bin)
- description and source-code
```javascript
function str2bin(str) {
  var result = [];
  for (var i = 0; i < str.length; i++) {
    result[i] = str.charCodeAt(i);
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.writeDate"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>writeDate (time)](#apidoc.element.openpgp.util.writeDate)
- description and source-code
```javascript
function writeDate(time) {
  var numeric = Math.round(time.getTime() / 1000);

  return this.writeNumber(numeric, 4);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.openpgp.util.writeNumber"></a>[function <span class="apidocSignatureSpan">openpgp.util.</span>writeNumber (n, bytes)](#apidoc.element.openpgp.util.writeNumber)
- description and source-code
```javascript
function writeNumber(n, bytes) {
  var b = new Uint8Array(bytes);
  for (var i = 0; i < bytes; i++) {
    b[i] = n >> 8 * (bytes - i - 1) & 0xFF;
  }

  return b;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
