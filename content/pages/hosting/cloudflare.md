---
title: Connect to Cloudflare Pages
date: Last Modified
permalink: /hosting/cloudflare/index.html
eleventyNavigation:
  key: hosting-cloudflare
  order: 31
  parent: hosting
  title: Connect to Cloudflare Pages
---

Follow the [instructions in the Cloudflare docs](https://developers.cloudflare.com/pages/get-started/) to setup a new Pages project, and connect it to your git repository.

## Build settings
Pleaes take special note of the below build settings that you will need to apply:

- **Build command**: `npm run build`
- **Build output directory**: `flowty/_site`

## Environment variables
You will also need to include the following environment variables that will be used when your site builds.

- **CONFIG_SITE_ID**: Your site ID (you can find this in the Flowty dashboard).
- **NODE_VERSION**: `v16`

::: callout
*Note: Environment variables are case sensitive.*
:::

Once you press **Save and deploy** your site will start building with Flowty's default settings. This might take a few minutes to complete depending on the site of your site.

{% image "cloudflare.png" "Cloudflare Pages setup" "600px" %}