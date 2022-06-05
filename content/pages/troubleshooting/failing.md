---
title: Failing builds
date: Last Modified
permalink: /failing-builds/index.html
eleventyNavigation:
  key: failing-builds
  parent: troubleshooting
  order: 72
  title: Failing builds
---

If you find that your Flowty website is failing to build, there are a few things you can try:

- Ensure there is no problem with your website host.
- Turn off AVIF image optimisations.
    - AVIF optimisations are very resource intensive, and could cause your site build to time out.
- Turn off all CSS optimisations
    - Like AVIF, these build steps can be resource intensive and might cause your build to fail.
- Ensure that your [Flowty site is verified](/verify-site/).
- Ensure that your Webflow Staging URL is online, and publicly accessible.