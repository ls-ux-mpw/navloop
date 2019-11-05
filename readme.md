# "Nav Loop" Correction

```js
$(document).ready(function () {
  $('.bpc-search-result-title').attr('id','title');
  $('.active-selection').find('a').attr('href', '#title');
});
```

This is a single snippet of jQuery used to keep mobile users from being stuck in an endless loop of page reloads when attempting to use the nav tiles on PLPs. It adds an `id` of "title" to the page title, and changes the `href` attribute of the nav tile link to the corresponding page to an anchor link connected to the title so users scroll down instead of reloading the page.

To activate this code, copy and paste it into any Hawk content area on a PLP -- ideally below the items so the nav tiles and title have a chance to render before the script. Be sure to always add it in preview rather than production.
