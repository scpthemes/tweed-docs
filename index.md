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

- [Setup order](#setup-order)
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

## Setup order

Each step uses what the step before it created, so this order saves going back:

1. Set the basics in the theme editor ([section 2](#2-first-steps-after-installing)).
2. Create the metafield and metaobject definitions ([section 3](#3-size-charts) and
   [section 4](#4-body-shapes-and-fit-notes)). Do it before you import or export products: a
   product export only has a column for a metafield whose definition exists.
3. Add your products, or fill the fit fields of the products you have, from a spreadsheet
   ([Fill fit data in a spreadsheet](#fill-fit-data-in-a-spreadsheet)).
4. Create your size charts and pick one on each product ([section 3](#3-size-charts)).
5. Create collections from product tags ([section 9](#9-collection-pages)).
6. Add filters in Search and Discovery ([section 5](#5-filters)).
7. Build the menus ([section 6](#6-navigation)) and the pages
   ([section 11](#11-pages-and-templates)).

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
   them. A product tab that points to a page shows the page instead of its text, and a tab with no
   text and no page is hidden from shoppers.

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
| Waist (optional) | `waist` | Single line text |
| Front leg length (optional) | `front_leg_length` | Single line text |
| Paw width (optional) | `paw_width` | Single line text |
| Weight | `weight` | Single line text |
| Breeds | `breeds` | Single line text |

Every field except Size can stay empty. A column shows only when at least one row of the chart
has a value for it, so the three optional fields stay out of sight until you use them: **Waist**
for overalls, snowsuits, onesies, recovery suits and 3-point harnesses, **Front leg length** for
pieces with legs, **Paw width** for boots and paw socks.

**Definition: Size chart** (type `size_chart`)

| Field name | Key | Type |
|---|---|---|
| Title | `title` | Single line text |
| Unit | `unit` | Single line text, with the choices `in` and `cm` |
| Weight unit | `weight_unit` | Single line text, with the choices `lb` and `kg` |
| Size is decided by (optional) | `primary_measurement` | Single line text, with the choices `chest`, `back_length`, `neck` and `paw_width` |
| Note | `note` | Multi-line text |
| Rows | `rows` | Metaobject, list of entries, referencing Size chart row |

**Size is decided by** tells shoppers which measurement to match. Brands differ here: many coats
and harnesses are sized by chest, rain and dry coats often by back length, collars by neck, boots
by paw width. The theme marks that column "Picks the size" in the size chart, lists it first on
the size ladder and says so in the How to measure drawer. Left empty, it is the chest (or the first
of back length, neck and paw width that the chart has).

Then add the product metafield in **Settings > Custom data > Products > Add definition**:
name **Size chart**, namespace and key `custom.size_chart`, type **Metaobject**, referencing Size
chart. To show a chart in a collection's promo tile, add the same definition under **Collections**.

**Filling a chart**

- Write ranges with a hyphen and numbers only: `17-21`, not `17 to 21 in`. The theme adds the unit
  and converts between inches and centimeters for shoppers.
- The **Size** value of a row must match the size option value of the products, for example `M`.
- Measurements describe the dog, not the garment. The theme tells shoppers so. If you copy a
  supplier's table, check that it lists dog measurements and not the garment laid flat.
- Back length runs from the base of the neck to the base of the tail. Some brands start at the
  shoulders, which gives a few centimeters less; if your table does, say so in the chart's Note.
- Converted centimeters are whole numbers, except below 10 cm and for paw width, where they keep
  one decimal (so 1.5 and 1.75 in show as 3.8 and 4.4 cm).

**How shoppers should measure** (the theme shows the measurements the product's chart uses in the
How to measure drawer; neck, chest and back length when the product has no chart):

- **Neck**: around the base of the neck, where a collar sits. Leave one finger of room.
- **Chest**: around the widest part of the ribcage, behind the front legs.
- **Back length**: from the base of the neck, where the collar sits, along the spine to the base of
  the tail.
- **Waist**: around the narrowest part of the belly, just in front of the hind legs, with the dog
  standing.
- **Front leg length**: with the dog standing, from the elbow, where the front leg meets the chest,
  down the back of the leg to just above the paw.
- **Paw width**: stand the dog on a sheet of paper, mark both sides of the paw at its widest point
  and measure between the marks. Hind paws are often smaller, so measure them too.

The step for the measurement that decides the size ends with "This measurement picks the size."

Where charts show up: the **Size ladder** block on the product page lists up to four measurements
per size (the deciding one first; phones show two), the **Size chart** section shows the full
table on product pages, a product photo whose alt text contains `#fit` gets a caption with the
selected size's measurements, and garment cards show the chest range when a shopper points at a
size. For a page with several charts that do not belong to one
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

### Fill fit data in a spreadsheet

With a large catalog, fill body shapes, fit notes and Shown on lines in a spreadsheet instead of
opening each product.

- **Products you already have**: create the definitions above first, then export your products
  in **Products > Export**. Once a definition exists, the export has a column for it, for example
  `Body shape (product.metafields.custom.body_shape)`. Fill those columns, then import the file in
  **Products > Import** with **Overwrite products with matching handles** selected. Change only the
  fit columns: when overwriting, an empty cell clears that value in your store, while a column you
  remove from the file leaves the value as it is.
- **New products**: start from the [product template](assets/tweed-product-template.csv). It holds
  two examples, saved as drafts so shoppers never see them: a rain coat with Color and Size options
  and a harness with sizes only. Every variant is one row; the product's details and fit fields go
  on its first row. Replace the examples with your products and import the file.

In both cases:

- **Body shape** takes `standard`, `deep-chest`, `long-body` or `broad-chest`, spelled exactly
  like that.
- **Product Category** takes a Shopify category ID (`ap-2-6-10` is Pet Rain Coats, `ap-2-17` is
  Pet Collars & Harnesses) or the full English category path. IDs also work when your admin is in
  another language.
- **Tags** fill your collections ([section 9](#9-collection-pages)), for example
  `dogs, rainwear`.
- **Variant Image** takes a public image URL, such as a file uploaded in **Content > Files**. Give
  each color its photo there and the theme shows that photo as the color's swatch
  ([section 8](#8-product-pages)).
- Pick size charts on the product pages ([section 3](#3-size-charts)).

## 5. Filters

Collection and search pages use Shopify's own filtering. Configure it in the free **Search and
Discovery** app by Shopify: **Filters > Add filter**. Recommended filters: Availability, Price,
Product type, Size (the size option), Color, Animal type, and the **Body shape** metafield.

**Animal type** lets shoppers narrow by species. Shopify's categories for pet apparel, collars and
harnesses, leashes and bowls have this standard field, with values such as Dogs, Cats, Rabbits and
Guinea pigs. Shopify creates it when you give a product its category, so there is no definition to
add: set it in the product's **Category metafields** section. Food and treat categories are already
split by species (Dog Food, Cat Food), so the **Category** filter covers them.

**Color**: when the Color option is linked to color entries ([section 8](#8-product-pages)), the
filter can show the colors as swatches. Open the filter in Search and Discovery, click **Manage
values** and select **Include swatch**.

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
- **Color swatches**: the variant picker and the product cards show an option named Color as
  swatches. Each swatch uses the color's entry when the option is linked to one, otherwise the
  photo of that color's variant, otherwise the color name. To link it, give the product a category
  with a Color field (pet apparel, collars and harnesses and leashes have one), click the Color
  option in **Variants**, click the dynamic source icon and pick the category's **Color**
  metafield. Set the color or pattern image of an entry once, in the product's **Category
  metafields** section; every product linked to that entry follows.
- **Size chart** and **Related products** sections can be added below the product information.
- **Complementary products** come from the Search and Discovery app's product recommendations.

## 9. Collection pages

The **Collection banner** shows the collection title, description and image. The **Product grid**
has products per page, products per row, a load more button or page numbers, filtering (section 5),
sorting and an optional **Promo tile** block that sits in the grid on the first page.

### Creating collections

Collections that fill themselves from product tags are the easiest to keep up:

1. Tag your products, for example `dogs`, `coats` or `harnesses`, in the `Tags` column of the
   product CSV or on the product page.
2. In **Products > Collections**, create a collection and add a condition: product tag is equal to
   `coats`. Products that match join the collection, and a product with several tags sits in
   several collections.

The product CSV also has a `Collection` column that creates a collection during the import, but it
puts each product in one collection only.

A structure that suits a pet apparel catalog: one collection per species (Dogs, Cats), per
department (Apparel, Walk, Supplies) and per product family (Coats, Rainwear, Knitwear, Harnesses,
Leashes, Collars, Food, Treats, Beds), plus New arrivals and Sale. Pick them in the home page
sections and link them from the main menu.

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
Spanish (Latin American forms, as in Shopify's own Spanish). Change any wording in **Online Store > Themes > the three dots > Edit default theme
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
