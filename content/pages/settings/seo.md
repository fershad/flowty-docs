---
title: Webflow sitemap and robots.txt
date: Last Modified
permalink: /settings/seo/index.html
eleventyNavigation:
  key: seo
  order: 52
  parent: settings
  title: Configure sitemap and robots.txt
---

In your site's dashboard, navigate to the **SEO** tab to adjust theese settings. Both the sitemap and robots.txt options are disabled by default.

## Generate a sitemap
Generate a sitemap for your Webflow site, to help search engines find your content. 

### Set a custom domain
By default, Flowty will use your site's Webflow staging URL when building your sitemap. This is less than ideal, especially if you are using a custom domain to host your site.

You can [set a custom domain](/settings/website/) for your site in the **Website settings** tab. If set, it will be used as the base URL for your sitemap when it is generated.

::: callout
*Currently all pages of your site will be included in the sitemap. I am actively working on a way for users to selectively exclude pages.*
:::

### Robots.txt
Robots.txt files allow you to tell search engines to ignore certain pages/parts of your site.

::: callout
*There is currently no way to disallow individual pages/paths from your site's robots.txt file.*
:::