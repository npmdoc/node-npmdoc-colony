# npmdoc-colony

#### api documentation for  [colony (v0.0.7)](https://github.com/hughsk/colony)  [![npm package](https://img.shields.io/npm/v/npmdoc-colony.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-colony) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-colony.svg)](https://travis-ci.org/npmdoc/node-npmdoc-colony)

#### In-browser network graphs representing the links between your Node.js code and its dependencies.

[![NPM](https://nodei.co/npm/colony.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/colony)

- [https://npmdoc.github.io/node-npmdoc-colony/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-colony/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-colony/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-colony/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-colony/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-colony/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Hugh Kennedy",
        "url": "http://hughskennedy.com/"
    },
    "bin": {
        "colony": "bin/colony"
    },
    "bugs": {
        "url": "https://github.com/hughsk/colony/issues"
    },
    "dependencies": {
        "async": "~0.1.22",
        "debounce": "0.0.3",
        "ejs": "~0.8.3",
        "highlight.js": "~7.2.0",
        "marked": "~0.2.5",
        "optimist": "~0.3.4",
        "reqursive": "0.0.6",
        "wrench": "~1.3.9"
    },
    "description": "In-browser network graphs representing the links between your Node.js code and its dependencies.",
    "devDependencies": {
        "browserify": "~1.16.1",
        "d3": "~2.10.1",
        "debounce": "0.0.1",
        "mousetrap": "0.0.1",
        "uglify-js": "~1.3.3"
    },
    "directories": {},
    "dist": {
        "shasum": "a3fdcc49deb01487d799201c74c2d5f3ceeb48a3",
        "tarball": "https://registry.npmjs.org/colony/-/colony-0.0.7.tgz"
    },
    "homepage": "https://github.com/hughsk/colony",
    "keywords": [
        "code",
        "visualisation",
        "require",
        "recursive",
        "structure",
        "codebase",
        "visualization"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "hughsk"
        }
    ],
    "name": "colony",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/hughsk/colony.git"
    },
    "scripts": {
        "browserify": "browserify src/index.js -o public/js/colony.js",
        "minify": "uglifyjs public/js/colony.js > public/js/colony.min.js",
        "pages": "rm -rf gh-pages; bin/colony ./index.js ./src/index.js -o gh-pages -r instructions.md -f hughsk/colony",
        "prepublish": "(mkdir -p public/js || true); npm run browserify && npm run minify",
        "test": "echo \"Sorry, no tests as of yet!\" && exit 1"
    },
    "version": "0.0.7"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
