# Eleventy l10n demo

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
