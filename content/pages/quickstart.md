---
title: Getting started
date: Last Modified
permalink: /getting-started/index.html
eleventyNavigation:
  key: quickstart
  order: 10
  title: Getting started
---

To start using Flowty [clone or download the code](https://github.com/fershad/flowty) that is available on GitHub.

## Configure your site

Once you have got the code from GitHub, navigate to the `/src/_data/config.js` file. In here, add the Webflow URL of your site to the `webflowUrl` field.

If you are planning to host your site on a custom domain, then you can also add that in this file.

```js
module.exports = {
  "webflowUrl": "https://your-site.webflow.io",
  "customDomain": "https://www.my-site.com",
  // Remaining settings removed for brevity
  ...
}
```

::: callout 
*Note: Your Webflow staging URL should end in `.webflow.io`.*
:::