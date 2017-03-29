Inspired by [prerender-spa-plugin](https://github.com/chrisvfritz/prerender-spa-plugin), but prerenders static HTML in multi-page application.

### Usage

``` js
// webpack.conf.js
const path = require('path')
const PrerenderMultiPagePlugin = require('prerender-multi-page-plugin')

module.exports = {
 // ...
 plugins: [
   new PrerenderMultiPagePlugin(
     path.join(__dirname, '../dist'), [ '/index.html', '/about.html', '/help.html' ]
   )
 ]
}
```
