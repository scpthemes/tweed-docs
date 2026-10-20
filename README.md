# Tweed documentation site

Source of the public Tweed theme documentation and support page, published
with GitHub Pages (Jekyll, no local build needed).

- `index.md`: setup guide
- `reference.md`: settings reference, generated from the theme schemas with
  `node tools/gen-docs.mjs` in the theme repository. Do not edit by hand.
- `faq.md`: frequently asked questions
- `support.md`: support policy and the link to the support form (support-shopify.scpthemes.com)
- `_config.yml`: site settings; `support_form_url` holds the form link

Publish: put these files at the root of a public repository, then
Settings > Pages > Build and deployment > Source: Deploy from a branch >
`main` and `/ (root)` > Save.
