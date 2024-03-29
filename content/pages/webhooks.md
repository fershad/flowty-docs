---
title: Automatically Update on Webflow Publish
date: Last Modified
permalink: /webhooks/index.html
eleventyNavigation:
  key: webhooks
  order: 40
  title: Automatically Update on Webflow Publish
---

Webhooks provide a way for Webflow to let your hosting provider know whenever a change has been made to your site. This can then automatically trigger a new website build that updates your Flowty site with the new content.

## Create a webhook on your host
First you will need a create a webhook on your site's hosting service. Below are links to instructions for some popular services:

- [Deploy Hooks on Cloudflare Pages](https://developers.cloudflare.com/pages/platform/deploy-hooks)
- [Build Hooks on Netlify](https://docs.netlify.com/configure-builds/build-hooks/)
- [Deploy Hooks on Vercel](https://vercel.com/docs/concepts/git/deploy-hooks)
- [Deploy Hooks on Render](https://render.com/docs/deploy-hooks)

## Adding webhooks to Webflow
Once you have created a webhook on your hosting service it needs to be added to Webflow.

1. In Webflow, go to your site's **Project Settings**.
1. Navigate to **Integrations**.
1. At the very bottom of the page you will see a section titled _Webhooks_.
1. Press **+ Add Webhook**.
1. Select `Site publish` as the trigger.
1. Paste in the webhook URL that you created on your site's host.
1. Press **Add Webhook** to complete the process.

If this is set up properly, then a new build of your site should be triggered next time you publish an update on Webflow.