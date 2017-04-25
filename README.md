# npmdoc-jimp

#### basic api documentation for  [jimp (v0.2.27)](https://github.com/oliver-moran/jimp#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-jimp.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-jimp) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-jimp.svg)](https://travis-ci.org/npmdoc/node-npmdoc-jimp)

#### An image processing library written entirely in JavaScript (i.e. zero external or native dependencies).

[![NPM](https://nodei.co/npm/jimp.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/jimp)

- [https://npmdoc.github.io/node-npmdoc-jimp/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-jimp/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-jimp/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-jimp/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-jimp/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-jimp/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Oliver Moran"
    },
    "bugs": {
        "url": "https://github.com/oliver-moran/jimp/issues"
    },
    "dependencies": {
        "bignumber.js": "^2.1.0",
        "bmp-js": "0.0.1",
        "es6-promise": "^3.0.2",
        "exif-parser": "^0.1.9",
        "file-type": "^3.1.0",
        "jpeg-js": "^0.2.0",
        "load-bmfont": "^1.2.3",
        "mime": "^1.3.4",
        "pixelmatch": "^4.0.0",
        "pngjs": "^3.0.0",
        "read-chunk": "^1.0.1",
        "request": "^2.65.0",
        "stream-to-buffer": "^0.1.0",
        "tinycolor2": "^1.1.2",
        "url-regex": "^3.0.0"
    },
    "description": "An image processing library written entirely in JavaScript (i.e. zero external or native dependencies).",
    "devDependencies": {
        "babel": "^6.0.14",
        "babel-cli": "^6.0.0",
        "babel-preset-es2015": "^6.0.14",
        "babel-preset-stage-0": "^6.0.14",
        "browserify": "^13.0.0",
        "envify": "^3.4.0",
        "express": "^4.13.4",
        "uglify-js": "^2.6.1",
        "uglifyify": "^3.0.1"
    },
    "directories": {},
    "dist": {
        "shasum": "41ef5082d8b63201d54747e04fe8bcacbaf25474",
        "tarball": "https://registry.npmjs.org/jimp/-/jimp-0.2.27.tgz"
    },
    "gitHead": "2dbb58f974dbd4f6639ca05edfd5a1f4eb1efd64",
    "homepage": "https://github.com/oliver-moran/jimp#readme",
    "keywords": [
        "image",
        "image processing",
        "image manipulation",
        "png",
        "jpg",
        "jpeg",
        "bmp",
        "resize",
        "scale",
        "crop"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "oliver.moran"
        }
    ],
    "name": "jimp",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/oliver-moran/jimp.git"
    },
    "scripts": {
        "minify-jimp": "uglifyjs browser/tmp.jimp.js --compress warnings=false --mangle -o browser/tmp.jimp.min.js",
        "prepublish": "./browser/browserify-build.sh",
        "start": "node server.js",
        "test": "./test/tests.sh"
    },
    "tonicExampleFilename": "example.js",
    "version": "0.2.27",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
