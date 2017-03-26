# api documentation for  [gulp-imagemin (v3.2.0)](https://github.com/sindresorhus/gulp-imagemin#readme)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-gulp-imagemin.svg)](https://travis-ci.org/npmdoc/node-npmdoc-gulp-imagemin)
#### Minify PNG, JPEG, GIF and SVG images

[![NPM](https://nodei.co/npm/gulp-imagemin.png?downloads=true)](https://www.npmjs.com/package/gulp-imagemin)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gulp-imagemin/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-gulp-imagemin_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gulp-imagemin/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-gulp-imagemin/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Sindre Sorhus",
        "email": "sindresorhus@gmail.com",
        "url": "sindresorhus.com"
    },
    "bugs": {
        "url": "https://github.com/sindresorhus/gulp-imagemin/issues"
    },
    "dependencies": {
        "chalk": "^1.0.0",
        "gulp-util": "^3.0.0",
        "imagemin": "^5.0.0",
        "imagemin-gifsicle": "^5.0.0",
        "imagemin-jpegtran": "^5.0.0",
        "imagemin-optipng": "^5.1.0",
        "imagemin-svgo": "^5.1.0",
        "plur": "^2.0.0",
        "pretty-bytes": "^4.0.2",
        "through2-concurrent": "^1.1.0"
    },
    "description": "Minify PNG, JPEG, GIF and SVG images",
    "devDependencies": {
        "ava": "*",
        "get-stream": "^2.1.0",
        "imagemin-pngquant": "^5.0.0",
        "pify": "^2.3.0",
        "xo": "*"
    },
    "directories": {},
    "dist": {
        "shasum": "26887ad65d2c51bb317c4b02b5604f4a78bf74a8",
        "tarball": "https://registry.npmjs.org/gulp-imagemin/-/gulp-imagemin-3.2.0.tgz"
    },
    "engines": {
        "node": ">=4"
    },
    "files": [
        "index.js"
    ],
    "gitHead": "38de5c8e7c49df2147f6678eef1e39f8a50c44d7",
    "homepage": "https://github.com/sindresorhus/gulp-imagemin#readme",
    "keywords": [
        "gulpplugin",
        "imagemin",
        "image",
        "img",
        "picture",
        "photo",
        "minify",
        "minifier",
        "compress",
        "png",
        "jpg",
        "jpeg",
        "gif",
        "svg"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "sindresorhus",
            "email": "sindresorhus@gmail.com"
        },
        {
            "name": "kevva",
            "email": "kevinmartensson@gmail.com"
        }
    ],
    "name": "gulp-imagemin",
    "optionalDependencies": {
        "imagemin-gifsicle": "^5.0.0",
        "imagemin-jpegtran": "^5.0.0",
        "imagemin-optipng": "^5.1.0",
        "imagemin-svgo": "^5.1.0"
    },
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/sindresorhus/gulp-imagemin.git"
    },
    "scripts": {
        "test": "xo && ava"
    },
    "version": "3.2.0",
    "xo": {
        "esnext": true
    }
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module gulp-imagemin](#apidoc.module.gulp-imagemin)
1.  [function <span class="apidocSignatureSpan">gulp-imagemin.</span>gifsicle ()](#apidoc.element.gulp-imagemin.gifsicle)
1.  [function <span class="apidocSignatureSpan">gulp-imagemin.</span>jpegtran ()](#apidoc.element.gulp-imagemin.jpegtran)
1.  [function <span class="apidocSignatureSpan">gulp-imagemin.</span>optipng ()](#apidoc.element.gulp-imagemin.optipng)
1.  [function <span class="apidocSignatureSpan">gulp-imagemin.</span>svgo ()](#apidoc.element.gulp-imagemin.svgo)



# <a name="apidoc.module.gulp-imagemin"></a>[module gulp-imagemin](#apidoc.module.gulp-imagemin)

#### <a name="apidoc.element.gulp-imagemin.gifsicle"></a>[function <span class="apidocSignatureSpan">gulp-imagemin.</span>gifsicle ()](#apidoc.element.gulp-imagemin.gifsicle)
- description and source-code
```javascript
gifsicle = function () {
		const args = [].slice.call(arguments);
		return loadPlugin(plugin, args);
	}
```
- example usage
```shell
...
'''

### Custom plugin options

'''js
…
.pipe(imagemin([
	imagemin.gifsicle({interlaced: true}),
	imagemin.jpegtran({progressive: true}),
	imagemin.optipng({optimizationLevel: 5}),
	imagemin.svgo({plugins: [{removeViewBox: true}]})
]))
…
'''
...
```

#### <a name="apidoc.element.gulp-imagemin.jpegtran"></a>[function <span class="apidocSignatureSpan">gulp-imagemin.</span>jpegtran ()](#apidoc.element.gulp-imagemin.jpegtran)
- description and source-code
```javascript
jpegtran = function () {
		const args = [].slice.call(arguments);
		return loadPlugin(plugin, args);
	}
```
- example usage
```shell
...

### Custom plugin options

'''js
…
.pipe(imagemin([
	imagemin.gifsicle({interlaced: true}),
	imagemin.jpegtran({progressive: true}),
	imagemin.optipng({optimizationLevel: 5}),
	imagemin.svgo({plugins: [{removeViewBox: true}]})
]))
…
'''

Note that you may come across an older, implicit syntax. In versions < 3, the same was written like this:
...
```

#### <a name="apidoc.element.gulp-imagemin.optipng"></a>[function <span class="apidocSignatureSpan">gulp-imagemin.</span>optipng ()](#apidoc.element.gulp-imagemin.optipng)
- description and source-code
```javascript
optipng = function () {
		const args = [].slice.call(arguments);
		return loadPlugin(plugin, args);
	}
```
- example usage
```shell
...
### Custom plugin options

'''js
…
.pipe(imagemin([
	imagemin.gifsicle({interlaced: true}),
	imagemin.jpegtran({progressive: true}),
	imagemin.optipng({optimizationLevel: 5}),
	imagemin.svgo({plugins: [{removeViewBox: true}]})
]))
…
'''

Note that you may come across an older, implicit syntax. In versions < 3, the same was written like this:
...
```

#### <a name="apidoc.element.gulp-imagemin.svgo"></a>[function <span class="apidocSignatureSpan">gulp-imagemin.</span>svgo ()](#apidoc.element.gulp-imagemin.svgo)
- description and source-code
```javascript
svgo = function () {
		const args = [].slice.call(arguments);
		return loadPlugin(plugin, args);
	}
```
- example usage
```shell
...

'''js
…
.pipe(imagemin([
	imagemin.gifsicle({interlaced: true}),
	imagemin.jpegtran({progressive: true}),
	imagemin.optipng({optimizationLevel: 5}),
	imagemin.svgo({plugins: [{removeViewBox: true}]})
]))
…
'''

Note that you may come across an older, implicit syntax. In versions < 3, the same was written like this:

'''js
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
