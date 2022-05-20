---
title: Connect to Vercel
date: Last Modified
permalink: /hosting/vercel/index.html
eleventyNavigation:
  key: hosting-vercel
  order: 33
  parent: hosting
  title: Connect to Vercel
---

Follow the [instructions in the Vercel docs](https://vercel.com/docs/concepts/projects/overview#git) to setup a new project, and connect it to your git repository.

## Build settings
Pleaes take special note of the below build settings that you will need to apply:

- **Build command**: `npm run build`
- **Output directory**: `flowty/_site`

## Advanced build settings
You will also need to include the following variables that will be used when your site builds.

- **CONFIG_SITE_ID**: Your site ID (you can find this in the Flowty dashboard).

::: callout
*Note: Environment variables are case sensitive.*
:::

Once you press **Deploy** your site will start building with Flowty's default settings. This might take a few minutes to complete depending on the site of your site.

{% image "vercel.png" "Vercel setup" "600px" %}