---
layout: default
title: Support
permalink: /support/
---

# Tweed support

Ask us about Tweed's features and settings, or report a bug. Before writing, the
[guide](../) and the [FAQ](../faq/) answer the most common questions.

**What to include:** your store URL, the page where you see the problem, what you expected
and what happened, and a screenshot or a short screen recording if you can.

**When we answer:** within two business days. Bugs that stop customers from buying (add to
cart, checkout, a page that does not load) are fixed right away and released as a theme update.

**What support covers:** the theme's built-in features and settings, and bugs in the theme as it
was shipped. Custom code, third-party apps and design changes are not covered.

{% assign form_url = site.support_form_url | strip %}
{% if form_url.size > 0 %}
<iframe
  class="form-frame"
  src="{{ form_url }}"
  title="Tweed support form"
  loading="lazy"
  allow="geolocation 'none'"
></iframe>

If the form does not load, [open the support form in a new tab]({{ form_url }}).
{% else %}
The support form is being set up. Please check back soon.
{% endif %}
