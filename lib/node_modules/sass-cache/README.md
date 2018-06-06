# sass-cache
selector-specifc cache functionality for node-sass

## How to install
`npm i sass-cache`

## How to use
```
const sass = require('node-sass'),
    sassCache = require('sass-cache');

sass.render({
        file: scss_filename,
        functions: sassCache.functions
    },
    function (err, result) {
        /*...*/
    });
```

## Features
Function Name | Params                            | Description
--------------|-----------------------------------|----------------
`cache-save`  | `selector`, `namespace`, `value`  | caches a value for that for the selector and namespace
`cache-load`  | `selector`, `namespace`           | loads cached value for the selector and namespace
