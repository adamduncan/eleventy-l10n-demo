# Eleventy l10n demo

Demo for handling Apache Content Negotiation in an Eleventy site.

Based on discussion in [https://github.com/11ty/eleventy/issues/761](https://github.com/11ty/eleventy/issues/761)

Demo site can be found at [https://eleventy-l10n-demo.netlify.app](https://eleventy-l10n-demo.netlify.app/), with English (default), Japanese and Spanish language pages (`/` and `/about/`).

## Install

```
npm install
```

## Run locally

Attempted to leverage Netlify CLI to run site locally, hoping it'd adhere to the `redirects` defined in `netlify.toml`.

```
npm i -g netlify-cli
netlify dev
```

But thinking Eleventy's Browsersync setup gets in the way here?

Instead if we're in Apache land and want to leverge the site's `.htaccess` redirect rules, perhaps we'd want to run the site (`npm start`) and then run MAMP (or similar) locally, pointing to output `_site` directory?

## Spoofing Language

[Quick Accept-Language Switcher](https://addons.mozilla.org/en-GB/firefox/addon/quick-accept-language-switc/) makes it super simple to alter `Accept-Language` value, to confirm user language settings are honoured.
