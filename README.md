# connect-fonts-moztt

MozTT fontpack for [connect-fonts](https://github.com/shane-tomlinson/connect-fonts).

## Usage

1. Include [connect-fonts](https://github.com/shane-tomlinson/connect-fonts) in a node module.
```js
const font_middleware = require("connect-fonts");
```

2. Include the font packs that you want to serve.
```js
const font_pack  = require("connect-fonts-moztt");
```

3. Add a middleware by calling the `setup` function.
```js
    app.use(font_middleware.setup({
      fonts: [ font_pack ],
      allow_origin: "https://exampledomain.com"
    }));
```

4. Add a link tag to include the font CSS.
```html
<link href="/moztt-bold/fonts.css" type="text/css" rel="stylesheet"/ >
```

Multiple fonts from the family can be included by using a comma separated list of fonts:
```html
<link href="/moztt-bold,moztt-light,moztt-medium,moztt-regular/fonts.css" type="text/css" rel="stylesheet"/ >
```

Available fonts:
* moztt-bold
* moztt-light
* moztt-medium
* moztt-regular

Locale-optimised font sets can be served by specifying the locale in the fonts.css URL.
```html
<link href="/latin/moztt-bold/fonts.css" type="text/css" rel="stylesheet"/ >
```

Available subsets:
* latin
* en

5. Set your CSS up to use the new font by using the "MozTT" font-family.
```
    body {
      font-family: 'MozTT', 'sans-serif', 'serif';
    }
```

## Font Info
MozTT

* Description: Copyright (c) 2012 by Ralph du Carrois & Erik Spiekermann. All rights reserved.
* Copyright: Copyright (c) 2012 by Ralph du Carrois & Erik Spiekermann. All rights reserved.
* Designer: Ralph du Carrois & Erik Spiekermann
* Designer URL: http://www.edemspiekermann.com 
* Vendor: Ralph du Carrois & Erik Spiekermann
* Vendor URL: http://www.edemspiekermann.com

## Development Info
* Homepage: https://github.com/shane-tomlinson/connect-fonts-moztt
* Repo: https://github.com/shane-tomlinson/connect-fonts-moztt

## Author
* Shane Tomlinson
* shane@shanetomlinson.com
* stomlinson@mozilla.com
* set117@yahoo.com
* https://shanetomlinson.com
* https://github.com/shane-tomlinson
* https://github.com/stomlinson
* @shane_tomlinson


## License

Software: Licenced under version 2.0 of the MPL

  https://www.mozilla.org/MPL/


  

