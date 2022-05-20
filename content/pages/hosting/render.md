---
title: Connect to Render.com
date: Last Modified
permalink: /hosting/render/index.html
eleventyNavigation:
  key: hosting-render
  order: 34
  parent: hosting
  title: Connect to Render.com
---

Follow the instructions below to setup a new Static Site, and connect it to your git repository, on [Render.com](https://render.com/).

## New Static Site
In the Render Dashboard, select the **New Static Site** option.

## Connect to GitHub or GitLab
If you have not already, you will be prompted to connect your Render account to GitHub or GitLab.
Once you have done this, you will be able to search for and select your site's Flowty repository.

## Build settings
Once you've selected a repository, you will be able to set the build settings for your site.
Here, you can give your site whatever name you like. Leave the `branch` field set as `main`.

Pleaes take special note of the below build settings that you will need to apply:

- **Build Command**: `npm run build`
- **Publish Directory**: `flowty/_site`

## Advanced build settings
You will also need to include the following variables that will be used when your site builds.

- **CONFIG_SITE_ID**: Your site ID (you can find this in the Flowty dashboard).
- **NODE_VERSION**: 16

::: callout
*Note: Environment variables are case sensitive.*
:::

Once you press **Deploy** your site will start building with Flowty's default settings. This might take a few minutes to complete depending on the site of your site.

{% image "render.png" "Render setup" "600px" %}