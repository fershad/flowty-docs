---
title: Flowty site settings
date: Last Modified
permalink: /settings/index.html
eleventyNavigation:
  key: settings
  order: 50
  title: Site settings
---

Your Flowty site settings can be adjusted via the `/src/_data/config.js` file. While we have set sensible defaults, you can change these at any time.

- [Set the optimisations](/settings/optimise/) that will be applied to your site.
- [Manage your sitemap](/settings/seo/) and robots.txt files.
- [Add custom code](/settings/custom-code/) to your Webflow site.

## The config file

By default, the `config.js` file for your project will look like the one below. You can turn optimisations on/off by changing the value of the corresponding property to `true` (on) or `false` (off).

```js
module.exports = {
    "webflowUrl": "", // Example: https://my-website.webflow.io
    "customDomain": "", // Example: https://my-website.com
    "css": {
        "critical": false,
        "purge": false
    },
    "embeds": {
        "optimiseYouTube": true,
        "lazyIframes": true
    },
    "js": {
        "webflow": {
            "remove": false
        },
        "jquery": {
            "remove": false
        },
    },
    "preloadNavigation": true,
    "images": {
        "webp": true,
        "avif": false,
    },
    "removeBranding": true,
    "videos": {
        "download": true,
        "disableAutoplay": false
    },
    "generateSitemap": false,
    "generateRobots": false,
    "sitemapExclude": ["/404"],
    "noindex": ["/404"],
    "customCodeHead": ``,
    "customCodeBody": ``,
}
```