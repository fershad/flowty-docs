---
title: Add custom code to your Webflow site
date: Last Modified
permalink: /settings/custom-code/index.html
---

Adding custom code to your site is currently only possible with a Webflow Site plan. Flowty allows you to add custom code snippets to the `head` and `body` sections of your site. This gives you a way to add custom functionality, analytics scripts, and other services your site.

You can add custom code in your site's `src/_data/config.js` file. Add your code to either the `customCodeHead` or `customCodeBody`.

```js
module.exports = {
    // ...
    "customCodeHead": ``, 
    "customCodeBody": ``,
    // ...
}
```

::: callout
*Custom code is applied to each page of your site. Page-level custom code functionality is not available.*
:::

