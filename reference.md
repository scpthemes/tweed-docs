---
layout: default
title: Settings reference
permalink: /reference/
---

# Settings reference

Every theme setting, section and block of Tweed, with the labels you see in the theme editor
(Online Store > Themes > Customize). This page is generated from the theme files, so it always
matches the version it was built from.

Theme version: 1.0.0.

- [Theme settings](#theme-settings)
- [Sections](#sections)

## Theme settings

Open them from the theme editor sidebar: Theme settings (the brush icon).

### Logo and favicon

| Setting | Type | Default | Notes |
|---|---|---|---|
| Logo | Image |  | Works with landscape, square and portrait images. Shows the store name when empty. |
| Logo width on large screens | Slider, 60 to 300 px | 140 px |  |
| Logo width on small screens | Slider, 40 to 200 px | 100 px |  |
| Favicon | Image |  | 32 x 32px .png recommended |

### Colors

**Color schemes**

> Sections and blocks pick one of these schemes. Every background color has its own text color, so contrast stays readable wherever a section uses the scheme.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Color schemes | Colors per scheme: Background, Background gradient, Text, Secondary text, Panel background, Borders, Button background, Button label, Button background on hover, Secondary button label, Sale price, Success messages, Error messages |  |  |

**Accent**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Accent background | Color |  | Colors the new badge, the cart count and the fit highlights. |
| Accent text | Color |  |  |

**Badges**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Sale badge background | Color |  |  |
| Sale badge text | Color |  |  |

### Typography

**Headings**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Font | Font |  |  |
| Font size scale | Slider, 80 to 130 % | 100 % |  |

**Body text**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Font | Font |  |  |
| Font size scale | Slider, 90 to 120 % | 100 % |  |

### Layout

| Setting | Type | Default | Notes |
|---|---|---|---|
| Page width | Slider, 1200 to 1600 px | 1440 px |  |
| Extra space between sections | Slider, 0 to 100 px | 0 px |  |

### Buttons, inputs and media

| Setting | Type | Default | Notes |
|---|---|---|---|
| Button corner radius | Slider, 0 to 24 px | 2 px |  |
| Input corner radius | Slider, 0 to 24 px | 2 px |  |
| Image corner radius | Slider, 0 to 24 px | 0 px |  |
| Product image shape | Choice: Original, Portrait 4:5, Square 1:1 | Portrait 4:5 |  |

### Product cards

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show vendor | On or off | On |  |
| Show color swatches | On or off | On |  |
| Show fit note | On or off | On | Reads the fit note metafield set under Fit. Pointing at a size shows its chest range. |
| Show body shape label | On or off | On |  |
| Show size ladder | On or off | On | Lists every value of the size option on the card. Sold out sizes stay visible and struck through. |
| Show sizes as add to cart buttons | On or off | On |  |
| Swap to the second image on hover | On or off | Off |  |

### Fit

> Tweed reads sizes and body shapes from standard Shopify product data. The theme documentation lists the metafield definitions to create.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Size option name | Text | `Size` | The product option that holds sizes, such as Size |
| Default unit | Choice: Inches, Centimeters | Inches |  |
| Measuring guide page | Page |  | Pick a page that uses the fit-guide template. How to measure and fit guide links across the theme lead to it. |

**Metafields**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Size chart metafield | Text | `custom.size_chart` | Product metafield that references a size chart entry, written as namespace.key |
| Body shape metafield | Text | `custom.body_shape` | Product metafield with one of these values: standard, deep-chest, long-body, broad-chest |
| Fit note metafield | Text | `custom.fit_note` |  |

### Cart

| Setting | Type | Default | Notes |
|---|---|---|---|
| Cart type | Choice: Popup notification, Page | Popup notification |  |
| Show free shipping progress | On or off | Off | Match the amount to your rates in Settings > Shipping and delivery. |
| Free shipping amount | Number |  | Order subtotal in your store currency |

### Search suggestions

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show suggestions as customers type | On or off | On |  |
| Show vendor | On or off | Off |  |
| Show price | On or off | On |  |

### Animations

| Setting | Type | Default | Notes |
|---|---|---|---|
| Fade sections in on scroll | On or off | On | Always off for visitors who ask their device for reduced motion. |

### Social media

**Accounts**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Instagram | Text |  | For example, https://instagram.com/yourstore |
| TikTok | Text |  | For example, https://tiktok.com/@yourstore |
| Facebook | Text |  | For example, https://facebook.com/yourstore |
| Pinterest | Text |  | For example, https://pinterest.com/yourstore |
| YouTube | Text |  | For example, https://youtube.com/@yourstore |
| X (Twitter) | Text |  | For example, https://x.com/yourstore |

### Gift card

| Setting | Type | Default | Notes |
|---|---|---|---|
| Image | Image |  | Shows on the gift card page that customers receive. 1200 x 750px recommended |

### Prices

> The cart total and checkout always show currency codes, such as $1.00 USD. Turn this on to show them on every other price too.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show currency codes | On or off | Off |  |

## Sections

Sections marked "Add section" can be added to any template that allows them, from the
theme editor: Add section. The others belong to one template or group.

### Announcement bar

Where: Add section, only in the header group.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show one announcement at a time with arrows | On or off | On | Announcements never rotate on their own. When off, all announcements show side by side. |
| Color scheme | Color scheme | Scheme 3 |  |

#### Block: Announcement

| Setting | Type | Default | Notes |
|---|---|---|---|
| Text | Text with bold, italic and links |  |  |
| Link | Link |  |  |

### Apps

Where: Add section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Match the theme's section spacing | On or off | On |  |

Accepts app blocks.

### Article

Where: part of the Blog posts (article) template.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show links to the blog and the next article | On or off | On |  |

> Comments show when you turn them on for the blog in Online Store > Blog posts > Manage blogs.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 32 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

#### Block: Heading

Up to 1 per section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show breadcrumbs | On or off | On |  |
| Show tags | On or off | On |  |
| Show author | On or off | On |  |
| Show date | On or off | On |  |
| Show reading time | On or off | On |  |

#### Block: Featured image

Up to 1 per section.

> Shows the article's featured image. 2400 x 1600px .jpg recommended

#### Block: Content

Up to 1 per section.

No settings.

#### Block: Products

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text |  |  |
| Products | Products |  |  |

#### Block: Share buttons

Up to 1 per section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show Facebook | On or off | On |  |
| Show X | On or off | On |  |
| Show Pinterest | On or off | On |  |
| Show copy link button | On or off | On |  |

#### Block: Custom Liquid

| Setting | Type | Default | Notes |
|---|---|---|---|
| Custom Liquid | Liquid code |  |  |

Accepts app blocks.

### Blog

Where: part of the Blogs template.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Intro text | Formatted text |  |  |
| Layout | Choice: Large first article, Grid | Large first article |  |
| Articles per page | Slider, 4 to 24 | 7 |  |
| Show load more button | On or off | Off | Page numbers always show below it. |

**Article cards**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show tags | On or off | On | Also adds tag filter links under the heading. |
| Show date | On or off | On |  |
| Show excerpt | On or off | On |  |
| Show author | On or off | On |  |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 32 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

### Blog posts

Where: Add section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text with bold, italic and links |  |  |
| Blog | Blog |  |  |
| Posts to show | Slider, 2 to 4 | 4 |  |
| Show date | On or off | On |  |
| Show first tag | On or off | On |  |
| Link label | Text |  | Links to the blog |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 88 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

### Cart items

Where: part of the Cart template.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show vendor | On or off | Off |  |
| Show order note | On or off | On |  |
| Note hint | Text |  | Short help text under the note label |

> Set the free shipping progress bar in Theme settings > Cart.

**Empty cart**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Text | Formatted text |  |  |
| Button label | Text |  |  |
| Button link | Link |  |  |
| Second button label | Text |  |  |
| Second button link | Link |  |  |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 32 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

#### Block: Custom Liquid

| Setting | Type | Default | Notes |
|---|---|---|---|
| Custom Liquid | Liquid code |  | Add app snippets or other code below the cart items. |

Accepts app blocks.

### Cart summary

Where: part of the Cart template.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show total savings | On or off | On |  |

> Dynamic checkout buttons show when you turn them on in Settings > Payments.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Color scheme | Color scheme | Scheme 2 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 32 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

#### Block: Assurance line

Up to 4 per section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Icon | Choice: Exchange, Truck, Map pin, Package, Lock, Gift, Clock, Ruler | Exchange |  |
| Text | Text |  |  |

### Collection banner

Where: part of the Collections (collection) template.

> Edit the collection title, description and image under Products > Collections.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show breadcrumbs | On or off | On |  |
| Show product count | On or off | On |  |
| Show description | On or off | On |  |
| Show image | On or off | On |  |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 32 px |  |
| Bottom padding | Slider, 0 to 160 px | 24 px |  |

### Collection list

Where: Add section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text with bold, italic and links |  |  |
| Body text | Formatted text |  |  |
| Link label | Text |  |  |
| Link | Link |  | Defaults to the collections list page |
| Show product count | On or off | On |  |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 88 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

#### Block: Collection

| Setting | Type | Default | Notes |
|---|---|---|---|
| Collection | Collection |  |  |
| Label | Text |  | Defaults to the collection title |

### Collection list page

Where: part of the Collections list template.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text | `Collections` |  |
| Text | Formatted text |  |  |
| Show breadcrumbs | On or off | On |  |

**Groups**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Group by navigation | Menu |  | Top-level links become group headings and their nested collection links fill each group. Leave empty to list every collection, with pagination. |
| Show links to each group | On or off | On |  |
| Large first card | Choice: None, First group, Every group | First group | Shows on desktop. Without groups, the first collection on the first page is large. |

**Collection cards**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show product count | On or off | On |  |
| Collections per page | Slider, 8 to 48 | 24 | Applies when the page lists every collection. |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 32 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

### Contact form

Where: Add section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text |  | Leave blank to show the page title. |
| Text | Formatted text |  |  |
| Show page content | On or off | On | Shows the text from Online Store > Pages under the heading. |
| Show breadcrumbs | On or off | On |  |
| Image | Image |  | 1600 x 1000px .jpg recommended |

**Store information**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show store information | On or off | On |  |
| Address | Text, several lines |  |  |
| Opening hours | Text |  |  |
| Phone number | Text |  |  |
| Email address | Text |  |  |

**Form**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Form heading | Text |  |  |
| Show phone field | On or off | On |  |
| Topics | Text |  | Separate topics with commas. Leave blank to hide the topic field. |
| Show measurement fields | On or off | On | Neck, chest and back length, in the unit set in Theme settings > Fit. |
| Success message | Text |  | Leave blank for the default message. |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 32 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

### Custom Liquid

Where: Add section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Liquid code | Liquid code |  | Paste app snippets or your own Liquid code. |
| Full page width | On or off | Off |  |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 40 px |  |
| Bottom padding | Slider, 0 to 160 px | 40 px |  |

### Featured collection

Where: Add section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text with bold, italic and links |  |  |
| Body text | Formatted text |  |  |
| Collection | Collection |  |  |
| Products to show | Slider, 4 to 12 | 8 |  |
| Columns on large screens | Choice: Three, Four | Four |  |
| Show link to the collection | On or off | On |  |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 88 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

#### Block: Editorial tile

Up to 1 per section.

> Takes two columns and two rows at the start of the grid.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Image | Image |  | 1200 x 1500px .jpg recommended |
| Heading | Text |  |  |
| Body text | Text |  |  |
| Link | Link |  |  |

### Featured look

Where: Add section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Image | Image |  | The section never crops this image, so hotspots stay where you place them. 1600 x 1280px .jpg recommended |
| Image position | Choice: Left, Right | Left | With Right, the text comes before the image on small screens |

**Text**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Subheading | Text |  |  |
| Heading | Text with bold, italic and links |  |  |
| Heading level | Choice: Page heading (h1), Section heading (h2) | Page heading (h1) | Use Page heading (h1) when this is the first section of the home page |
| Heading size | Choice: Extra large, Large | Extra large |  |
| Body text | Formatted text |  |  |
| Button label | Text |  |  |
| Button link | Link |  | Defaults to all products |
| Secondary link label | Text |  |  |
| Secondary link | Link |  | Defaults to the measuring guide page set in theme settings under Fit |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 24 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

#### Block: Hotspot

| Setting | Type | Default | Notes |
|---|---|---|---|
| Product | Product |  |  |
| Horizontal position | Slider, 0 to 100 % | 50 % |  |
| Vertical position | Slider, 0 to 100 % | 50 % |  |

### Featured product

Where: Add section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Product | Product |  |  |
| Desktop media position | Choice: Left, Right | Left | With Right, the product details come before the media on small screens |
| Loop videos | On or off | Off |  |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 88 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

#### Block: Text

| Setting | Type | Default | Notes |
|---|---|---|---|
| Text | Formatted text |  |  |
| Text style | Choice: Body, Subdued, Caption | Body |  |

#### Block: Heading

Up to 1 per section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading size | Choice: Small, Medium, Large | Medium |  |

#### Block: Price

Up to 1 per section.

No settings.

#### Block: Variant picker

Up to 1 per section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Style | Choice: Swatches and buttons, Buttons, Dropdown | Swatches and buttons |  |

#### Block: Purchase options

Up to 1 per section.

> Shows subscription options for products with selling plans.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text |  |  |
| Note | Text |  |  |

#### Block: Quantity selector

Up to 1 per section.

No settings.

#### Block: Buy buttons

Up to 1 per section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show dynamic checkout buttons | On or off | On | Shows the shopper's preferred express payment method, such as PayPal or Apple Pay, from the ones your store offers. |
| Let gift card buyers add a recipient | On or off | On |  |

#### Block: Custom Liquid

| Setting | Type | Default | Notes |
|---|---|---|---|
| Liquid | Liquid code |  | Paste app snippets or your own Liquid code. |

Accepts app blocks.

### Fit finder

Where: Add section.

> Links to a collection filtered by size or body shape. Body shape links need the body shape metafield added as a filter in the Search and Discovery app.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text with bold, italic and links |  |  |
| Body text | Formatted text |  |  |
| Link label | Text |  |  |
| Link | Link |  | Defaults to the measuring guide page set in theme settings under Fit |
| Collection to filter | Collection |  | Defaults to all products |

**Sizes**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text |  |  |
| Unit of the chest ranges | Choice: Inches, Centimeters | Inches | Shoppers can switch between inches and centimeters on size charts; these ranges follow their choice |

**Body shapes**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text |  |  |
| Show example breeds | On or off | On |  |
| Color scheme | Color scheme | Scheme 4 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 88 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

#### Block: Size

Up to 8 per section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Size | Text | `M` | A value of the size option, written exactly as on your products |
| Chest range | Text | `17-21` | Numbers only, such as 17-21 |
| Example breed | Text |  |  |

#### Block: Body shape

Up to 4 per section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Body shape | Choice: Standard, Deep chest, Long body, Broad chest | Standard | Must match the body shape metafield values of your products |
| Label | Text |  | Defaults to the body shape name |
| Example breeds | Text |  |  |
| Extra line | Text |  | Optional, such as the number of pieces cut for this shape |

### Fit guide

Where: Add section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Diagram | Image |  | A drawing with room around the measuring points. 1500 x 1000px .png recommended |
| Heading | Text with bold, italic and links |  |  |
| Note | Formatted text |  |  |
| Button label | Text |  |  |
| Button link | Link |  | Defaults to the measuring guide page set in theme settings under Fit |
| Color scheme | Color scheme | Scheme 2 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 88 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

#### Block: Measuring point

| Setting | Type | Default | Notes |
|---|---|---|---|
| Label | Text | `Chest` |  |
| Body text | Formatted text |  |  |
| Horizontal position | Slider, 0 to 100 % | 50 % |  |
| Vertical position | Slider, 0 to 100 % | 50 % |  |

### Fit rail

Where: Add section, only in the header group.

> Links to a collection filtered by size or body shape. Stays hidden on collection and cart pages.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text |  |  |
| Collection to filter | Collection |  | Defaults to all products |
| Guide link label | Text |  |  |
| Guide link | Link |  | Defaults to the measuring guide page set in theme settings under Fit |
| Color scheme | Color scheme | Scheme 1 |  |

#### Block: Size

| Setting | Type | Default | Notes |
|---|---|---|---|
| Size | Text | `M` | A value of the size option, written exactly as on your products |

#### Block: Body shape

| Setting | Type | Default | Notes |
|---|---|---|---|
| Body shape | Choice: Standard, Deep chest, Long body, Broad chest | Deep chest |  |
| Label | Text |  |  |

### Footer

Where: Add section, only in the footer group.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show tape measure edge | On or off | On |  |

**Bottom bar**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show social media icons | On or off | On | Add account links in theme settings under Social media. |
| Show Follow on Shop | On or off | On | Customers can follow the store in the Shop app. Requires Shop Pay. |
| Show payment icons | On or off | On |  |
| Show policy links | On or off | On | Add policies in Settings > Policies. |
| Show Powered by Shopify | On or off | On |  |

**Country and language**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show country selector | On or off | On |  |
| Show language selector | On or off | On |  |

**Colors**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Color scheme | Color scheme | Scheme 3 |  |

#### Block: Email signup

Up to 1 per section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text with bold, italic and links |  |  |
| Text | Formatted text |  |  |
| Button label | Text | `Subscribe` |  |

> Shopify adds subscribers to your customer list with the tag newsletter.

#### Block: Footer menu

Up to 4 per section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text with bold, italic and links |  |  |
| Footer menu | Menu | footer |  |

#### Block: Store information

Up to 2 per section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text with bold, italic and links |  |  |
| Address | Text with bold, italic and links |  |  |
| Phone number | Text |  |  |
| Email | Text |  |  |
| Opening hours | Text with bold, italic and links |  |  |

#### Block: Text

Up to 2 per section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text with bold, italic and links |  |  |
| Text | Formatted text |  |  |

### Header

Where: only in the header group.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Main menu | Menu | main-menu | Top-level items with children open a panel. Add a Shop by fit or Featured link block to fill it. |
| Sticky header | Choice: Always, When scrolling up, Never | Always |  |

**Search**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show search field on large screens | On or off | On | Smaller screens show a search icon that opens the search drawer. |
| Search field placeholder | Text | `Search` |  |

**Country and language**

> Add countries in Settings > Markets and languages in Settings > Languages.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show country selector | On or off | On |  |
| Show language selector | On or off | On |  |

**Colors**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Color scheme | Color scheme | Scheme 1 |  |
| Navigation color scheme | Color scheme | Scheme 1 | Colors the dropdown panels and the mobile drawer. |

#### Block: Shop by fit

Up to 3 per section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Main menu item | Text | `Dogs` | Enter the name of a top-level item, such as Dogs. The column shows in its panel. |
| Heading | Text |  |  |
| Collection to filter | Collection |  | Defaults to all products |
| Sizes | Text |  | Values of the size option, separated by commas |
| Show body shapes | On or off | On | Links filter by the body shape metafield set in theme settings under Fit. |
| Deep chest examples | Text |  |  |
| Long body examples | Text |  |  |
| Broad chest examples | Text |  |  |

#### Block: Featured link

Up to 3 per section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Main menu item | Text | `Dogs` | Enter the name of a top-level item, such as Dogs. The link shows in its panel. |
| Image | Image |  |  |
| Heading | Text |  |  |
| Text | Text |  |  |
| Link | Link |  |  |

### Image gallery

Where: Add section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text with bold, italic and links |  |  |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 88 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

#### Block: Image

| Setting | Type | Default | Notes |
|---|---|---|---|
| Image | Image |  | 1500 x 1200px .jpg recommended |
| Caption | Text |  |  |

### Image with text

Where: Add section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Image | Image |  | 1800 x 1200px .jpg recommended |
| Image position | Choice: Left, Right | Left | With Right, the text comes before the image on small screens |
| Image shape | Choice: Original, Wide 16:9, Landscape 4:3 | Original |  |

**Text**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text with bold, italic and links |  |  |
| Heading size | Choice: Large, Medium | Large |  |
| Body text | Formatted text |  |  |
| Button label | Text |  |  |
| Button link | Link |  | Defaults to all products |
| Color scheme | Color scheme | Scheme 3 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 0 px |  |
| Bottom padding | Slider, 0 to 160 px | 0 px |  |

### Logo list

Where: Add section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text with bold, italic and links |  |  |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 52 px |  |
| Bottom padding | Slider, 0 to 160 px | 52 px |  |

#### Block: Logo

| Setting | Type | Default | Notes |
|---|---|---|---|
| Logo | Image |  | A single-color logo on a transparent background. 160 x 160px .png recommended |
| Name | Text |  | Shows beside the logo |
| Link | Link |  |  |

### Map

Where: Add section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text with bold, italic and links |  |  |
| Address | Formatted text |  |  |
| Opening hours | Text |  |  |

**Directions**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Button label | Text |  | Opens Google Maps with directions to the address. Leave blank to hide the button. |
| Directions address | Text |  | Google Maps looks up this address. Defaults to the address above. |

**Image**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Image | Image |  | A map or a photo of your storefront. 1600 x 900px .png recommended |
| Show pin | On or off | On |  |
| Pin horizontal position | Slider, 0 to 100 % | 50 % |  |
| Pin vertical position | Slider, 0 to 100 % | 50 % |  |
| Color scheme | Color scheme | Scheme 2 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 0 px |  |
| Bottom padding | Slider, 0 to 160 px | 0 px |  |

### Newsletter

Where: Add section.

> Shopify adds subscribers to your customer list with the tag newsletter.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text with bold, italic and links |  |  |
| Body text | Formatted text |  |  |
| Button label | Text | `Subscribe` |  |
| Alignment | Choice: Left, Center | Left |  |
| Color scheme | Color scheme | Scheme 2 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 88 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

### Page

Where: part of the Pages template.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show breadcrumbs | On or off | On |  |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 32 px |  |
| Bottom padding | Slider, 0 to 160 px | 64 px |  |

### Page not found

Where: part of the 404 page template.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text |  | Leave blank to show Page not found. |
| Text | Formatted text |  |  |
| Image | Image |  | 1200 x 1200px .png recommended |
| Show search field | On or off | On |  |
| Show fit guide link | On or off | On | Links to the measuring guide page you pick in Theme settings > Fit. |
| Show home page link | On or off | On |  |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 64 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

#### Block: Link

Up to 4 per section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Label | Text |  |  |
| Link | Link |  |  |

### Password page

Where: part of the Password page template.

> The heading shows the message for visitors from Online Store > Preferences. When that message is blank, the heading below shows.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text |  |  |
| Image | Image |  | 1600 x 1000px .jpg recommended |
| Color scheme | Color scheme | Scheme 1 |  |

#### Block: Text

| Setting | Type | Default | Notes |
|---|---|---|---|
| Text | Formatted text |  |  |

#### Block: Email signup

Up to 1 per section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Button label | Text |  |  |
| Success message | Text |  | Leave blank for the default message. |

#### Block: Social media icons

Up to 1 per section.

> Add social media links in Theme settings > Social media.

### Pickup availability

Where: part of the Products (shown by the Pickup availability block) template.

### Product grid

Where: part of the Collections (collection) template.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Products on each page | Slider, 8 to 48 | 24 |  |
| Products per row on desktop | Slider, 2 to 4 | 4 |  |
| Products per row on mobile | Choice: One, Two | Two |  |
| Let customers change products per row | On or off | On |  |
| Pagination | Choice: Load more button, Page numbers | Load more button | Page numbers stay available below the load more button. |

**Filtering**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Enable filtering | On or off | On | Set up filters in the Search and Discovery app. [Learn more](https://help.shopify.com/manual/online-store/search-and-discovery/filters) |
| Filter layout | Choice: Sidebar, Drawer | Sidebar | Phones always use the drawer. |
| Show fit bar | On or off | On | Moves the size and body shape filters into a sticky bar above the grid. Set the option name and the metafield in theme settings under Fit. |
| Show in stock switch | On or off | On | Replaces the availability filter with one switch. |

**Sorting**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show sorting | On or off | On |  |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 0 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

#### Block: Promo tile

Up to 1 per section.

> Shows on the first page of the grid until a shopper applies a filter.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Position in grid | Slider, 2 to 12 | 7 |  |
| Heading | Text |  |  |
| Text | Formatted text |  |  |
| Show chest by size | On or off | On | Reads the collection's size chart metafield, the same namespace and key as the product size chart in theme settings under Fit. |
| Link label | Text |  |  |
| Link | Link |  | Defaults to the measuring guide page set in theme settings under Fit |
| Image | Image |  | Shows at the bottom of the tile. 900 x 600px .png recommended |
| Color scheme | Color scheme | Scheme 2 |  |

#### Block: Custom Liquid

| Setting | Type | Default | Notes |
|---|---|---|---|
| Liquid code | Liquid code |  | Add app snippets or other Liquid code above the product grid. |

Accepts app blocks.

### Product information

Where: part of the Products template.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show breadcrumbs | On or off | On |  |

**Media**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Desktop layout | Choice: Stacked, Thumbnails | Stacked |  |
| Desktop media size | Choice: Large, Medium | Large |  |
| Let customers zoom images | On or off | On |  |
| Loop videos | On or off | Off |  |

**Layout**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Keep product information in view on desktop | On or off | On |  |
| Show sticky add to cart bar on mobile | On or off | On |  |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 16 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

#### Block: Vendor

Up to 1 per section.

No settings.

#### Block: Heading

Up to 1 per section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading size | Choice: Small, Medium, Large | Medium |  |

#### Block: Price

Up to 1 per section.

> Shows the sale price, compare-at price, unit price, the tax note and the Shop Pay Installments banner when Shop Pay Installments is on.

#### Block: Text

| Setting | Type | Default | Notes |
|---|---|---|---|
| Content | Choice: Text below, Product subtitle | Text below | Product subtitle reads the standard metafield descriptors.subtitle, so each product shows its own summary. |
| Text | Formatted text |  |  |
| Text style | Choice: Body, Subdued, Caption | Body |  |

#### Block: Description

Up to 1 per section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show as a collapsible tab | On or off | Off |  |
| Tab heading | Text | `Description` |  |
| Start expanded | On or off | On |  |

#### Block: Variant picker

Up to 1 per section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Style | Choice: Swatches and buttons, Buttons, Dropdown | Swatches and buttons | Swatches show for options with swatch colors or images, and for options named Color. Other options show as buttons. |

#### Block: Size ladder

Up to 1 per section.

> Shows the size option as rows of measurements from the product's size chart. Set the option name and the size chart metafield in Theme settings > Fit.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show measuring hint | On or off | On |  |
| Show typical breeds | On or off | On |  |
| Show stock status | On or off | On |  |
| Show link to the size chart | On or off | On |  |

**How to measure**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show how to measure link | On or off | On |  |
| Measuring guide page | Page |  | Defaults to the measuring guide page in Theme settings > Fit. Without a page, the block shows three measuring steps. |
| Image | Image |  | 900 x 600px .png recommended |

#### Block: Fit note

Up to 1 per section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Text | Text, several lines |  | The product's custom.shown_on metafield replaces this text when it has a value. |

#### Block: Quantity selector

Up to 1 per section.

No settings.

#### Block: Purchase options

Up to 1 per section.

> Shows subscription options for products with selling plans.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text |  |  |
| Note | Text |  |  |

#### Block: Buy buttons

Up to 1 per section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Show dynamic checkout buttons | On or off | On | Shows the shopper's preferred express payment method, such as PayPal or Apple Pay, from the ones your store offers. |
| Let gift card buyers add a recipient | On or off | On | Lets customers send a gift card to a recipient on a chosen date, with a personal message. |

#### Block: Pickup availability

Up to 1 per section.

> Shows where the selected variant can be picked up, for locations with local pickup on.

#### Block: Complementary products

Up to 1 per section.

> Choose complementary products in the Search and Discovery app.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text |  |  |
| Maximum products to show | Slider, 2 to 4 | 3 |  |

#### Block: Collapsible tab

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text |  |  |
| Icon | Choice: None, Info, Ruler, Scissors, Shirt, Truck, Package, Exchange, Repeat, Tag, Gift, Lock, Map pin, Clock, Message, Dog, Cat | None |  |
| Content | Formatted text |  |  |
| Content from a page | Page |  | Replaces the text above. A tab with no text and no page is hidden. |
| Start expanded | On or off | Off |  |

#### Block: Share

Up to 1 per section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Label | Text | `Share` |  |

> Opens the device share sheet, or copies the product link where sharing is not available.

#### Block: Custom Liquid

| Setting | Type | Default | Notes |
|---|---|---|---|
| Liquid | Liquid code |  | Paste app snippets or your own Liquid code. |

Accepts app blocks.

### Related products

Where: Add section, only on product templates.

> Recommendations come from Shopify and improve with sales. Adjust them in the Search and Discovery app.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text |  |  |
| Link label | Text |  |  |
| Link | Link |  |  |
| Maximum products to show | Slider, 2 to 8 | 4 |  |
| Number of columns on desktop | Slider, 2 to 5 | 4 |  |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 88 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

### Restock list

Where: Add section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text with bold, italic and links |  |  |
| Body text | Formatted text |  |  |
| Products | Products |  |  |
| Collection | Collection |  | Fills the list when no products are selected |
| Products to show from the collection | Slider, 2 to 8 | 5 |  |
| Show subscription note | On or off | On | Shows on products that have selling plans. Shoppers choose the plan on the product page. |
| Link label | Text |  |  |
| Link | Link |  | Defaults to the collection, or to all products |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 88 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

### Rich text

Where: Add section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text with bold, italic and links |  |  |
| Heading size | Choice: Large, Medium, Small | Medium |  |
| Body text | Formatted text |  |  |
| Button label | Text |  |  |
| Button link | Link |  | Defaults to all products |
| Button style | Choice: Solid, Outline | Outline |  |
| Alignment | Choice: Left, Center | Left |  |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 88 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

### Search results

Where: part of the Search template.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Results per page | Slider, 8 to 48 | 24 |  |
| Show article images | On or off | On |  |

**Refine results**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Enable filtering | On or off | On | Filters apply to products. Set them up in the Search and Discovery app. [Learn more](https://help.shopify.com/manual/online-store/search-and-discovery/filters) |
| Filter layout | Choice: Sidebar, Drawer | Drawer | Phones always use the drawer. |
| Show in stock switch | On or off | On | Replaces the availability filter with one switch. |
| Show sorting | On or off | On |  |

**Suggested searches**

> Suggestions show before a search starts and when a search has no results.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Navigation | Menu |  | Shows its links as suggestions. |
| Search terms | Text |  | Separate terms with commas. The section shows them when no navigation is selected. |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 32 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

### Size chart

Where: Add section, only on product templates.

> Shows the size chart of the product, from the metafield set in Theme settings > Fit.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text |  | Leave blank to show the name of the size chart entry. |
| Text | Formatted text |  |  |
| Show typical breeds | On or off | On |  |
| Show links to other body shapes | On or off | On | Needs the body shape metafield as a filter in the Search and Discovery app. |
| Color scheme | Color scheme | Scheme 2 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 88 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

### Size charts

Where: Add section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text with bold, italic and links |  |  |
| Body text | Formatted text |  |  |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 88 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

#### Block: Size chart

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text |  | Shows on the tab and above the table |
| Body shape icon | Choice: None, Standard, Deep chest, Long body, Broad chest | Standard |  |
| Unit of the values | Choice: Inches and pounds, Centimeters and kilograms | Inches and pounds | Shoppers can switch between inches and centimeters, and the theme converts the values for them |
| Length column headings | Text |  | Separate headings with commas |
| Weight column heading | Text | `Weight` | Leave empty when the chart has no weight column |
| Notes column heading | Text |  | A last text column, such as typical breeds. Leave empty to hide it |
| Rows | Text, several lines |  | One size per line. Separate cells with \|, starting with the size, then the length columns, the weight and the note. Ranges use a hyphen, such as 17-21 |
| Note below the table | Text |  |  |

### Slideshow

Where: Add section.

> Slides change only when a shopper uses the arrows or dots.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text |  | Only screen readers announce this heading |
| Image shape | Choice: Landscape 5:4, Wide 16:9, Square | Landscape 5:4 |  |
| Show previous and next buttons | On or off | On |  |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 88 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

#### Block: Slide

| Setting | Type | Default | Notes |
|---|---|---|---|
| Image | Image |  | 1600 x 1280px .jpg recommended |
| Heading | Text with bold, italic and links |  |  |
| Body text | Formatted text |  |  |
| Button label | Text |  |  |
| Button link | Link |  | Defaults to all products |

### Testimonials

Where: Add section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text with bold, italic and links |  |  |
| Body text | Formatted text |  |  |
| Color scheme | Color scheme | Scheme 2 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 88 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

#### Block: Testimonial

| Setting | Type | Default | Notes |
|---|---|---|---|
| Quote | Text, several lines |  |  |
| Author | Text |  |  |
| Image | Image |  | Shows as a circle. 200 x 200px .jpg recommended |

**Fit details**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Breed | Text |  |  |
| Weight | Text |  |  |
| Product and size bought | Text |  |  |
| Fit | Text |  | Such as true to size |
| Lead quote | On or off | Off | Takes a wider column and two rows on large screens |

### Video

Where: Add section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text with bold, italic and links |  |  |
| Body text | Formatted text |  |  |

**Source**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Shopify-hosted video | Shopify-hosted video |  | Takes priority over the YouTube or Vimeo link |
| YouTube or Vimeo link | YouTube or Vimeo link |  |  |
| Cover image | Image |  | Shows until the video plays. Defaults to the preview of the Shopify-hosted video. 1600 x 900px .jpg recommended |
| Description for screen readers | Text |  | Defaults to the heading |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 88 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |

### Video banner

Where: Add section.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Heading | Text with bold, italic and links |  |  |
| Heading level | Choice: Page heading (h1), Section heading (h2) | Section heading (h2) | Use Page heading (h1) when this is the first section of the home page |
| Body text | Formatted text |  |  |
| Button label | Text |  |  |
| Button link | Link |  | Defaults to all products |

**Video**

> The video plays muted on a loop, so choose a clip that needs no sound or captions. Shoppers can pause it.

| Setting | Type | Default | Notes |
|---|---|---|---|
| Video | Shopify-hosted video |  | Shopify-hosted. A 10 to 30 second clip at 1920 x 1080px is recommended |
| Mobile video | Shopify-hosted video |  | Optional. Plays on screens narrower than 750px. A 1080 x 1350px clip is recommended |
| Cover image | Image |  | Shows until the video plays, and stays when a shopper's device asks for reduced motion. Defaults to the video preview. 1920 x 1080px .jpg recommended |
| Play automatically | On or off | On | Starts after the page has loaded and the section is on screen |

**Layout**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Shape | Choice: Wide 16:9, Extra wide 21:9, Landscape 3:2 | Wide 16:9 |  |
| Mobile shape | Choice: Portrait 4:5, Tall 9:16, Square, Same as larger screens | Portrait 4:5 |  |
| Text position | Choice: Left, Center, Right | Left | On mobile the text sits below the video |
| Color scheme | Color scheme | Scheme 1 |  |

**Section padding**

| Setting | Type | Default | Notes |
|---|---|---|---|
| Top padding | Slider, 0 to 160 px | 88 px |  |
| Bottom padding | Slider, 0 to 160 px | 88 px |  |
