---
title: Optimise your Webflow site
date: Last Modified
permalink: /settings/optimise/index.html
eleventyNavigation:
  key: optimise
  order: 51
  parent: settings
  title: Configure optimisations
---

Flowty can automatically apply optimisations to your Webflow site's images, CSS, JavaScript, and more. Optimisations can be easily toggled on/off in the Flowty Dashboard.

Any item marked with `default` below is a base Flowty configuration, and will be turned on the first time your site builds using Flowty.

## Image optimisations
Flowty's image optimisations allow you to use modern WebP and AVIF formats on your Webflow site.

### Download `default`
Images can be downloaded, and served from the same domain as the website itself. This helps with performance, and ensures they are hosted sustainably if a green web host is used.

### WebP and AVIF
Webflow does not serve WebP or AVIF versions of images. Flowty runs all images through an optimisation step and serves modern formats with a fallback for older browsers.

### Automatically set lazy loading `default`
With lazy loading applied to images, the browser will wait to download images until the user is just about to see them. This help reduce the amount of data used when a site is first loaded.

### Optimise CSS background images
Background images that are requested via CSS also get downloaded locally, and run through an optimisation step to reduce their size.

## CSS 
CSS optimisations available in Flowty allow you to reduce the CSS loaded on each page of your site.

### Download `default`
Your Webflow site's CSS can be downloaded, and served from the same domain as the website itself. This helps with performance, and ensures they are hosted sustainably if a green web host is used.

### Inline critical CSS
An optional step to help with performance. Flowty extracts the CSS required for the initial rendering of a page, and inlines it into the HTML.

### Remove unused CSS
An optional step that should be used with care. Flowty checks each page, and generates a file CSS that includes only the declarations required by that page. This can greatly reduce the CSS file size for some pages.

## JavaScript
Download and minify, or complete remove, your site's Webflow JavaScript files.

### Download `default`
Your Webflow site's JavaScript and jQuery files can be downloaded, and served from the same domain as the website itself. This helps with performance, and ensures they are hosted sustainably if a green web host is used.

### Remove
Some sites don’t much interactivity. In these cases, designers can save kilobytes by removing the Webflow JS or jQuery files from the site.

### Minify `default`
Sites on Webflow’s free plan come with unminified JS. Flowty runs a minification step on the Javascript files it downloads, to reduce their transfer size.

### Download JavaScript from CDNs
You can also choose to have Flowty download JavaScript files that are used on your site from known JavaScript CDNs. This can help with performance, and also lets you be sure those files are being served from a green web host.

## Font optimisations
Webflow allows designers to use Google Fonts or upload their own custom fonts. Flowty downloads these font files and hosts them on the same origin as the site itself.

::: callout
*Flowty only has options to download Google Fonts, and Webflow custom fonts.*
:::

## Video optimisations
Download background videos, and reduce the size of YouTube embeds on your Webflow site.

### Download
Your Webflow site's background video files can be downloaded, and served from the same domain as the website itself. This helps with performance, and ensures they are hosted sustainably if a green web host is used.

### Optimise Youtube embeds
Flowty uses the [Lite Youtube Embed](https://github.com/paulirish/lite-youtube-embed) package to significantly reduce the amount of data consumed by embedded Youtube videos when a page is first loaded.

## Optimise other embeds
Flowty can also help optimise other types of embedded content.

### Lazy load iframes
Adds the `loading="lazy"` attribute to iframe tags, allowing the browser to defer download their content until just before the user will see it.

## Other optimisations

- Remove the “Made in Webflow” branding on pages. `default`
- Download website metadata (icons, open graph images etc) and host them locally. `default`
- Use [instant.page](https://instant.page) to improve site navigation.