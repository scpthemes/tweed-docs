---
layout: default
title: Guide
permalink: /
---

# Tweed theme guide

Tweed is a Shopify theme for pet apparel stores with large catalogs. Next to species and
department, shoppers browse by fit: size and body shape. This guide sets the theme up from a fresh
install. Every setting is listed with its exact label in the [settings reference](reference/), and
common questions are answered in the [FAQ](faq/).

- [1. Before you start](#1-before-you-start)
- [2. First steps after installing](#2-first-steps-after-installing)
- [3. Size charts](#3-size-charts)
- [4. Body shapes and fit notes](#4-body-shapes-and-fit-notes)
- [5. Filters](#5-filters)
- [6. Navigation](#6-navigation)
- [7. Home page](#7-home-page)
- [8. Product pages](#8-product-pages)
- [9. Collection pages](#9-collection-pages)
- [10. Cart](#10-cart)
- [11. Pages and templates](#11-pages-and-templates)
- [12. Languages and markets](#12-languages-and-markets)
- [13. Speed and accessibility](#13-speed-and-accessibility)
- [14. Support and updates](#14-support-and-updates)

## 1. Before you start

Tweed works with standard Shopify data and needs no apps. To use its fit features you need:

- A product option that holds sizes, usually named **Size**. Write the values the same way on every
  product (for example XS, S, M, L, XL, XXL).
- Optional: size chart entries (section 3) and a body shape for each product (section 4). Without
  them the theme still works and hides what is missing.

## 2. First steps after installing

1. Open **Online Store > Themes**, find Tweed and click **Customize**.
2. **Theme settings > Logo and favicon**: upload your logo and a 32 x 32px favicon.
3. **Theme settings > Colors**: Tweed has four color schemes. Sections pick a scheme; change the
   colors of a scheme once and every section that uses it follows.
4. **Theme settings > Typography**: pick a heading font and a body font from the Shopify font
   library.
5. **Theme settings > Fit**: check **Size option name** (default `Size`), choose the **Default
   unit** (inches or centimeters) and pick the **Measuring guide page** (section 11). The metafield
   keys under **Metafields** only change if you use other keys than the defaults in section 3 and 4.
6. Replace the instructional text in the announcement bar, the cart and the product tabs with your
   own wording. Those defaults explain what to write; they are visible to shoppers until you edit
   them.

## 3. Size charts

A size chart is a list of rows, one per size, with the dog's measurements. Products point to a
chart, so one chart can serve many products. Create the two definitions once in **Settings >
Custom data > Metaobjects > Add definition**.

**Definition: Size chart row** (type `size_chart_row`)

| Field name | Key | Type |
|---|---|---|
| Size | `size` | Single line text |
| Neck | `neck` | Single line text |
| Chest | `chest` | Single line text |
| Back length | `back_length` | Single line text |
| Weight | `weight` | Single line text |
| Breeds | `breeds` | Single line text |

**Definition: Size chart** (type `size_chart`)

| Field name | Key | Type |
|---|---|---|
| Title | `title` | Single line text |
| Unit | `unit` | Single line text, with the choices `in` and `cm` |
| Weight unit | `weight_unit` | Single line text, with the choices `lb` and `kg` |
| Note | `note` | Multi-line text |
| Rows | `rows` | Metaobject, list of entries, referencing Size chart row |

Then add the product metafield in **Settings > Custom data > Products > Add definition**:
name **Size chart**, namespace and key `custom.size_chart`, type **Metaobject**, referencing Size
chart. To show a chart in a collection's promo tile, add the same definition under **Collections**.

**Filling a chart**

- Write ranges with a hyphen and numbers only: `17-21`, not `17 to 21 in`. The theme adds the unit
  and converts between inches and centimeters for shoppers.
- The **Size** value of a row must match the size option value of the products, for example `M`.
- Measurements describe the dog, not the garment. The theme tells shoppers so.

**How shoppers should measure** (the theme shows this in the How to measure drawer):

- **Neck**: around the base of the neck, where a collar sits. Leave one finger of room.
- **Chest**: around the widest part of the ribcage, just behind the front legs. This decides the
  size.
- **Back length**: from the base of the neck to the base of the tail.

Where charts show up: the **Size ladder** block on the product page lists the measurements per size,
the **Size chart** section shows the full table on product pages, and garment cards show the chest
range when a shopper points at a size. For a page with several charts that do not belong to one
product (for example one per body shape), use the **Size charts** section and type the rows into
its blocks.

## 4. Body shapes and fit notes

Body shape links let shoppers find cuts for deep-chested, long or broad dogs. Add these product
metafields in **Settings > Custom data > Products > Add definition**:

| Name | Namespace and key | Type | Used for |
|---|---|---|---|
| Body shape | `custom.body_shape` | Single line text, choices `standard`, `deep-chest`, `long-body`, `broad-chest` | Fit rail, fit finder, Shop by fit menu column, collection fit bar |
| Fit note | `custom.fit_note` | Single line text | A short line on product cards, such as "Runs small, size up" |
| Shown on | `custom.shown_on` | Multi-line text | The Fit note block on the product page, such as "Shown on Juno, whippet, 13 kg, size M" |

## 5. Filters

Collection and search pages use Shopify's own filtering. Configure it in the free **Search and
Discovery** app by Shopify: **Filters > Add filter**. Recommended filters: Availability, Price,
Product type, Size (the size option), Color, and the **Body shape** metafield.

The body shape links of the fit rail, the fit finder and the Shop by fit column open a collection
filtered by the Body shape metafield. They filter once that metafield is added as a filter; before
that they open the collection unfiltered.

In the theme editor, the **Product grid** section (collection template) has **Enable filtering**,
**Filter layout** (sidebar or drawer) and **Show fit bar**, which moves the size and body shape
filters into a bar above the grid.

## 6. Navigation

- **Main menu**: Online Store > Navigation > Main menu. A top-level item with child links opens a
  panel on large screens and a drawer on phones; each panel starts with a "Shop all" link to the
  item itself.
- **Shop by fit column**: in the Header section, add a **Shop by fit** block and type the name of a
  top-level menu item in **Main menu item** (for example Dogs). The column shows size links and
  body shape links in that item's panel.
- **Featured link**: a Header block that adds an image link to a panel.
- **Footer menus**: add **Footer menu** blocks to the Footer section and pick a menu for each.
- **Customer account menu**: the account button uses Shopify's Customer account main menu (Online
  Store > Navigation).
- **Fit rail**: a bar under the header with size and body shape links. Add it in the header group;
  it stays hidden on collection and cart pages, where the fit bar takes over.

## 7. Home page

The home page ships with these sections, in this order: Featured look, Fit finder, Featured
collection, Collection list, Fit guide, Image with text, Restock list, Testimonials (hidden until
you add real customer notes), Logo list and Blog posts. Add, remove and reorder them in the theme
editor. Other sections you can add: Slideshow, Video, Video banner, Rich text, Image gallery, Map,
Newsletter, Size charts, Contact form, Custom Liquid and Apps.

Notes on a few of them:

- **Featured look**: a product photo with numbered hotspots. Add a **Hotspot** block per product and
  place it with the position sliders; every hotspot has a matching row in the parts list.
- **Fit finder**: size blocks (size, chest range, example breed) and body shape blocks. The example
  values that ship with the theme are typical ranges; replace them with your own chart.
- **Fit guide**: a diagram with **Measuring point** blocks placed on it.
- **Restock list**: rows for food and supplies with unit prices and quantities.
- **Slideshow**: slides change only when shoppers use the arrows or dots.
- **Video banner**: a short muted clip on a loop with a pause button. It loads after the page and
  stays still for shoppers who ask for reduced motion. Use one per page and pick a cover image.

## 8. Product pages

The **Product information** section is built from blocks you can reorder: Vendor, Heading, Price,
Text, Description, Variant picker, Size ladder, Fit note, Quantity selector, Purchase options, Buy
buttons, Pickup availability, Complementary products, Collapsible tab, Share, Custom Liquid and app
blocks.

- **Size ladder**: one button per size with the chart measurements, a How to measure drawer and a
  link to the full chart. It needs the size option (section 1) and shows measurements when the
  product has a size chart (section 3).
- **Media**: product photos, videos and 3D models. Choose a stacked or thumbnail layout and turn
  zoom on or off in the section settings.
- **Size chart** and **Related products** sections can be added below the product information.
- **Complementary products** come from the Search and Discovery app's product recommendations.

## 9. Collection pages

The **Collection banner** shows the collection title, description and image. The **Product grid**
has products per page, products per row, a load more button or page numbers, filtering (section 5),
sorting and an optional **Promo tile** block that sits in the grid on the first page.

## 10. Cart

**Theme settings > Cart** sets the cart type: a popup notification after adding to cart, or the cart
page. Turn on **Show free shipping progress** and enter your free shipping amount to show the
progress bar. In the cart template, the **Cart summary** section takes **Assurance line** blocks for
short service promises such as free exchanges.

## 11. Pages and templates

- **Fit guide page**: create a page (Online Store > Pages), choose the template `page.fit-guide`
  and select the page in Theme settings > Fit > **Measuring guide page**. Every How to measure and
  fit guide link in the theme leads there. The template holds the page content, the Fit guide
  diagram, a Video, Size charts and Rich text.
- **Contact page**: create a page with the template `page.contact`.
- **Policies**: Settings > Policies. The footer can link to them through a footer menu.

## 12. Languages and markets

The storefront text and the theme editor are translated into English, French, German, Italian and
Spanish. Change any wording in **Online Store > Themes > the three dots > Edit default theme
content**. Add countries in Settings > Markets and languages in Settings > Languages; the country
and language selectors in the header and footer appear when there is more than one choice.
Right-to-left languages are supported.

## 13. Speed and accessibility

- Upload photos at least 1800 pixels wide; Shopify serves smaller copies to small screens.
- The first image of the page loads first; everything below loads as shoppers scroll.
- Keep to one Video banner per page and use short clips.
- The theme supports keyboard navigation, screen readers, reduced motion and visible focus. When you
  change colors, keep text readable: dark text on light backgrounds or the reverse.
- Give every product image alt text in the product admin.

## 14. Support and updates

- [Contact support](support/) for questions about the theme's features and settings and for bugs.
  We answer within two business days.
- Bugs that stop customers from buying are fixed right away and released as an update.
- Support does not cover custom code, third-party apps or design changes.
- Updates appear in your theme library. Release notes list what changed in each version.
