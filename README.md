# get-scrollbar-width
Utility function to determine the scrollbar width of the current browser, returns zero if running server-side

I find this utility function particularly useful when creating a modal that blocks scrolling to determine how much padding is needed to prevent nasty jank from scrollbar removal.

```js
var getScrollbarWidth = require('get-scrollbar-width');

var currentBrowserScrollbarWidth = getScrollbarWidth();

console.log(currentBrowserScrollbarWidth); // value depends on browser, 15 pixels is common
```

[![NPM][nodei-image]][nodei-url]

[nodei-image]: https://nodei.co/npm/simple-iso-fetch.png?downloads=true&downloadRank=true&stars=true
[nodei-url]: https://www.npmjs.com/package/simple-iso-fetch
