# api documentation for  [jimp (v0.2.27)](https://github.com/oliver-moran/jimp#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-jimp.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-jimp) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-jimp.svg)](https://travis-ci.org/npmdoc/node-npmdoc-jimp)
#### An image processing library written entirely in JavaScript (i.e. zero external or native dependencies).

[![NPM](https://nodei.co/npm/jimp.png?downloads=true)](https://www.npmjs.com/package/jimp)

[![apidoc](https://npmdoc.github.io/node-npmdoc-jimp/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-jimp%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-jimp/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-jimp/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-jimp/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Oliver Moran",
        "email": "oliver.moran@gmail.com"
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
            "name": "oliver.moran",
            "email": "oliver@nth-iteration.ie"
        }
    ],
    "name": "jimp",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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
    "version": "0.2.27"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module jimp](#apidoc.module.jimp)
1.  [function <span class="apidocSignatureSpan">jimp.</span>diff (img1, img2, threshold)](#apidoc.element.jimp.diff)
1.  [function <span class="apidocSignatureSpan">jimp.</span>distance (img1, img2)](#apidoc.element.jimp.distance)
1.  [function <span class="apidocSignatureSpan">jimp.</span>intToRGBA (i, cb)](#apidoc.element.jimp.intToRGBA)
1.  [function <span class="apidocSignatureSpan">jimp.</span>limit255 (n)](#apidoc.element.jimp.limit255)
1.  [function <span class="apidocSignatureSpan">jimp.</span>loadFont (file, cb)](#apidoc.element.jimp.loadFont)
1.  [function <span class="apidocSignatureSpan">jimp.</span>phash (size, smallerSize)](#apidoc.element.jimp.phash)
1.  [function <span class="apidocSignatureSpan">jimp.</span>read (src, cb)](#apidoc.element.jimp.read)
1.  [function <span class="apidocSignatureSpan">jimp.</span>resize (widthOriginal, heightOriginal, targetWidth, targetHeight, blendAlpha, interpolationPass, resizeCallback)](#apidoc.element.jimp.resize)
1.  [function <span class="apidocSignatureSpan">jimp.</span>rgbaToInt (r, g, b, a, cb)](#apidoc.element.jimp.rgbaToInt)
1.  number <span class="apidocSignatureSpan">jimp.</span>AUTO
1.  number <span class="apidocSignatureSpan">jimp.</span>HORIZONTAL_ALIGN_CENTER
1.  number <span class="apidocSignatureSpan">jimp.</span>HORIZONTAL_ALIGN_LEFT
1.  number <span class="apidocSignatureSpan">jimp.</span>HORIZONTAL_ALIGN_RIGHT
1.  number <span class="apidocSignatureSpan">jimp.</span>PNG_FILTER_AUTO
1.  number <span class="apidocSignatureSpan">jimp.</span>PNG_FILTER_AVERAGE
1.  number <span class="apidocSignatureSpan">jimp.</span>PNG_FILTER_NONE
1.  number <span class="apidocSignatureSpan">jimp.</span>PNG_FILTER_PAETH
1.  number <span class="apidocSignatureSpan">jimp.</span>PNG_FILTER_SUB
1.  number <span class="apidocSignatureSpan">jimp.</span>PNG_FILTER_UP
1.  number <span class="apidocSignatureSpan">jimp.</span>VERTICAL_ALIGN_BOTTOM
1.  number <span class="apidocSignatureSpan">jimp.</span>VERTICAL_ALIGN_MIDDLE
1.  number <span class="apidocSignatureSpan">jimp.</span>VERTICAL_ALIGN_TOP
1.  object <span class="apidocSignatureSpan">jimp.</span>phash.prototype
1.  object <span class="apidocSignatureSpan">jimp.</span>resize.prototype
1.  object <span class="apidocSignatureSpan">jimp.</span>resize2
1.  string <span class="apidocSignatureSpan">jimp.</span>FONT_SANS_128_BLACK
1.  string <span class="apidocSignatureSpan">jimp.</span>FONT_SANS_128_WHITE
1.  string <span class="apidocSignatureSpan">jimp.</span>FONT_SANS_16_BLACK
1.  string <span class="apidocSignatureSpan">jimp.</span>FONT_SANS_16_WHITE
1.  string <span class="apidocSignatureSpan">jimp.</span>FONT_SANS_32_BLACK
1.  string <span class="apidocSignatureSpan">jimp.</span>FONT_SANS_32_WHITE
1.  string <span class="apidocSignatureSpan">jimp.</span>FONT_SANS_64_BLACK
1.  string <span class="apidocSignatureSpan">jimp.</span>FONT_SANS_64_WHITE
1.  string <span class="apidocSignatureSpan">jimp.</span>FONT_SANS_8_BLACK
1.  string <span class="apidocSignatureSpan">jimp.</span>FONT_SANS_8_WHITE
1.  string <span class="apidocSignatureSpan">jimp.</span>MIME_BMP
1.  string <span class="apidocSignatureSpan">jimp.</span>MIME_JPEG
1.  string <span class="apidocSignatureSpan">jimp.</span>MIME_PNG
1.  string <span class="apidocSignatureSpan">jimp.</span>RESIZE_BEZIER
1.  string <span class="apidocSignatureSpan">jimp.</span>RESIZE_BICUBIC
1.  string <span class="apidocSignatureSpan">jimp.</span>RESIZE_BILINEAR
1.  string <span class="apidocSignatureSpan">jimp.</span>RESIZE_HERMITE
1.  string <span class="apidocSignatureSpan">jimp.</span>RESIZE_NEAREST_NEIGHBOR

#### [module jimp.phash](#apidoc.module.jimp.phash)
1.  [function <span class="apidocSignatureSpan">jimp.</span>phash (size, smallerSize)](#apidoc.element.jimp.phash.phash)

#### [module jimp.phash.prototype](#apidoc.module.jimp.phash.prototype)
1.  [function <span class="apidocSignatureSpan">jimp.phash.prototype.</span>distance (s1, s2)](#apidoc.element.jimp.phash.prototype.distance)
1.  [function <span class="apidocSignatureSpan">jimp.phash.prototype.</span>getHash (img)](#apidoc.element.jimp.phash.prototype.getHash)
1.  number <span class="apidocSignatureSpan">jimp.phash.prototype.</span>size
1.  number <span class="apidocSignatureSpan">jimp.phash.prototype.</span>smallerSize

#### [module jimp.resize](#apidoc.module.jimp.resize)
1.  [function <span class="apidocSignatureSpan">jimp.</span>resize (widthOriginal, heightOriginal, targetWidth, targetHeight, blendAlpha, interpolationPass, resizeCallback)](#apidoc.element.jimp.resize.resize)

#### [module jimp.resize.prototype](#apidoc.module.jimp.resize.prototype)
1.  [function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>bypassResizer (buffer)](#apidoc.element.jimp.resize.prototype.bypassResizer)
1.  [function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>configurePasses ()](#apidoc.element.jimp.resize.prototype.configurePasses)
1.  [function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>generateFloatBuffer (bufferLength)](#apidoc.element.jimp.resize.prototype.generateFloatBuffer)
1.  [function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>generateUint8Buffer (bufferLength)](#apidoc.element.jimp.resize.prototype.generateUint8Buffer)
1.  [function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>initialize ()](#apidoc.element.jimp.resize.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>initializeFirstPassBuffers (BILINEARAlgo)](#apidoc.element.jimp.resize.prototype.initializeFirstPassBuffers)
1.  [function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>initializeSecondPassBuffers (BILINEARAlgo)](#apidoc.element.jimp.resize.prototype.initializeSecondPassBuffers)
1.  [function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>resize (buffer)](#apidoc.element.jimp.resize.prototype.resize)
1.  [function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>resizeHeightInterpolated (buffer)](#apidoc.element.jimp.resize.prototype.resizeHeightInterpolated)
1.  [function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>resizeHeightRGB (buffer)](#apidoc.element.jimp.resize.prototype.resizeHeightRGB)
1.  [function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>resizeHeightRGBA (buffer)](#apidoc.element.jimp.resize.prototype.resizeHeightRGBA)
1.  [function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>resizeWidthInterpolatedRGB (buffer)](#apidoc.element.jimp.resize.prototype.resizeWidthInterpolatedRGB)
1.  [function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>resizeWidthInterpolatedRGBA (buffer)](#apidoc.element.jimp.resize.prototype.resizeWidthInterpolatedRGBA)
1.  [function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>resizeWidthRGB (buffer)](#apidoc.element.jimp.resize.prototype.resizeWidthRGB)
1.  [function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>resizeWidthRGBA (buffer)](#apidoc.element.jimp.resize.prototype.resizeWidthRGBA)

#### [module jimp.resize2](#apidoc.module.jimp.resize2)
1.  [function <span class="apidocSignatureSpan">jimp.resize2.</span>_interpolate2D (src, dst, options, interpolate)](#apidoc.element.jimp.resize2._interpolate2D)
1.  [function <span class="apidocSignatureSpan">jimp.resize2.</span>bezierInterpolation (src, dst, options)](#apidoc.element.jimp.resize2.bezierInterpolation)
1.  [function <span class="apidocSignatureSpan">jimp.resize2.</span>bicubicInterpolation (src, dst, options)](#apidoc.element.jimp.resize2.bicubicInterpolation)
1.  [function <span class="apidocSignatureSpan">jimp.resize2.</span>bilinearInterpolation (src, dst, options)](#apidoc.element.jimp.resize2.bilinearInterpolation)
1.  [function <span class="apidocSignatureSpan">jimp.resize2.</span>hermiteInterpolation (src, dst, options)](#apidoc.element.jimp.resize2.hermiteInterpolation)
1.  [function <span class="apidocSignatureSpan">jimp.resize2.</span>nearestNeighbor (src, dst, options)](#apidoc.element.jimp.resize2.nearestNeighbor)



# <a name="apidoc.module.jimp"></a>[module jimp](#apidoc.module.jimp)

#### <a name="apidoc.element.jimp.diff"></a>[function <span class="apidocSignatureSpan">jimp.</span>diff (img1, img2, threshold)](#apidoc.element.jimp.diff)
- description and source-code
```javascript
diff = function (img1, img2, threshold) {
    if ("object" != typeof img1 || img1.constructor != Jimp || "object" != typeof img2 || img2.constructor != Jimp)
        return throwError.call(this, "img1 and img2 must be an Jimp images");

    if (img1.bitmap.width != img2.bitmap.width || img1.bitmap.height != img2.bitmap.height) {
        switch (img1.bitmap.width * img1.bitmap.height > img2.bitmap.width * img2.bitmap.height) {
            case true: // img1 is bigger
                img1 = img1.clone().resize(img2.bitmap.width, img2.bitmap.height);
                break;
            default:
                // img2 is bigger (or they are the same in area)
                img2 = img2.clone().resize(img1.bitmap.width, img1.bitmap.height);
                break;
        }
    }

    threshold = threshold || 0.1;
    if ("number" != typeof threshold || threshold < 0 || threshold > 1)
        return throwError.call(this, "threshold must be a number between 0 and 1");

    var diff = new Jimp(img1.bitmap.width, img1.bitmap.height, 0xFFFFFFFF);

    var numDiffPixels = PixelMatch(
        img1.bitmap.data,
        img2.bitmap.data,
        diff.bitmap.data,
        diff.bitmap.width,
        diff.bitmap.height,
        {threshold: threshold}
    );

    return {
        percent: numDiffPixels / (diff.bitmap.width * diff.bitmap.height),
        image: diff
    };
}
```
- example usage
```shell
...
'''js
Jimp.distance(image1, image2); // returns a number 0-1, where 0 means the two images are perceived to be identical
'''

Jimp also allows the diffing of two Jimp images using [PixelMatch](https://github.com/mapbox/pixelmatch) as follows:

'''js
var diff = Jimp.diff(image1, image2, threshold); // threshold ranges 0-1 (default: 0.1)
diff.image;   // a Jimp image showing differences
diff.percent; // the proportion of different pixels (0-1), where 0 means the images are pixel identical
'''

Using a mix of hamming distance and pixel diffing to comare images, the following code has a 99% success rate of detecting the same
 image from a random sample (with 1% false positives). The test this figure is drawn from attempts to match each image from a sample
 of 120 PNGs against 120 corresponing JPEGs saved at a quality setting of 60.

'''js
...
```

#### <a name="apidoc.element.jimp.distance"></a>[function <span class="apidocSignatureSpan">jimp.</span>distance (img1, img2)](#apidoc.element.jimp.distance)
- description and source-code
```javascript
distance = function (img1, img2) {
    var phash = new ImagePHash();
    var hash1 = phash.getHash(img1);
    var hash2 = phash.getHash(img2);
    return phash.distance(hash1, hash2);
}
```
- example usage
```shell
...
'''

There are 18,446,744,073,709,551,615 unique hashes. The hamming distance between the binary representation of these hashes can be
 used to find similar-looking images.

To calculate the hamming distance between two Jimp images based on their perceptual hash use:

'''js
Jimp.distance(image1, image2); // returns a number 0-1, where 0 means the two images are perceived to be identical
'''

Jimp also allows the diffing of two Jimp images using [PixelMatch](https://github.com/mapbox/pixelmatch) as follows:

'''js
var diff = Jimp.diff(image1, image2, threshold); // threshold ranges 0-1 (default: 0.1)
diff.image;   // a Jimp image showing differences
...
```

#### <a name="apidoc.element.jimp.intToRGBA"></a>[function <span class="apidocSignatureSpan">jimp.</span>intToRGBA (i, cb)](#apidoc.element.jimp.intToRGBA)
- description and source-code
```javascript
intToRGBA = function (i, cb){
    if ("number" != typeof i)
        return throwError.call(this, "i must be a number", cb);

    var rgba = {}
    rgba.r = Math.floor(i / Math.pow(256, 3));
    rgba.g = Math.floor((i - (rgba.r * Math.pow(256, 3))) / Math.pow(256, 2));
    rgba.b = Math.floor((i - (rgba.r * Math.pow(256, 3)) - (rgba.g * Math.pow(256, 2))) / Math.pow(256, 1));
    rgba.a = Math.floor((i - (rgba.r * Math.pow(256, 3)) - (rgba.g * Math.pow(256, 2)) - (rgba.b * Math.pow(256, 1))) / Math.pow
(256, 0));

    if (isNodePattern(cb)) return cb.call(this, null, rgba);
    else return rgba;
}
```
- example usage
```shell
...
image.setPixelColor(hex, x, y); // sets the colour of that pixel
'''

Two static helper functions exist to convert RGBA values into single integer (hex) values:

'''js
Jimp.rgbaToInt(r, g, b, a); // e.g. converts 255, 255, 255, 255 to 0xFFFFFFFF
Jimp.intToRGBA(hex);        // e.g. converts 0xFFFFFFFF to {r: 255, g: 255, b: 255, a:255}
'''

### Creating new images ###

If you want to begin with an empty Jimp image, you can call the Jimp constructor passing the width and height of the image to create
 and (optionally) a Node-style callback:

'''js
...
```

#### <a name="apidoc.element.jimp.limit255"></a>[function <span class="apidocSignatureSpan">jimp.</span>limit255 (n)](#apidoc.element.jimp.limit255)
- description and source-code
```javascript
limit255 = function (n) {
    n = Math.max(n, 0);
    n = Math.min(n, 255);
    return n;
}
```
- example usage
```shell
...

    var a = bg.a + fg.a - bg.a * fg.a;

    var r = ((fg.r * fg.a) + (bg.r * bg.a) * (1 - fg.a)) / a;
    var g = ((fg.g * fg.a) + (bg.g * bg.a) * (1 - fg.a)) / a;
    var b = ((fg.b * fg.a) + (bg.b * bg.a) * (1 - fg.a)) / a;

    that.bitmap.data[dstIdx + 0] = Jimp.limit255(r * 255);
    that.bitmap.data[dstIdx + 1] = Jimp.limit255(g * 255);
    that.bitmap.data[dstIdx + 2] = Jimp.limit255(b * 255);
    that.bitmap.data[dstIdx + 3] = Jimp.limit255(a * 255);
});

if (isNodePattern(cb)) return cb.call(this, null, this);
else return this;
...
```

#### <a name="apidoc.element.jimp.loadFont"></a>[function <span class="apidocSignatureSpan">jimp.</span>loadFont (file, cb)](#apidoc.element.jimp.loadFont)
- description and source-code
```javascript
loadFont = function (file, cb) {
    if ("string" != typeof file)
        return throwError.call(this, "file must be a string", cb);

    var that = this;

    return new Promise(function (resolve, reject) {
        cb = cb || function(err, font) {
            if (err) reject(err);
            else resolve(font);
        }

        BMFont(file, function(err, font) {
            var chars = {}, kernings = {};

            if (err) return throwError.call(that, err, cb);

            for (var i = 0; i < font.chars.length; i++) {
                chars[String.fromCharCode(font.chars[i].id)] = font.chars[i];
            }

            for (var i = 0; i < font.kernings.length; i++) {
                var firstString = String.fromCharCode(font.kernings[i].first);
                kernings[firstString] = kernings[firstString] || {};
                kernings[firstString][String.fromCharCode(font.kernings[i].second)] = font.kernings[i].amount;
            }

            loadPages(Path.dirname(file), font.pages).then(function (pages) {
                cb(null, {
                    chars: chars,
                    kernings: kernings,
                    pages: pages,
                    common: font.common,
                    info: font.info
                });
            });
        });
    });
}
```
- example usage
```shell
...
'''

### Writing text ###

Jimp supports basic typography using BMFont format (.fnt) [bitmap fonts](https://en.wikipedia.org/wiki/Bitmap_fonts):

'''js
Jimp.loadFont( path ).then(function (font) { // load font from .fnt file
    image.print(font, x, y, str);        // print a message on an image
    image.print(font, x, y, str, width); // print a message on an image with text wrapped at width
});

Jimp.loadFont( path, cb ); // using a callback pattern
'''
...
```

#### <a name="apidoc.element.jimp.phash"></a>[function <span class="apidocSignatureSpan">jimp.</span>phash (size, smallerSize)](#apidoc.element.jimp.phash)
- description and source-code
```javascript
function ImagePHash(size, smallerSize) {
    this.size = this.size || size;
    this.smallerSize = this.smallerSize || smallerSize;
    initCoefficients(this.size);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jimp.read"></a>[function <span class="apidocSignatureSpan">jimp.</span>read (src, cb)](#apidoc.element.jimp.read)
- description and source-code
```javascript
read = function (src, cb) {
    var promise = new Promise(
        function(resolve, reject) {
            cb = cb || function(err, image) {
                if (err) reject(err);
                else resolve(image);
            }
            if ("string" != typeof src && ("object" != typeof src || !Buffer.isBuffer(src)))
                return throwError.call(this, "src must be a string or a Buffer", cb);
            var img = new Jimp(src, cb);
        }
    );
    return promise;
}
```
- example usage
```shell
...

Example usage:

'''js
var Jimp = require("jimp");

// open a file called "lenna.png"
Jimp.read("lenna.png", function (err, lenna) {
    if (err) throw err;
    lenna.resize(256, 256)            // resize
         .quality(60)                 // set JPEG quality
         .greyscale()                 // set greyscale
         .write("lena-small-bw.jpg"); // save
});
'''
...
```

#### <a name="apidoc.element.jimp.resize"></a>[function <span class="apidocSignatureSpan">jimp.</span>resize (widthOriginal, heightOriginal, targetWidth, targetHeight, blendAlpha, interpolationPass, resizeCallback)](#apidoc.element.jimp.resize)
- description and source-code
```javascript
function Resize(widthOriginal, heightOriginal, targetWidth, targetHeight, blendAlpha, interpolationPass, resizeCallback) {
    this.widthOriginal = Math.abs(parseInt(widthOriginal) || 0);
    this.heightOriginal = Math.abs(parseInt(heightOriginal) || 0);
    this.targetWidth = Math.abs(parseInt(targetWidth) || 0);
    this.targetHeight = Math.abs(parseInt(targetHeight) || 0);
    this.colorChannels = (!!blendAlpha) ? 4 : 3;
    this.interpolationPass = !!interpolationPass;
    this.resizeCallback = (typeof resizeCallback == "function") ? resizeCallback : function (returnedArray) {};
    this.targetWidthMultipliedByChannels = this.targetWidth * this.colorChannels;
    this.originalWidthMultipliedByChannels = this.widthOriginal * this.colorChannels;
    this.originalHeightMultipliedByChannels = this.heightOriginal * this.colorChannels;
    this.widthPassResultSize = this.targetWidthMultipliedByChannels * this.heightOriginal;
    this.finalResultSize = this.targetWidthMultipliedByChannels * this.targetHeight;
    this.initialize();
}
```
- example usage
```shell
...

'''js
var Jimp = require("jimp");

// open a file called "lenna.png"
Jimp.read("lenna.png", function (err, lenna) {
    if (err) throw err;
    lenna.resize(256, 256)            // resize
         .quality(60)                 // set JPEG quality
         .greyscale()                 // set greyscale
         .write("lena-small-bw.jpg"); // save
});
'''

Using promises:
...
```

#### <a name="apidoc.element.jimp.rgbaToInt"></a>[function <span class="apidocSignatureSpan">jimp.</span>rgbaToInt (r, g, b, a, cb)](#apidoc.element.jimp.rgbaToInt)
- description and source-code
```javascript
rgbaToInt = function (r, g, b, a, cb){
    if ("number" != typeof r || "number" != typeof g || "number" != typeof b || "number" != typeof a)
        return throwError.call(this, "r, g, b and a must be numbers", cb);
    if (r < 0 || r > 255)
        return throwError.call(this, "r must be between 0 and 255", cb);
    if (g < 0 || g > 255)
        throwError.call(this, "g must be between 0 and 255", cb);
    if (b < 0 || b > 255)
        return throwError.call(this, "b must be between 0 and 255", cb);
    if (a < 0 || a > 255)
        return throwError.call(this, "a must be between 0 and 255", cb);

    var i = (r * Math.pow(256, 3)) + (g * Math.pow(256, 2)) + (b *  Math.pow(256, 1)) + (a * Math.pow(256, 0));

    if (isNodePattern(cb)) return cb.call(this, null, i);
    else return i;
}
```
- example usage
```shell
...
image.getPixelColor(x, y);      // returns the colour of that pixel e.g. 0xFFFFFFFF
image.setPixelColor(hex, x, y); // sets the colour of that pixel
'''

Two static helper functions exist to convert RGBA values into single integer (hex) values:

'''js
Jimp.rgbaToInt(r, g, b, a); // e.g. converts 255, 255, 255, 255 to 0xFFFFFFFF
Jimp.intToRGBA(hex);        // e.g. converts 0xFFFFFFFF to {r: 255, g: 255, b: 255, a:255}
'''

### Creating new images ###

If you want to begin with an empty Jimp image, you can call the Jimp constructor passing the width and height of the image to create
 and (optionally) a Node-style callback:
...
```



# <a name="apidoc.module.jimp.phash"></a>[module jimp.phash](#apidoc.module.jimp.phash)

#### <a name="apidoc.element.jimp.phash.phash"></a>[function <span class="apidocSignatureSpan">jimp.</span>phash (size, smallerSize)](#apidoc.element.jimp.phash.phash)
- description and source-code
```javascript
function ImagePHash(size, smallerSize) {
    this.size = this.size || size;
    this.smallerSize = this.smallerSize || smallerSize;
    initCoefficients(this.size);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jimp.phash.prototype"></a>[module jimp.phash.prototype](#apidoc.module.jimp.phash.prototype)

#### <a name="apidoc.element.jimp.phash.prototype.distance"></a>[function <span class="apidocSignatureSpan">jimp.phash.prototype.</span>distance (s1, s2)](#apidoc.element.jimp.phash.prototype.distance)
- description and source-code
```javascript
distance = function (s1, s2) {
    var counter = 0;
    for (var k = 0; k < s1.length; k++) {
        if (s1[k] != s2[k]) {
            counter++;
        }
    }
    return (counter / s1.length);
}
```
- example usage
```shell
...
'''

There are 18,446,744,073,709,551,615 unique hashes. The hamming distance between the binary representation of these hashes can be
 used to find similar-looking images.

To calculate the hamming distance between two Jimp images based on their perceptual hash use:

'''js
Jimp.distance(image1, image2); // returns a number 0-1, where 0 means the two images are perceived to be identical
'''

Jimp also allows the diffing of two Jimp images using [PixelMatch](https://github.com/mapbox/pixelmatch) as follows:

'''js
var diff = Jimp.diff(image1, image2, threshold); // threshold ranges 0-1 (default: 0.1)
diff.image;   // a Jimp image showing differences
...
```

#### <a name="apidoc.element.jimp.phash.prototype.getHash"></a>[function <span class="apidocSignatureSpan">jimp.phash.prototype.</span>getHash (img)](#apidoc.element.jimp.phash.prototype.getHash)
- description and source-code
```javascript
getHash = function (img) {
<span class="apidocCodeCommentSpan">    /* 1. Reduce size.
     * Like Average Hash, pHash starts with a small image.
     * However, the image is larger than 8x8; 32x32 is a good size.
     * This is really done to simplify the DCT computation and not
     * because it is needed to reduce the high frequencies.
     */
</span>    img = img.clone().resize(this.size, this.size);

    /* 2. Reduce color.
     * The image is reduced to a grayscale just to further simplify
     * the number of computations.
     */
    img.grayscale();

    var vals = [];

    for (var x = 0; x < img.bitmap.width; x++) {
        vals[x] = [];
        for (var y = 0; y < img.bitmap.height; y++) {
            vals[x][y] = intToRGBA(img.getPixelColor(x, y)).b;
        }
    }

    /* 3. Compute the DCT.
     * The DCT separates the image into a collection of frequencies
     * and scalars. While JPEG uses an 8x8 DCT, this algorithm uses
     * a 32x32 DCT.
     */
    var dctVals = applyDCT(vals, this.size);

    /* 4. Reduce the DCT.
     * This is the magic step. While the DCT is 32x32, just keep the
     * top-left 8x8. Those represent the lowest frequencies in the
     * picture.
     */
    /* 5. Compute the average value.
     * Like the Average Hash, compute the mean DCT value (using only
     * the 8x8 DCT low-frequency values and excluding the first term
     * since the DC coefficient can be significantly different from
     * the other values and will throw off the average).
     */
    var total = 0;

    for (var x = 0; x < this.smallerSize; x++) {
        for (var y = 0; y < this.smallerSize; y++) {
            total += dctVals[x][y];
        }
    }

    var avg = total / (this.smallerSize * this.smallerSize);

    /* 6. Further reduce the DCT.
     * This is the magic step. Set the 64 hash bits to 0 or 1
     * depending on whether each of the 64 DCT values is above or
     * below the average value. The result doesn't tell us the
     * actual low frequencies; it just tells us the very-rough
     * relative scale of the frequencies to the mean. The result
     * will not vary as long as the overall structure of the image
     * remains the same; this can survive gamma and color histogram
     * adjustments without a problem.
     */
    var hash = "";

	var count = 0;
    for (var x = 0; x < this.smallerSize; x++) {
        for (var y = 0; y < this.smallerSize; y++) {
            hash += (dctVals[x][y] > avg?"1":"0");
        }
    }

    return hash;
}
```
- example usage
```shell
...
 * Calculates the hamming distance of two images based on their perceptual hash
 * @param img1 a Jimp image to compare
 * @param img2 a Jimp image to compare
 * @returns a number ranging from 0 to 1, 0 means they are believed to be identical
 */
Jimp.distance = function (img1, img2) {
    var phash = new ImagePHash();
    var hash1 = phash.getHash(img1);
    var hash2 = phash.getHash(img2);
    return phash.distance(hash1, hash2);
}


// An object representing a bitmap in memory, comprising:
//  - data: a buffer of the bitmap data
...
```



# <a name="apidoc.module.jimp.resize"></a>[module jimp.resize](#apidoc.module.jimp.resize)

#### <a name="apidoc.element.jimp.resize.resize"></a>[function <span class="apidocSignatureSpan">jimp.</span>resize (widthOriginal, heightOriginal, targetWidth, targetHeight, blendAlpha, interpolationPass, resizeCallback)](#apidoc.element.jimp.resize.resize)
- description and source-code
```javascript
function Resize(widthOriginal, heightOriginal, targetWidth, targetHeight, blendAlpha, interpolationPass, resizeCallback) {
    this.widthOriginal = Math.abs(parseInt(widthOriginal) || 0);
    this.heightOriginal = Math.abs(parseInt(heightOriginal) || 0);
    this.targetWidth = Math.abs(parseInt(targetWidth) || 0);
    this.targetHeight = Math.abs(parseInt(targetHeight) || 0);
    this.colorChannels = (!!blendAlpha) ? 4 : 3;
    this.interpolationPass = !!interpolationPass;
    this.resizeCallback = (typeof resizeCallback == "function") ? resizeCallback : function (returnedArray) {};
    this.targetWidthMultipliedByChannels = this.targetWidth * this.colorChannels;
    this.originalWidthMultipliedByChannels = this.widthOriginal * this.colorChannels;
    this.originalHeightMultipliedByChannels = this.heightOriginal * this.colorChannels;
    this.widthPassResultSize = this.targetWidthMultipliedByChannels * this.heightOriginal;
    this.finalResultSize = this.targetWidthMultipliedByChannels * this.targetHeight;
    this.initialize();
}
```
- example usage
```shell
...

'''js
var Jimp = require("jimp");

// open a file called "lenna.png"
Jimp.read("lenna.png", function (err, lenna) {
    if (err) throw err;
    lenna.resize(256, 256)            // resize
         .quality(60)                 // set JPEG quality
         .greyscale()                 // set greyscale
         .write("lena-small-bw.jpg"); // save
});
'''

Using promises:
...
```



# <a name="apidoc.module.jimp.resize.prototype"></a>[module jimp.resize.prototype](#apidoc.module.jimp.resize.prototype)

#### <a name="apidoc.element.jimp.resize.prototype.bypassResizer"></a>[function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>bypassResizer (buffer)](#apidoc.element.jimp.resize.prototype.bypassResizer)
- description and source-code
```javascript
bypassResizer = function (buffer) {
    //Just return the buffer passsed:
    return buffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jimp.resize.prototype.configurePasses"></a>[function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>configurePasses ()](#apidoc.element.jimp.resize.prototype.configurePasses)
- description and source-code
```javascript
configurePasses = function () {
    if (this.widthOriginal == this.targetWidth) {
        //Bypass the width resizer pass:
        this.resizeWidth = this.bypassResizer;
    } else {
        //Setup the width resizer pass:
        this.ratioWeightWidthPass = this.widthOriginal / this.targetWidth;
        if (this.ratioWeightWidthPass < 1 && this.interpolationPass) {
            this.initializeFirstPassBuffers(true);
            this.resizeWidth = (this.colorChannels == 4) ? this.resizeWidthInterpolatedRGBA : this.resizeWidthInterpolatedRGB;
        } else {
            this.initializeFirstPassBuffers(false);
            this.resizeWidth = (this.colorChannels == 4) ? this.resizeWidthRGBA : this.resizeWidthRGB;
        }
    }
    if (this.heightOriginal == this.targetHeight) {
        //Bypass the height resizer pass:
        this.resizeHeight = this.bypassResizer;
    } else {
        //Setup the height resizer pass:
        this.ratioWeightHeightPass = this.heightOriginal / this.targetHeight;
        if (this.ratioWeightHeightPass < 1 && this.interpolationPass) {
            this.initializeSecondPassBuffers(true);
            this.resizeHeight = this.resizeHeightInterpolated;
        } else {
            this.initializeSecondPassBuffers(false);
            this.resizeHeight = (this.colorChannels == 4) ? this.resizeHeightRGBA : this.resizeHeightRGB;
        }
    }
}
```
- example usage
```shell
...
this.finalResultSize = this.targetWidthMultipliedByChannels * this.targetHeight;
this.initialize();
}

Resize.prototype.initialize = function () {
//Perform some checks:
if (this.widthOriginal > 0 && this.heightOriginal > 0 && this.targetWidth > 0 && this.targetHeight > 0) {
    this.configurePasses();
} else {
    throw (new Error("Invalid settings specified for the resizer."));
}
}

Resize.prototype.configurePasses = function () {
if (this.widthOriginal == this.targetWidth) {
...
```

#### <a name="apidoc.element.jimp.resize.prototype.generateFloatBuffer"></a>[function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>generateFloatBuffer (bufferLength)](#apidoc.element.jimp.resize.prototype.generateFloatBuffer)
- description and source-code
```javascript
generateFloatBuffer = function (bufferLength) {
    //Generate a float32 typed array buffer:
    try {
        return new Float32Array(bufferLength);
    } catch (error) {
        return [];
    }
}
```
- example usage
```shell
...
Resize.prototype.bypassResizer = function (buffer) {
//Just return the buffer passsed:
return buffer;
}

Resize.prototype.initializeFirstPassBuffers = function (BILINEARAlgo) {
//Initialize the internal width pass buffers:
this.widthBuffer = this.generateFloatBuffer(this.widthPassResultSize);
if (!BILINEARAlgo) {
    this.outputWidthWorkBench = this.generateFloatBuffer(this.originalHeightMultipliedByChannels);
}
}

Resize.prototype.initializeSecondPassBuffers = function (BILINEARAlgo) {
//Initialize the internal height pass buffers:
...
```

#### <a name="apidoc.element.jimp.resize.prototype.generateUint8Buffer"></a>[function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>generateUint8Buffer (bufferLength)](#apidoc.element.jimp.resize.prototype.generateUint8Buffer)
- description and source-code
```javascript
generateUint8Buffer = function (bufferLength) {
    //Generate a uint8 typed array buffer:
    try {
        return new Uint8Array(bufferLength);
    } catch (error) {
        return [];
    }
}
```
- example usage
```shell
...
if (!BILINEARAlgo) {
    this.outputWidthWorkBench = this.generateFloatBuffer(this.originalHeightMultipliedByChannels);
}
}

Resize.prototype.initializeSecondPassBuffers = function (BILINEARAlgo) {
//Initialize the internal height pass buffers:
this.heightBuffer = this.generateUint8Buffer(this.finalResultSize);
if (!BILINEARAlgo) {
    this.outputHeightWorkBench = this.generateFloatBuffer(this.targetWidthMultipliedByChannels);
}
}

Resize.prototype.generateFloatBuffer = function (bufferLength) {
//Generate a float32 typed array buffer:
...
```

#### <a name="apidoc.element.jimp.resize.prototype.initialize"></a>[function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>initialize ()](#apidoc.element.jimp.resize.prototype.initialize)
- description and source-code
```javascript
initialize = function () {
    //Perform some checks:
    if (this.widthOriginal > 0 && this.heightOriginal > 0 && this.targetWidth > 0 && this.targetHeight > 0) {
        this.configurePasses();
    } else {
        throw (new Error("Invalid settings specified for the resizer."));
    }
}
```
- example usage
```shell
...
this.interpolationPass = !!interpolationPass;
this.resizeCallback = (typeof resizeCallback == "function") ? resizeCallback : function (returnedArray) {};
this.targetWidthMultipliedByChannels = this.targetWidth * this.colorChannels;
this.originalWidthMultipliedByChannels = this.widthOriginal * this.colorChannels;
this.originalHeightMultipliedByChannels = this.heightOriginal * this.colorChannels;
this.widthPassResultSize = this.targetWidthMultipliedByChannels * this.heightOriginal;
this.finalResultSize = this.targetWidthMultipliedByChannels * this.targetHeight;
this.initialize();
}

Resize.prototype.initialize = function () {
//Perform some checks:
if (this.widthOriginal > 0 && this.heightOriginal > 0 && this.targetWidth > 0 && this.targetHeight > 0) {
    this.configurePasses();
} else {
...
```

#### <a name="apidoc.element.jimp.resize.prototype.initializeFirstPassBuffers"></a>[function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>initializeFirstPassBuffers (BILINEARAlgo)](#apidoc.element.jimp.resize.prototype.initializeFirstPassBuffers)
- description and source-code
```javascript
initializeFirstPassBuffers = function (BILINEARAlgo) {
    //Initialize the internal width pass buffers:
    this.widthBuffer = this.generateFloatBuffer(this.widthPassResultSize);
    if (!BILINEARAlgo) {
        this.outputWidthWorkBench = this.generateFloatBuffer(this.originalHeightMultipliedByChannels);
    }
}
```
- example usage
```shell
...
if (this.widthOriginal == this.targetWidth) {
    //Bypass the width resizer pass:
    this.resizeWidth = this.bypassResizer;
} else {
    //Setup the width resizer pass:
    this.ratioWeightWidthPass = this.widthOriginal / this.targetWidth;
    if (this.ratioWeightWidthPass < 1 && this.interpolationPass) {
        this.initializeFirstPassBuffers(true);
        this.resizeWidth = (this.colorChannels == 4) ? this.resizeWidthInterpolatedRGBA : this.resizeWidthInterpolatedRGB;
    } else {
        this.initializeFirstPassBuffers(false);
        this.resizeWidth = (this.colorChannels == 4) ? this.resizeWidthRGBA : this.resizeWidthRGB;
    }
}
if (this.heightOriginal == this.targetHeight) {
...
```

#### <a name="apidoc.element.jimp.resize.prototype.initializeSecondPassBuffers"></a>[function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>initializeSecondPassBuffers (BILINEARAlgo)](#apidoc.element.jimp.resize.prototype.initializeSecondPassBuffers)
- description and source-code
```javascript
initializeSecondPassBuffers = function (BILINEARAlgo) {
    //Initialize the internal height pass buffers:
    this.heightBuffer = this.generateUint8Buffer(this.finalResultSize);
    if (!BILINEARAlgo) {
        this.outputHeightWorkBench = this.generateFloatBuffer(this.targetWidthMultipliedByChannels);
    }
}
```
- example usage
```shell
...
    if (this.heightOriginal == this.targetHeight) {
        //Bypass the height resizer pass:
        this.resizeHeight = this.bypassResizer;
    } else {
        //Setup the height resizer pass:
        this.ratioWeightHeightPass = this.heightOriginal / this.targetHeight;
        if (this.ratioWeightHeightPass < 1 && this.interpolationPass) {
            this.initializeSecondPassBuffers(true);
            this.resizeHeight = this.resizeHeightInterpolated;
        } else {
            this.initializeSecondPassBuffers(false);
            this.resizeHeight = (this.colorChannels == 4) ? this.resizeHeightRGBA : this.resizeHeightRGB;
        }
    }
}
...
```

#### <a name="apidoc.element.jimp.resize.prototype.resize"></a>[function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>resize (buffer)](#apidoc.element.jimp.resize.prototype.resize)
- description and source-code
```javascript
resize = function (buffer) {
    this.resizeCallback(this.resizeHeight(this.resizeWidth(buffer)));
}
```
- example usage
```shell
...

'''js
var Jimp = require("jimp");

// open a file called "lenna.png"
Jimp.read("lenna.png", function (err, lenna) {
    if (err) throw err;
    lenna.resize(256, 256)            // resize
         .quality(60)                 // set JPEG quality
         .greyscale()                 // set greyscale
         .write("lena-small-bw.jpg"); // save
});
'''

Using promises:
...
```

#### <a name="apidoc.element.jimp.resize.prototype.resizeHeightInterpolated"></a>[function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>resizeHeightInterpolated (buffer)](#apidoc.element.jimp.resize.prototype.resizeHeightInterpolated)
- description and source-code
```javascript
resizeHeightInterpolated = function (buffer) {
    var ratioWeight = this.ratioWeightHeightPass;
    var weight = 0;
    var finalOffset = 0;
    var pixelOffset = 0;
    var pixelOffsetAccumulated = 0;
    var pixelOffsetAccumulated2 = 0;
    var firstWeight = 0;
    var secondWeight = 0;
    var outputBuffer = this.heightBuffer;
    //Handle for only one interpolation input being valid for start calculation:
    for (; weight < 1 / 3; weight += ratioWeight) {
        for (pixelOffset = 0; pixelOffset < this.targetWidthMultipliedByChannels;) {
            outputBuffer[finalOffset++] = Math.round(buffer[pixelOffset++]);
        }
    }
    //Adjust for overshoot of the last pass's counter:
    weight -= 1 / 3;
    for (var interpolationHeightSourceReadStop = this.heightOriginal - 1; weight < interpolationHeightSourceReadStop; weight +=
ratioWeight) {
        //Calculate weightings:
        secondWeight = weight % 1;
        firstWeight = 1 - secondWeight;
        //Interpolate:
        pixelOffsetAccumulated = Math.floor(weight) * this.targetWidthMultipliedByChannels;
        pixelOffsetAccumulated2 = pixelOffsetAccumulated + this.targetWidthMultipliedByChannels;
        for (pixelOffset = 0; pixelOffset < this.targetWidthMultipliedByChannels; ++pixelOffset) {
            outputBuffer[finalOffset++] = Math.round((buffer[pixelOffsetAccumulated++] * firstWeight) + (buffer[pixelOffsetAccumulated2
++] * secondWeight));
        }
    }
    //Handle for only one interpolation input being valid for end calculation:
    while (finalOffset < this.finalResultSize) {
        for (pixelOffset = 0, pixelOffsetAccumulated = interpolationHeightSourceReadStop * this.targetWidthMultipliedByChannels;
pixelOffset < this.targetWidthMultipliedByChannels; ++pixelOffset) {
            outputBuffer[finalOffset++] = Math.round(buffer[pixelOffsetAccumulated++]);
        }
    }
    return outputBuffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jimp.resize.prototype.resizeHeightRGB"></a>[function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>resizeHeightRGB (buffer)](#apidoc.element.jimp.resize.prototype.resizeHeightRGB)
- description and source-code
```javascript
resizeHeightRGB = function (buffer) {
    var ratioWeight = this.ratioWeightHeightPass;
    var ratioWeightDivisor = 1 / ratioWeight;
    var weight = 0;
    var amountToNext = 0;
    var actualPosition = 0;
    var currentPosition = 0;
    var pixelOffset = 0;
    var outputOffset = 0;
    var output = this.outputHeightWorkBench;
    var outputBuffer = this.heightBuffer;
    do {
        for (pixelOffset = 0; pixelOffset < this.targetWidthMultipliedByChannels;) {
            output[pixelOffset++] = 0;
            output[pixelOffset++] = 0;
            output[pixelOffset++] = 0;
        }
        weight = ratioWeight;
        do {
            amountToNext = 1 + actualPosition - currentPosition;
            if (weight >= amountToNext) {
                for (pixelOffset = 0; pixelOffset < this.targetWidthMultipliedByChannels;) {
                    output[pixelOffset++] += buffer[actualPosition++] * amountToNext;
                    output[pixelOffset++] += buffer[actualPosition++] * amountToNext;
                    output[pixelOffset++] += buffer[actualPosition++] * amountToNext;
                }
                currentPosition = actualPosition;
                weight -= amountToNext;
            } else {
                for (pixelOffset = 0, amountToNext = actualPosition; pixelOffset < this.targetWidthMultipliedByChannels;) {
                    output[pixelOffset++] += buffer[amountToNext++] * weight;
                    output[pixelOffset++] += buffer[amountToNext++] * weight;
                    output[pixelOffset++] += buffer[amountToNext++] * weight;
                }
                currentPosition += weight;
                break;
            }
        } while (weight > 0 && actualPosition < this.widthPassResultSize);
        for (pixelOffset = 0; pixelOffset < this.targetWidthMultipliedByChannels;) {
            outputBuffer[outputOffset++] = Math.round(output[pixelOffset++] * ratioWeightDivisor);
            outputBuffer[outputOffset++] = Math.round(output[pixelOffset++] * ratioWeightDivisor);
            outputBuffer[outputOffset++] = Math.round(output[pixelOffset++] * ratioWeightDivisor);
        }
    } while (outputOffset < this.finalResultSize);
    return outputBuffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jimp.resize.prototype.resizeHeightRGBA"></a>[function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>resizeHeightRGBA (buffer)](#apidoc.element.jimp.resize.prototype.resizeHeightRGBA)
- description and source-code
```javascript
resizeHeightRGBA = function (buffer) {
    var ratioWeight = this.ratioWeightHeightPass;
    var ratioWeightDivisor = 1 / ratioWeight;
    var weight = 0;
    var amountToNext = 0;
    var actualPosition = 0;
    var currentPosition = 0;
    var pixelOffset = 0;
    var outputOffset = 0;
    var output = this.outputHeightWorkBench;
    var outputBuffer = this.heightBuffer;
    do {
        for (pixelOffset = 0; pixelOffset < this.targetWidthMultipliedByChannels;) {
            output[pixelOffset++] = 0;
            output[pixelOffset++] = 0;
            output[pixelOffset++] = 0;
            output[pixelOffset++] = 0;
        }
        weight = ratioWeight;
        do {
            amountToNext = 1 + actualPosition - currentPosition;
            if (weight >= amountToNext) {
                for (pixelOffset = 0; pixelOffset < this.targetWidthMultipliedByChannels;) {
                    output[pixelOffset++] += buffer[actualPosition++] * amountToNext;
                    output[pixelOffset++] += buffer[actualPosition++] * amountToNext;
                    output[pixelOffset++] += buffer[actualPosition++] * amountToNext;
                    output[pixelOffset++] += buffer[actualPosition++] * amountToNext;
                }
                currentPosition = actualPosition;
                weight -= amountToNext;
            } else {
                for (pixelOffset = 0, amountToNext = actualPosition; pixelOffset < this.targetWidthMultipliedByChannels;) {
                    output[pixelOffset++] += buffer[amountToNext++] * weight;
                    output[pixelOffset++] += buffer[amountToNext++] * weight;
                    output[pixelOffset++] += buffer[amountToNext++] * weight;
                    output[pixelOffset++] += buffer[amountToNext++] * weight;
                }
                currentPosition += weight;
                break;
            }
        } while (weight > 0 && actualPosition < this.widthPassResultSize);
        for (pixelOffset = 0; pixelOffset < this.targetWidthMultipliedByChannels;) {
            outputBuffer[outputOffset++] = Math.round(output[pixelOffset++] * ratioWeightDivisor);
            outputBuffer[outputOffset++] = Math.round(output[pixelOffset++] * ratioWeightDivisor);
            outputBuffer[outputOffset++] = Math.round(output[pixelOffset++] * ratioWeightDivisor);
            outputBuffer[outputOffset++] = Math.round(output[pixelOffset++] * ratioWeightDivisor);
        }
    } while (outputOffset < this.finalResultSize);
    return outputBuffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jimp.resize.prototype.resizeWidthInterpolatedRGB"></a>[function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>resizeWidthInterpolatedRGB (buffer)](#apidoc.element.jimp.resize.prototype.resizeWidthInterpolatedRGB)
- description and source-code
```javascript
resizeWidthInterpolatedRGB = function (buffer) {
    var ratioWeight = this.ratioWeightWidthPass;
    var weight = 0;
    var finalOffset = 0;
    var pixelOffset = 0;
    var firstWeight = 0;
    var secondWeight = 0;
    var outputBuffer = this.widthBuffer;
    //Handle for only one interpolation input being valid for start calculation:
    for (var targetPosition = 0; weight < 1 / 3; targetPosition += 3, weight += ratioWeight) {
        for (finalOffset = targetPosition, pixelOffset = 0; finalOffset < this.widthPassResultSize; pixelOffset += this.originalWidthMultipliedByChannels
, finalOffset += this.targetWidthMultipliedByChannels) {
            outputBuffer[finalOffset] = buffer[pixelOffset];
            outputBuffer[finalOffset + 1] = buffer[pixelOffset + 1];
            outputBuffer[finalOffset + 2] = buffer[pixelOffset + 2];
        }
    }
    //Adjust for overshoot of the last pass's counter:
    weight -= 1 / 3;
    for (var interpolationWidthSourceReadStop = this.widthOriginal - 1; weight < interpolationWidthSourceReadStop; targetPosition
 += 3, weight += ratioWeight) {
        //Calculate weightings:
        secondWeight = weight % 1;
        firstWeight = 1 - secondWeight;
        //Interpolate:
        for (finalOffset = targetPosition, pixelOffset = Math.floor(weight) * 3; finalOffset < this.widthPassResultSize; pixelOffset
 += this.originalWidthMultipliedByChannels, finalOffset += this.targetWidthMultipliedByChannels) {
            outputBuffer[finalOffset] = (buffer[pixelOffset] * firstWeight) + (buffer[pixelOffset + 3] * secondWeight);
            outputBuffer[finalOffset + 1] = (buffer[pixelOffset + 1] * firstWeight) + (buffer[pixelOffset + 4] * secondWeight);
            outputBuffer[finalOffset + 2] = (buffer[pixelOffset + 2] * firstWeight) + (buffer[pixelOffset + 5] * secondWeight);
        }
    }
    //Handle for only one interpolation input being valid for end calculation:
    for (interpolationWidthSourceReadStop = this.originalWidthMultipliedByChannels - 3; targetPosition < this.targetWidthMultipliedByChannels
; targetPosition += 3) {
        for (finalOffset = targetPosition, pixelOffset = interpolationWidthSourceReadStop; finalOffset < this.widthPassResultSize
; pixelOffset += this.originalWidthMultipliedByChannels, finalOffset += this.targetWidthMultipliedByChannels) {
            outputBuffer[finalOffset] = buffer[pixelOffset];
            outputBuffer[finalOffset + 1] = buffer[pixelOffset + 1];
            outputBuffer[finalOffset + 2] = buffer[pixelOffset + 2];
        }
    }
    return outputBuffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jimp.resize.prototype.resizeWidthInterpolatedRGBA"></a>[function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>resizeWidthInterpolatedRGBA (buffer)](#apidoc.element.jimp.resize.prototype.resizeWidthInterpolatedRGBA)
- description and source-code
```javascript
resizeWidthInterpolatedRGBA = function (buffer) {
    var ratioWeight = this.ratioWeightWidthPass;
    var weight = 0;
    var finalOffset = 0;
    var pixelOffset = 0;
    var firstWeight = 0;
    var secondWeight = 0;
    var outputBuffer = this.widthBuffer;
    //Handle for only one interpolation input being valid for start calculation:
    for (var targetPosition = 0; weight < 1 / 3; targetPosition += 4, weight += ratioWeight) {
        for (finalOffset = targetPosition, pixelOffset = 0; finalOffset < this.widthPassResultSize; pixelOffset += this.originalWidthMultipliedByChannels
, finalOffset += this.targetWidthMultipliedByChannels) {
            outputBuffer[finalOffset] = buffer[pixelOffset];
            outputBuffer[finalOffset + 1] = buffer[pixelOffset + 1];
            outputBuffer[finalOffset + 2] = buffer[pixelOffset + 2];
            outputBuffer[finalOffset + 3] = buffer[pixelOffset + 3];
        }
    }
    //Adjust for overshoot of the last pass's counter:
    weight -= 1 / 3;
    for (var interpolationWidthSourceReadStop = this.widthOriginal - 1; weight < interpolationWidthSourceReadStop; targetPosition
 += 4, weight += ratioWeight) {
        //Calculate weightings:
        secondWeight = weight % 1;
        firstWeight = 1 - secondWeight;
        //Interpolate:
        for (finalOffset = targetPosition, pixelOffset = Math.floor(weight) * 4; finalOffset < this.widthPassResultSize; pixelOffset
 += this.originalWidthMultipliedByChannels, finalOffset += this.targetWidthMultipliedByChannels) {
            outputBuffer[finalOffset] = (buffer[pixelOffset] * firstWeight) + (buffer[pixelOffset + 4] * secondWeight);
            outputBuffer[finalOffset + 1] = (buffer[pixelOffset + 1] * firstWeight) + (buffer[pixelOffset + 5] * secondWeight);
            outputBuffer[finalOffset + 2] = (buffer[pixelOffset + 2] * firstWeight) + (buffer[pixelOffset + 6] * secondWeight);
            outputBuffer[finalOffset + 3] = (buffer[pixelOffset + 3] * firstWeight) + (buffer[pixelOffset + 7] * secondWeight);
        }
    }
    //Handle for only one interpolation input being valid for end calculation:
    for (interpolationWidthSourceReadStop = this.originalWidthMultipliedByChannels - 4; targetPosition < this.targetWidthMultipliedByChannels
; targetPosition += 4) {
        for (finalOffset = targetPosition, pixelOffset = interpolationWidthSourceReadStop; finalOffset < this.widthPassResultSize
; pixelOffset += this.originalWidthMultipliedByChannels, finalOffset += this.targetWidthMultipliedByChannels) {
            outputBuffer[finalOffset] = buffer[pixelOffset];
            outputBuffer[finalOffset + 1] = buffer[pixelOffset + 1];
            outputBuffer[finalOffset + 2] = buffer[pixelOffset + 2];
            outputBuffer[finalOffset + 3] = buffer[pixelOffset + 3];
        }
    }
    return outputBuffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jimp.resize.prototype.resizeWidthRGB"></a>[function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>resizeWidthRGB (buffer)](#apidoc.element.jimp.resize.prototype.resizeWidthRGB)
- description and source-code
```javascript
resizeWidthRGB = function (buffer) {
    var ratioWeight = this.ratioWeightWidthPass;
    var ratioWeightDivisor = 1 / ratioWeight;
    var weight = 0;
    var amountToNext = 0;
    var actualPosition = 0;
    var currentPosition = 0;
    var line = 0;
    var pixelOffset = 0;
    var outputOffset = 0;
    var nextLineOffsetOriginalWidth = this.originalWidthMultipliedByChannels - 2;
    var nextLineOffsetTargetWidth = this.targetWidthMultipliedByChannels - 2;
    var output = this.outputWidthWorkBench;
    var outputBuffer = this.widthBuffer;
    do {
        for (line = 0; line < this.originalHeightMultipliedByChannels;) {
            output[line++] = 0;
            output[line++] = 0;
            output[line++] = 0;
        }
        weight = ratioWeight;
        do {
            amountToNext = 1 + actualPosition - currentPosition;
            if (weight >= amountToNext) {
                for (line = 0, pixelOffset = actualPosition; line < this.originalHeightMultipliedByChannels; pixelOffset += nextLineOffsetOriginalWidth
) {
                    output[line++] += buffer[pixelOffset++] * amountToNext;
                    output[line++] += buffer[pixelOffset++] * amountToNext;
                    output[line++] += buffer[pixelOffset] * amountToNext;
                }
                currentPosition = actualPosition = actualPosition + 3;
                weight -= amountToNext;
            } else {
                for (line = 0, pixelOffset = actualPosition; line < this.originalHeightMultipliedByChannels; pixelOffset += nextLineOffsetOriginalWidth
) {
                    output[line++] += buffer[pixelOffset++] * weight;
                    output[line++] += buffer[pixelOffset++] * weight;
                    output[line++] += buffer[pixelOffset] * weight;
                }
                currentPosition += weight;
                break;
            }
        } while (weight > 0 && actualPosition < this.originalWidthMultipliedByChannels);
        for (line = 0, pixelOffset = outputOffset; line < this.originalHeightMultipliedByChannels; pixelOffset += nextLineOffsetTargetWidth
) {
            outputBuffer[pixelOffset++] = output[line++] * ratioWeightDivisor;
            outputBuffer[pixelOffset++] = output[line++] * ratioWeightDivisor;
            outputBuffer[pixelOffset] = output[line++] * ratioWeightDivisor;
        }
        outputOffset += 3;
    } while (outputOffset < this.targetWidthMultipliedByChannels);
    return outputBuffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jimp.resize.prototype.resizeWidthRGBA"></a>[function <span class="apidocSignatureSpan">jimp.resize.prototype.</span>resizeWidthRGBA (buffer)](#apidoc.element.jimp.resize.prototype.resizeWidthRGBA)
- description and source-code
```javascript
resizeWidthRGBA = function (buffer) {
    var ratioWeight = this.ratioWeightWidthPass;
    var ratioWeightDivisor = 1 / ratioWeight;
    var weight = 0;
    var amountToNext = 0;
    var actualPosition = 0;
    var currentPosition = 0;
    var line = 0;
    var pixelOffset = 0;
    var outputOffset = 0;
    var nextLineOffsetOriginalWidth = this.originalWidthMultipliedByChannels - 3;
    var nextLineOffsetTargetWidth = this.targetWidthMultipliedByChannels - 3;
    var output = this.outputWidthWorkBench;
    var outputBuffer = this.widthBuffer;
    do {
        for (line = 0; line < this.originalHeightMultipliedByChannels;) {
            output[line++] = 0;
            output[line++] = 0;
            output[line++] = 0;
            output[line++] = 0;
        }
        weight = ratioWeight;
        do {
            amountToNext = 1 + actualPosition - currentPosition;
            if (weight >= amountToNext) {
                for (line = 0, pixelOffset = actualPosition; line < this.originalHeightMultipliedByChannels; pixelOffset += nextLineOffsetOriginalWidth
) {
                    output[line++] += buffer[pixelOffset++] * amountToNext;
                    output[line++] += buffer[pixelOffset++] * amountToNext;
                    output[line++] += buffer[pixelOffset++] * amountToNext;
                    output[line++] += buffer[pixelOffset] * amountToNext;
                }
                currentPosition = actualPosition = actualPosition + 4;
                weight -= amountToNext;
            } else {
                for (line = 0, pixelOffset = actualPosition; line < this.originalHeightMultipliedByChannels; pixelOffset += nextLineOffsetOriginalWidth
) {
                    output[line++] += buffer[pixelOffset++] * weight;
                    output[line++] += buffer[pixelOffset++] * weight;
                    output[line++] += buffer[pixelOffset++] * weight;
                    output[line++] += buffer[pixelOffset] * weight;
                }
                currentPosition += weight;
                break;
            }
        } while (weight > 0 && actualPosition < this.originalWidthMultipliedByChannels);
        for (line = 0, pixelOffset = outputOffset; line < this.originalHeightMultipliedByChannels; pixelOffset += nextLineOffsetTargetWidth
) {
            outputBuffer[pixelOffset++] = output[line++] * ratioWeightDivisor;
            outputBuffer[pixelOffset++] = output[line++] * ratioWeightDivisor;
            outputBuffer[pixelOffset++] = output[line++] * ratioWeightDivisor;
            outputBuffer[pixelOffset] = output[line++] * ratioWeightDivisor;
        }
        outputOffset += 4;
    } while (outputOffset < this.targetWidthMultipliedByChannels);
    return outputBuffer;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jimp.resize2"></a>[module jimp.resize2](#apidoc.module.jimp.resize2)

#### <a name="apidoc.element.jimp.resize2._interpolate2D"></a>[function <span class="apidocSignatureSpan">jimp.resize2.</span>_interpolate2D (src, dst, options, interpolate)](#apidoc.element.jimp.resize2._interpolate2D)
- description and source-code
```javascript
_interpolate2D = function (src, dst, options, interpolate) {

    var bufSrc = src.data;
    var bufDst = dst.data;

    var wSrc = src.width;
    var hSrc = src.height;
    //console.log("wSrc="+wSrc + ", hSrc="+hSrc + ", srcLen="+bufSrc.length);

    var wDst = dst.width;
    var hDst = dst.height;
    //console.log("wDst="+wDst + ", hDst="+hDst + ", dstLen="+bufDst.length);

    // when dst smaller than src/2, interpolate first to a multiple between 0.5 and 1.0 src, then sum squares
    var wM = Math.max(1, Math.floor(wSrc / wDst));
    var wDst2 = wDst * wM;
    var hM = Math.max(1, Math.floor(hSrc / hDst));
    var hDst2 = hDst * hM;
    //console.log("wM="+wM + ", wDst2="+wDst2 + ", hM="+hM + ", hDst2="+hDst2);

    // ===========================================================
    // Pass 1 - interpolate rows
    // buf1 has width of dst2 and height of src
    var buf1 = new Buffer(wDst2 * hSrc * 4);
    for (var i = 0; i < hSrc; i++) {
        for (var j = 0; j < wDst2; j++) {
            // i in src coords, j in dst coords

            // calculate x in src coords
            // this interpolation requires 4 sample points and the two inner ones must be real
            // the outer points can be fudged for the edges.
            // therefore (wSrc-1)/wDst2
            var x = j * (wSrc-1) / wDst2;
            var xPos = Math.floor(x);
            var t = x - xPos;
            var srcPos = (i * wSrc + xPos) * 4;

            var buf1Pos = (i * wDst2 + j) * 4;
            for (var k = 0; k < 4; k++) {
                var kPos = srcPos + k;
                var x0 = (xPos > 0) ? bufSrc[kPos - 4] : 2*bufSrc[kPos]-bufSrc[kPos+4];
                var x1 = bufSrc[kPos];
                var x2 = bufSrc[kPos + 4];
                var x3 = (xPos < wSrc - 2) ? bufSrc[kPos + 8] : 2*bufSrc[kPos + 4]-bufSrc[kPos];
                buf1[buf1Pos+k] = interpolate(x0,x1,x2,x3,t);
            }
        }
    }
    //this._writeFile(wDst2, hSrc, buf1, "out/buf1.jpg");

    // ===========================================================
    // Pass 2 - interpolate columns
    // buf2 has width and height of dst2
    var buf2 = new Buffer(wDst2 * hDst2 * 4);
    for (var i = 0; i < hDst2; i++) {
        for (var j = 0; j < wDst2; j++) {
            // i&j in dst2 coords

            // calculate y in buf1 coords
            // this interpolation requires 4 sample points and the two inner ones must be real
            // the outer points can be fudged for the edges.
            // therefore (hSrc-1)/hDst2
            var y = i * (hSrc-1) / hDst2;
            var yPos = Math.floor(y);
            var t = y - yPos;
            var buf1Pos = (yPos * wDst2 + j) * 4;
            var buf2Pos = (i * wDst2 + j) * 4;
            for (var k = 0; k < 4; k++) {
                var kPos = buf1Pos + k;
                var y0 = (yPos > 0) ? buf1[kPos - wDst2*4] : 2*buf1[kPos]-buf1[kPos + wDst2*4];
                var y1 = buf1[kPos];
                var y2 = buf1[kPos + wDst2*4];
                var y3 = (yPos < hSrc-2) ? buf1[kPos + wDst2*8] : 2*buf1[kPos + wDst2*4]-buf1[kPos];

                buf2[buf2Pos + k] = interpolate(y0,y1,y2,y3,t);
            }
        }
    }
    //this._writeFile(wDst2, hDst2, buf2, "out/buf2.jpg");

    // ===========================================================
    // Pass 3 - scale to dst
    var m = wM * hM;
    if (m > 1) {
        for (var i = 0; i < hDst; i++) {
            for (var j = 0; j < wDst; j++) {
                // i&j in dst bounded coords
                var r = 0;
                var g = 0;
                var b = 0;
                var a = 0;
                for (var y = 0; y < hM; y++) {
                    var yPos = i * hM + y;
                    for (var x = 0; x < wM; x++) {
                        var xPos = j * wM + x;
                        var xyPos = (yPos * wDst2 + xPos) * 4;
                        r += buf2[xyPos];
                        g += buf2[xyPos+1];
                        b += buf2[xyPos+2]; ...
```
- example usage
```shell
...
    var interpolateCubic = function(x0, x1, x2, x3, t) {
        var a0 = x3 - x2 - x0 + x1;
        var a1 = x0 - x1 - a0;
        var a2 = x2 - x0;
        var a3 = x1;
        return Math.max(0,Math.min(255,(a0 * (t * t * t)) + (a1 * (t * t)) + (a2 * t) + (a3)));
    }
    return this._interpolate2D(src, dst, options, interpolateCubic);
},

hermiteInterpolation: function(src, dst, options) {
    var interpolateHermite = function(x0, x1, x2, x3, t)
    {
        var c0 = x1;
        var c1 = 0.5 * (x2 - x0);
...
```

#### <a name="apidoc.element.jimp.resize2.bezierInterpolation"></a>[function <span class="apidocSignatureSpan">jimp.resize2.</span>bezierInterpolation (src, dst, options)](#apidoc.element.jimp.resize2.bezierInterpolation)
- description and source-code
```javascript
bezierInterpolation = function (src, dst, options) {
    // between 2 points y(n), y(n+1), use next points out, y(n-1), y(n+2)
    // to predict control points (a & b) to be placed at n+0.5
    //  ya(n) = y(n) + (y(n+1)-y(n-1))/4
    //  yb(n) = y(n+1) - (y(n+2)-y(n))/4
    // then use std bezier to interpolate [n,n+1)
    //  y(n+t) = y(n)*(1-t)^3 + 3 * ya(n)*(1-t)^2*t + 3 * yb(n)*(1-t)*t^2 + y(n+1)*t^3
    //  note the 3* factor for the two control points
    // for edge cases, can choose:
    //  y(-1) = y(0) - 2*(y(1)-y(0))
    //  y(w) = y(w-1) + 2*(y(w-1)-y(w-2))
    // but can go with y(-1) = y(0) and y(w) = y(w-1)
    var interpolateBezier = function(x0, x1, x2, x3, t) {
        // x1, x2 are the knots, use x0 and x3 to calculate control points
        var cp1 = x1 + (x2-x0)/4;
        var cp2 = x2 - (x3-x1)/4;
        var nt = 1-t;
        var c0 =      x1 * nt * nt * nt;
        var c1 = 3 * cp1 * nt * nt *  t;
        var c2 = 3 * cp2 * nt *  t *  t;
        var c3 =      x2 *  t *  t *  t;
        return Math.max(0,Math.min(255,Math.round(c0 + c1 + c2 + c3)));
    }
    return this._interpolate2D(src, dst, options, interpolateBezier);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jimp.resize2.bicubicInterpolation"></a>[function <span class="apidocSignatureSpan">jimp.resize2.</span>bicubicInterpolation (src, dst, options)](#apidoc.element.jimp.resize2.bicubicInterpolation)
- description and source-code
```javascript
bicubicInterpolation = function (src, dst, options) {
    var interpolateCubic = function(x0, x1, x2, x3, t) {
        var a0 = x3 - x2 - x0 + x1;
        var a1 = x0 - x1 - a0;
        var a2 = x2 - x0;
        var a3 = x1;
        return Math.max(0,Math.min(255,(a0 * (t * t * t)) + (a1 * (t * t)) + (a2 * t) + (a3)));
    }
    return this._interpolate2D(src, dst, options, interpolateCubic);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jimp.resize2.bilinearInterpolation"></a>[function <span class="apidocSignatureSpan">jimp.resize2.</span>bilinearInterpolation (src, dst, options)](#apidoc.element.jimp.resize2.bilinearInterpolation)
- description and source-code
```javascript
bilinearInterpolation = function (src, dst, options) {

    var wSrc = src.width;
    var hSrc = src.height;
    //console.log("wSrc="+wSrc + ", hSrc="+hSrc);

    var wDst = dst.width;
    var hDst = dst.height;
    //console.log("wDst="+wDst + ", hDst="+hDst);

    var bufSrc = src.data;
    var bufDst = dst.data;

    var interpolate = function(k, kMin, vMin, kMax, vMax) {
        // special case - k is integer
        if (kMin === kMax) {
            return vMin;
        }

        return Math.round((k - kMin) * vMax + (kMax - k) * vMin);
    };
    var assign = function(pos, offset, x, xMin, xMax, y, yMin, yMax) {
        var posMin = (yMin * wSrc + xMin) * 4 + offset;
        var posMax = (yMin * wSrc + xMax) * 4 + offset;
        var vMin = interpolate(x, xMin, bufSrc[posMin], xMax, bufSrc[posMax]);

        // special case, y is integer
        if (yMax === yMin) {
            bufDst[pos+offset] = vMin;
        } else {
            posMin = (yMax * wSrc + xMin) * 4 + offset;
            posMax = (yMax * wSrc + xMax) * 4 + offset;
            var vMax = interpolate(x, xMin, bufSrc[posMin], xMax, bufSrc[posMax]);

            bufDst[pos+offset] = interpolate(y, yMin, vMin, yMax, vMax);
        }
    }

    for (var i = 0; i < hDst; i++) {
        for (var j = 0; j < wDst; j++) {
            var posDst = (i * wDst + j) * 4;

            // x & y in src coordinates
            var x = j * wSrc / wDst;
            var xMin = Math.floor(x);
            var xMax = Math.min(Math.ceil(x), wSrc-1);

            var y = i * hSrc / hDst;
            var yMin = Math.floor(y);
            var yMax = Math.min(Math.ceil(y), hSrc-1);

            assign(posDst, 0, x, xMin, xMax, y, yMin, yMax);
            assign(posDst, 1, x, xMin, xMax, y, yMin, yMax);
            assign(posDst, 2, x, xMin, xMax, y, yMin, yMax);
            assign(posDst, 3, x, xMin, xMax, y, yMin, yMax);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jimp.resize2.hermiteInterpolation"></a>[function <span class="apidocSignatureSpan">jimp.resize2.</span>hermiteInterpolation (src, dst, options)](#apidoc.element.jimp.resize2.hermiteInterpolation)
- description and source-code
```javascript
hermiteInterpolation = function (src, dst, options) {
    var interpolateHermite = function(x0, x1, x2, x3, t)
    {
        var c0 = x1;
        var c1 = 0.5 * (x2 - x0);
        var c2 = x0 - (2.5 * x1) + (2 * x2) - (0.5 * x3);
        var c3 = (0.5 * (x3 - x0)) + (1.5 * (x1 - x2));
        return  Math.max(0,Math.min(255,Math.round((((((c3 * t) + c2) * t) + c1) * t) + c0)));
    }
    return this._interpolate2D(src, dst, options, interpolateHermite);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jimp.resize2.nearestNeighbor"></a>[function <span class="apidocSignatureSpan">jimp.resize2.</span>nearestNeighbor (src, dst, options)](#apidoc.element.jimp.resize2.nearestNeighbor)
- description and source-code
```javascript
nearestNeighbor = function (src, dst, options) {

    var wSrc = src.width;
    var hSrc = src.height;
    //console.log("wSrc="+wSrc + ", hSrc="+hSrc);

    var wDst = dst.width;
    var hDst = dst.height;
    //console.log("wDst="+wDst + ", hDst="+hDst);

    var bufSrc = src.data;
    var bufDst = dst.data;

    for (var i = 0; i < hDst; i++) {
        for (var j = 0; j < wDst; j++) {
            var posDst = (i * wDst + j) * 4;

            var iSrc = Math.round(i * hSrc / hDst);
            var jSrc = Math.round(j * wSrc / wDst);
            var posSrc = (iSrc * wSrc + jSrc) * 4;

            bufDst[posDst++] = bufSrc[posSrc++];
            bufDst[posDst++] = bufSrc[posSrc++];
            bufDst[posDst++] = bufSrc[posSrc++];
            bufDst[posDst++] = bufSrc[posSrc++];
        }
    }
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
