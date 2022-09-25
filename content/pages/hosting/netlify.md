---
title: Connect to Netlify
date: Last Modified
permalink: /hosting/netlify/index.html
eleventyNavigation:
  key: hosting-netlify
  order: 32
  parent: hosting
  title: Connect to Netlify
---

Follow the [instructions in the Netlify docs](https://docs.netlify.com/welcome/add-new-site/#import-from-an-existing-repository) to setup a new project, and connect it to your git repository.

## Build settings
Pleaes take special note of the below build settings that you will need to apply:

- **Build command**: `npm run build`
- **Publish directory**: `_site`

## Advanced build settings
You will also need to include the following variables that will be used when your site builds.

- **NODE_VERSION**: `v16`

::: callout
*Note: Environment variables are case sensitive.*
:::

Once you press **Deploy site** your site will start building with Flowty's default settings. This might take a few minutes to complete depending on the site of your site.
