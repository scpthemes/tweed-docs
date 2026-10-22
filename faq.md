---
layout: default
title: FAQ
permalink: /faq/
---

# Frequently asked questions

Answers to the questions merchants ask most about Tweed. The [guide](../) explains the setup step by
step and the [settings reference](../reference/) lists every setting. If your question is not here,
[contact support](../support/).

## Sizes and fit

### The size ladder does not show on my product page

The size ladder reads the product option that holds sizes. Open Theme settings > Fit and check that
**Size option name** matches your option exactly, for example `Size` or `Taille`. Products without
that option show the usual variant picker instead, and the theme editor shows a note on those
products.

### The size ladder shows sizes but no measurements

Measurements come from a size chart entry linked to the product. Create the size chart definitions
(see [Size charts](../#3-size-charts)), add an entry with one row per size, and pick that entry in the
product's **Size chart** metafield. The value in the row's Size field must match the size option
value, for example `M` and `M`.

### Shoppers can switch between inches and centimeters. Do I need two charts?

No. Enter each chart in one unit and set its Unit field to `in` or `cm`. The theme converts every
value on the page when a shopper switches, and remembers the choice on their next visit. Theme
settings > Fit > **Default unit** decides what shoppers see first.

### The body shape links do not filter the collection

Body shape filtering uses a product metafield filter, which you turn on once in the free Search and
Discovery app: Filters > Add filter > the body shape metafield. Until then the links open the
collection without filtering. See [Filters](../#5-filters).

### Do I have to enter fit data product by product?

No. Create the metafield definitions, then fill body shapes, fit notes and Shown on lines in a
spreadsheet and import it: export your products, or start from the theme's product template. See
[Fill fit data in a spreadsheet](../#fill-fit-data-in-a-spreadsheet).

### Can I use the fit features for cats or other pets?

Yes. Size charts, body shapes and fit notes are plain product data. Leave a body shape empty when it
does not apply; the theme hides what is missing.

## Home page and sections

### The Testimonials section is not visible after installing

It ships hidden, because it should only show notes you received from real customers. In the theme
editor, select the section in the sidebar, show it with the eye icon, and replace the example
blocks with your customers' words.

### Why does the slideshow not change slides on its own?

Slides that move on their own are hard to read and to use with a keyboard or a screen reader
(WCAG 2.2.2). Shoppers change slides with the arrows and dots.

### Can I put a video at the top of my home page?

Yes. Add the **Video banner** section and move it to the top. Upload a short clip (10 to 30
seconds) to Shopify; the theme plays a version of at most 720 pixels on the short side, waits until
the page has loaded and starts it only when the section is on screen. A **Cover image** shows first
and stays for shoppers whose device asks for reduced motion. Set **Heading level** to Page heading
(h1) when it is the first section. A video adds weight to the page, so use one clip, not several.

### How do I change the links in the customer account menu?

The account button uses Shopify's customer account menu. Edit its links in Online Store >
Navigation > Customer account main menu.

## Products, cart and checkout

### How do I show unit prices?

Add a unit price to the variant in the product admin (Products > the product > the variant > Unit
price). Product pages, cards and the cart show it automatically.

### How do I offer subscriptions?

Install a subscription app such as Shopify Subscriptions and create selling plans. The product
page, the Restock list section and the cart then show the purchase options. Tweed itself does not
create subscriptions.

### Where is the free shipping progress bar?

Theme settings > Cart > **Show free shipping progress**. Enter the same amount as your free
shipping rate in Settings > Shipping and delivery; the theme does not read your shipping rates.

### How do I show pickup availability?

Turn on local pickup for a location in Settings > Shipping and delivery. Products stocked at that
location then show the **Pickup availability** block's message on the product page.

## Languages and markets

### Which languages does the theme include?

The storefront text and the theme editor are translated into English, French, German, Italian and
Spanish (Latin American forms, as in Shopify's own Spanish). Shopify picks the file that matches the store or market language. Edit any wording in
Online Store > Themes > Edit default theme content.

### How do shoppers change country or language?

Add markets with their own currency or language in Settings > Markets. The header and footer show
the country and language selectors when there is more than one choice; turn them on or off in the
Header and Footer sections.

## Updates and code

### Do I need any apps?

No. Every feature in the demo store is part of the theme. Search and Discovery is Shopify's own
free app for configuring filters and works with every theme.

### How do I update Tweed?

Shopify shows an update in your theme library when a new version is released. The update creates a
new copy of the theme with your settings; check it in preview before publishing.

### Can I edit the theme code?

Yes, but duplicate the theme first (Online Store > Themes > the three dots > Duplicate) and edit
the copy. Code changes are not carried over by theme updates, and support covers the theme as it
was shipped.
