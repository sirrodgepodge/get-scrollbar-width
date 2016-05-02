# get-scrollbar-width
Utility function to determine the scrollbar width of the current browser, returns zero if running server-side

I find this utility function particularly useful when creating a modal that blocks scrolling to determine how much padding is needed to prevent nasty jank from scrollbar removal.

        var getScrollbarWidth = require('get-scrollbar-width');
        
        var currentBrowserScrollbarWidth = getScrollbarWidth();
        
        console.log(currentBrowserScrollbarWidth); // value depends on browser, 15 pixels is common
