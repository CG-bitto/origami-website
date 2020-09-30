---
title: Origami Newsletter, September 2020
description: This issue features image service cost saving and promoted content teasers.
author: Lee Moody
tags:
  - Newsletter
---

<abbr title="Too long; didn't read">
	<strong>
	TL;DR:
	</strong>
</abbr> {{page.description}}

## Top Things

These are some of the bigger things we've done over the last month.

### Image Service Cost Savings

The [Origami Image Service](https://www.ft.com/__origami/service/image/v2/) transforms images for many FT Group products, e.g. by format, quality, dimension, or tint. We noticed that lots of images included by our products are actually the exact same image, but hosted on a different URL. To optimise for this situation the Image Service now generates a key based on the image content. The key is compared against other images to avoid storing duplicates.

This work has saved at least ~$900 a month against our storage costs. Previously we stored 36 million images (3.34 Terabytes) which is now down to 7.8 million (0.49 Terabytes).

@todo add images

### Promoted Content Teaser

@todo we supported the ads team to roll out fully.

## Special Thanks

@todo special thanks ads team.

## Broader Update

A digest of other things that have happened since our last update:

- MINOR: [o-cookie-message](https://github.com/Financial-Times/o-cookie-message) adds a deprecation warning for unused options.
- MINOR: [o-header](https://github.com/Financial-Times/o-header) moves Customer Products style overrides into `o-header` where appropriate, to be shared with other teams consistently; fixes a regression in the transparent variant which made links difficult to see and documents the variants limitations.
- MINOR: [origami-navigation-service](https://github.com/Financial-Times/origami-navigation-service) upgrades its `o-header` example.
- MINOR: [o-topper](https://github.com/Financial-Times/o-topper) extracts Customer Products specific logic for mapping article data to a topper to [n-map-content-to-topper](https://github.com/Financial-Times/n-map-content-to-topper), which may also be used for server-side rendering (great work, Keran Braich!)
- MINOR: [origami-component-converter](https://github.com/Financial-Times/origami-component-converter) automates publishing to npm, adds a `module` entrypoint to `package.json` with an ESM build, along with the `browser` entrypoint for a CommonJS build, when components are published to npm.
- MINOR: [origami-specialist-title-logos](https://github.com/Financial-Times/origami-specialist-title-logos) adds a new FT Live logo.
- MINOR: [polyfill-service](https://github.com/Financial-Times/polyfill-service) adds a polyfill-specific hero image (thanks to Gabrielle von Koss! Gabi used to be a member of the Origami team but no longer works at the FT 💔); adds the latest version of `polyfill-library` bringing `Intl.DateTimeFormat`, `Intl.ListFormat`, `Intl.DisplayNames`, and `Intl.NumberFormat` support.
- PATCH: [o-autoinit](https://github.com/Financial-Times/o-autoinit) lists `CustomEvent` as a required polyfill.
- PATCH: [o-colors](https://github.com/Financial-Times/o-colors) corrects `oColorsMix` documentation (thanks Kiya Gurmesa!)
- PATCH: [o-forms](https://github.com/Financial-Times/o-forms) corrects suffixed button colour given valid input; improves guidance to make it harder to copy inaccessible markup.
- PATCH: [o-header-services](https://github.com/Financial-Times/o-header-services) introduces drawer navigation fixes for IE11; removes focusable elements from dropdown menus for keyboard accessibility.
- PATCH: [o-teaser](https://github.com/Financial-Times/o-teaser) updates paid post teaser to a new prompted content teaser.
- PATCH: [origami-build-tools](https://github.com/Financial-Times/origami-build-tools) compiles demos and includes the `CustomEvent` polyfill for testing in IE11.
- PATCH: [origami-component-manifest-linter](https://github.com/Financial-Times/origami-component-manifest-linter) refactors code, adds many new tests, bugfixes, and documentation.
- PATCH: [origami-template-repository](https://github.com/Financial-Times/origami-template-repository) updates to latest version of Origami workflows.
- PATCH: [scrumple](https://github.com/Financial-Times/scrumple) rewrites Scrumple JavaScript to ES5 syntax to work in IE11 without compilation.
- All components: add extension to relative JavaScript imports to make the code work directly in a browser without compilation.
