---
title: Sitemap and robots.txt
date: Last Modified
permalink: /settings/seo/index.html
eleventyNavigation:
  key: optimise
  order: 52
  parent: settings
  title: Sitemap and robots.txt
---

You can include or exclude pages from the 

## Generate a sitemap
Generate a sitemap for your Webflow site, to help search engines find your content. 

### Set a custom domain
By default, Flowty will use your site's Webflow staging URL when building your sitemap. This is less than ideal, especially if you are using a custom domain to host your site.

You can set a custom domain for your site by updating the `customDomain` attribute in your project's `src/_data/config.js` file.

```js
module.exports = {
  "webflowUrl": "https://your-site.webflow.io",
  "customDomain": "https://www.my-site.com",
  // Remaining settings removed for brevity
  ...
}
```
### Excluding pages from the sitemap
You can exclude a page from the sitemap by adding its path to the `sitemapExclude` array in your `src/_data/config.js` file. 

```js
module.exports = {
  // ...
  "sitemapExclude": ["/404", "/a-page", "/another-page", "/blog/a-blog-post"],
  // ...
}
```

### Robots.txt
Robots.txt files allow you to tell search engines to ignore certain pages/parts of your site.

### Block pages from indexing
You can exclude a page from indexing by robots by adding its path to the `noindex` array in your `src/_data/config.js` file. 

```js
module.exports = {
  // ...
  "noindex": ["/404", "/a-page", "/another-page", "/blog/a-blog-post"],
  // ...
}
```

::: callout
*There is currently no way to disallow individual pages/paths from your site's robots.txt file. However Flowty does include a `<meta name="robots" content="noindex">` in the HTML for pages you wish to exclude.*
:::