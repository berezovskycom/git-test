# Optimization tips for front-end developers

### 1. Image optimization
- compress files as much as possible.
- use retina technique (srcset).
- don't forget about lazyload [more info here](https://www.robinosborne.co.uk/2016/05/16/lazy-loading-images-dont-rely-on-javascript/).
- add wepb support.
- generate sprites for icons and small images that repeat on your page.

### 2. JS
- external scripts should load asynchronously.
- combine all your internal scripts into one file.
- use document.onload event, but not if you really need your code initialized with dom load.
- for small projects vanilla javaScript is preferable.
- compression, obviously.

### 3. Fonts
- use only Google Fonts.
- avoid FOIT (Flash of Invisible Text). You might want to use font-display, but it's not supported by many browsers yet.

### 4. CSS
- compression is your first friend. Don't use the styles you don't need.
- add critical styles (bg-color, width, etc.) to <style> tag in html, so the user will see your page before full css load.
- avoid "big" styles like animation, box-shadow, etc.
- you might want to compress class names for better DOMContentLoaded.

### 5. General
- test your changes in different browsers.
- use many testing tools. In general, be flexible.

