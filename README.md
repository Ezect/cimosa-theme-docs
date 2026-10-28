# Cimosa: user documentation

Cimosa is an editorial Online Store 2.0 theme for fashion and apparel stores. It uses plain CSS and JavaScript, supports optional 3D product models and scroll effects, and ships with English and Italian translations (storefront and theme editor).

Version 1.0.0. Support: see SUPPORT-EN.md (https://github.com/Ezect/cimosa-theme-docs/issues). Third-party licenses: see the credits file.

## Contents

1. Installation
2. Getting started in the theme editor
3. Sections and blocks
4. Theme settings
5. Presets
6. 3D viewer
7. Collections and search
8. Product page, cart and checkout
9. Accessibility
10. Languages
11. FAQ
12. Troubleshooting
13. Support

## 1. Installation

Option A: upload a zip
1. In the Shopify admin go to Online Store > Themes.
2. Click Add theme > Upload zip file and choose the Cimosa zip.
3. Click Customize on the uploaded theme to edit it. The theme stays unpublished until you click Publish.

Option B: Shopify CLI
1. Install Shopify CLI.
2. In the theme folder run `shopify theme dev --store your-store.myshopify.com` to preview, or `shopify theme push` to upload.

Before you switch themes, duplicate your current theme (Actions > Duplicate) as a backup.

After installing:
- Set a logo and favicon in Theme settings > Logo.
- Create menus in Content > Menus (a main menu and a footer menu) and select them in the Header and Footer sections. For a mega menu, add sub-items to the top-level links.
- Create the pages you need (About, Contact, FAQ, size guide). Cimosa includes page templates named `page.about`, `page.contact` and `page.faq`.
- Add products and collections. 3D models are optional.

## 2. Getting started in the theme editor

Open Online Store > Themes > Customize. Use the page selector at the top to move between Home, Product, Collection, Cart, Blog, Search and other pages. On every page you can add, remove and reorder sections; each section has its own settings and blocks. The header and footer are section groups shared by all pages. Settings that apply everywhere are in Theme settings.

The home page is built from many Cimosa sections. You do not need all of them: remove any section you do not want and the rest of the page does not change.

## 3. Sections and blocks

Names are as shown in the theme editor.

### Home and marketing sections

| Section | What it does | Blocks |
|---|---|---|
| Cimosa: Hero | Large layered hero with heading, text and buttons | none |
| Cimosa: 3D hero | Hero with a 3D object (product model or bundled demo model) | Fact |
| Cimosa: Stacked bands | Full-width photo bands that cover each other while scrolling | Band |
| Cimosa: Stacked cards | Cards that pile up while scrolling | Card |
| Cimosa: 3D carousel | Cover-flow carousel | Slide |
| Cimosa: Floating images | Images floating at different depths | Image |
| Cimosa: 3D spotlight | 3D object with hotspots | Hotspot |
| Cimosa: 3D showcase | Gallery of 3D objects, or an object turning with the scroll (two sections share this name) | Object; Shape, Word |
| Cimosa: Scroll text | Giant text lines sliding in opposite directions, with counters | Line, Stat |
| Cimosa: Story sticky | Sticky storytelling section with steps | Step, App |
| Cimosa: H-scroll | Horizontal scrolling gallery | none |
| Cimosa: Scroll gallery | Scroll-driven gallery | Slide, App |
| Cimosa: Lookbook | Lookbook with product hotspots | Hotspot |
| Cimosa: Shop the look | Shoppable lookbook | Hotspot |
| Cimosa: Editorial | Editorial layout with looks | Look |
| Cimosa: Feature story | Feature story with facts | Fact |
| Cimosa: Category mosaic | Mosaic of category tiles | Tile |
| Cimosa: Collection grid | Grid of collections | Collection |
| Cimosa: Gallery | Photo gallery | Photo |
| Cimosa: Marquee | Scrolling text strip | Text |
| Cimosa: Video | Full-width video | none |
| Cimosa: Promo banner | Promotional banner | App |
| Cimosa: Countdown | Countdown to a date | none |
| Cimosa: Brand story | Image and text story | App |
| Cimosa: Benefits | Benefit columns | Benefit, App |
| Cimosa: Trust strip | Strip of short trust messages | Item |
| Cimosa: Reviews | Customer reviews (entered manually) | Review, App |
| Cimosa: Quote wall | Wall of quotes | Quote |
| Cimosa: FAQ | Questions and answers | Question, App |
| Cimosa: Journal | Latest blog posts | none |
| Cimosa: Newsletter | Newsletter sign-up form | App |
| Cimosa: Contact | Contact details, social links and FAQ | Detail, Social, FAQ, App |
| Cimosa: Size guide | Size chart tables | Size |
| Announcement bar | Messages at the top of the page | Message |
| Custom Liquid | Your own Liquid, HTML or CSS | App, Custom Liquid |

Replace the sample review and quote texts with real ones before you publish.

### Product sections

| Section | What it does | Blocks |
|---|---|---|
| Cimosa: Featured | Products from a collection | none |
| Featured product | One product with buy buttons | App, Text, Brand, Title, Price, Description, Buy buttons, Link, Custom Liquid |
| Cimosa: Related products | Related products (Shopify recommendations) | none |
| Complementary products | Complementary products (Shopify recommendations) | none |
| Cimosa: Recently viewed | Products the visitor looked at | none |

### Header, footer and cart

| Section | Blocks |
|---|---|
| Header | Mega menu feature, Menu badge, App |
| Footer | Menu, Text, Newsletter, App |
| Cart drawer | none (cart type is set in Theme settings > Cart) |

### Main page sections

Product, Collection page, Collection list page, Cart page, Search page, Blog, Article, Page, Contact form, 404 page, Password page, and the customer account pages (Login, Register, Reset password, Activate account, Account, Addresses, Order).

Product page blocks: Title, Badges, Rating, Price, Variant picker, Size guide, Buy buttons, Description, Pickup availability, Shipping and returns, Collapsible row, Payment icons, Custom Liquid and App. The Page section supports App and Custom Liquid blocks.

Where a section lists App blocks you can add blocks from installed Shopify apps (reviews, subscriptions, wishlists and so on).

## 4. Theme settings

Open Theme settings in the editor.

- Logo: logo image, logo width, favicon.
- Colors: Color mode (Light, Dark, or Automatic, which follows the visitor's device). Light palette: background, text and buttons, secondary text, surface, accent for text and links, warm grey, accent, sale badge, new badge. Dark palette: background, text and buttons, secondary text, accent. Keep a contrast ratio of at least 4.5:1 for text colors.
- Typography: heading font and body font (Shopify font library), uppercase headings, heading scale, body size.
- Layout: maximum page width (Narrow, Wide, Full width), side margin, space between sections.
- Buttons: corner radius and button style.
- Cards: product card image ratio, second image on hover, show brand, show badges.
- Motion effects: see below.
- Shopping features: quick view on product cards; light/dark switch in the header.
- Cart: cart type (Drawer or Page) and order note.
- Social: Instagram, Facebook, TikTok, YouTube and Pinterest links. Leave empty what you do not use.

### Motion effects

Path: Customize > Theme settings > Motion effects.

- Motion effects: Off (static pages, effect files are not loaded), Reduced (soft fades only) or Full (3D, parallax, scroll effects).
- Effect intensity: Low, Medium or High. It scales angles, distances and shadows.
- Each effect has its own switch: reveal on scroll, photo parallax, titles that slide in, 3D card entrance, 3D tilt, clip-path photo bands, marquee, image zoom, hero layers, split titles, 3D curtain, card flip, glare, 3D carousel, stacked cards, 3D showcase, giant text lines, animated counters, section perspective, background parallax, dynamic shadow, floating images, 3D photo turn, microinteractions, custom cursor.
- Start 3D objects automatically when they scroll into view.

Visitors whose device asks for reduced motion always see a static page, whatever you choose. If your store feels slow on phones, choose Reduced or intensity Low and switch off the effects you do not need. Some effects use CSS scroll-driven animations, which work in current Chrome, Edge and Safari; in Firefox the page stays static but complete.

## 5. Presets

Cimosa includes one preset, named Cimosa: warm paper background, dark text and a camel accent, with motion set to Full. Every setting can be changed in Theme settings. To keep a variant, duplicate the theme (Actions > Duplicate) before experimenting.

## 6. 3D viewer

Cimosa shows 3D models with Google's open-source model-viewer.

Using your own models:
1. Add a `.glb` file to a product in the Shopify admin (Product > Media). Keep it small (a few MB at most) for fast loading.
2. The product page shows the model in the gallery with a "View in 3D" button and a 3D thumbnail.

Demo models: when a product has no 3D file, the Product section setting "3D preview next to the photos" can show a bundled demo model that matches the product type (hat, suitcase, glasses, sneakers, tee, hoodie, jeans). Choose None to turn this off. Real 3D files added in Shopify always take priority. Demo models are previews only.

The 3D hero, 3D spotlight and 3D showcase sections let you pick a product or a bundled demo model.

Behavior:
- A poster image is shown first. The model downloads only when it is about to appear on screen, or when the visitor presses "View in 3D" if automatic start is off.
- It does not start automatically on slow connections or with data saver on.
- The 3D effects follow the Motion effects setting and the visitor's reduced-motion preference.

## 7. Collections and search

- Collection page: product grid with filtering (storefront filters from Shopify Search & Discovery), sorting, pagination, banner and breadcrumbs.
- Collection list page: all collections as cards.
- Search: predictive search in the header and a results page with filters, sorting and pagination.
- To set up filters, install the free Shopify Search & Discovery app and add filters (availability, price, size, color and so on).
- Product cards can show a second image on hover, badges (sale, new), brand and unit price. Quick view is optional in Theme settings.

## 8. Product page, cart and checkout

Product page: gallery (stacked or grid layout, zoom, thumbnails, video, 3D), sticky product info, variant picker with swatches, quantity, unit price, size guide dialog, low stock message, pickup availability, complementary and related products, subscription selling plans, gift card recipient form, sticky add-to-cart bar, accelerated checkout buttons and Shop Pay Installments banner (when enabled in your payment settings).

Cart: choose Drawer or Page in Theme settings > Cart. Both show line items, quantity changes, automatic discounts, a discount code field, an optional order note and the checkout button.

Checkout: Cimosa uses the standard Shopify checkout. Accelerated checkout buttons (for example Shop Pay) appear on the product page and in the cart when enabled in your payment settings. To style the checkout (logo, colors, fonts) use the checkout customization in the theme editor or Settings > Checkout.

Customer accounts: login, register, reset password, addresses, order history and order details. Gift card pages show a QR code for in-store use. Language and country selectors are available when your store has more than one language or market. The footer can show the Follow on Shop button.

## 9. Accessibility

Cimosa is built with accessibility in mind:
- Skip-to-content link, visible keyboard focus and page landmarks.
- Menus, the cart drawer, quick view and dialogs can be used with the keyboard.
- Form fields have labels and error messages are shown next to the form.
- Images use the alt text you set in Shopify; add it to every meaningful image (products: Product > image > Edit alt text; images picked in sections: Content > Files). Purely decorative images do not need it.
- Motion respects the visitor's reduced-motion device setting, and you can switch motion off or reduce it in Theme settings.
- Check contrast when you choose custom colors and when placing text over photos (increase the overlay opacity if needed).

Accessibility also depends on your content: write alt text, use clear headings, and test with a keyboard and a screen reader before launch.

## 10. Languages

Storefront text and editor labels are included in English and Italian. For other languages, edit the translations in Online Store > Themes > Actions > Edit default theme content, or use Shopify's Translate & Adapt app. The language and country selector appears when you sell in more than one language or market.

## 11. FAQ

**Can I turn off all effects?** Yes: Theme settings > Motion effects > Off.

**Does Cimosa work with apps?** Yes. App blocks are supported on the product page and in many sections. Not every 3D section has app blocks.

**Is the theme fast?** Speed depends on your images, apps and the effects you keep on. Measure your own store with PageSpeed Insights. Choosing Reduced or Off motion and removing unused sections helps.

**Does it have predictive search, color swatches and unit prices?** Yes, all three are included.

**Do I need 3D models?** No. 3D is optional and can be left unused.

**Can I use my own fonts?** Cimosa uses the Shopify font library (font picker). No font files are bundled.

**Does Cimosa include a demo store content?** The preset gives you the look; add your own products, collections and images.

**Where do I report a problem?** See Support below.

## 12. Troubleshooting

- 3D model does not appear: check the file is a `.glb`, that it is attached to the product under Media, and that Motion effects is not Off for automatic start (the visitor can still press "View in 3D").
- Effects do not run: set Motion effects to Full and check the single effect switch. Devices set to reduce motion always see a static page. Some scroll-driven effects show a static layout in Firefox.
- Text is hard to read: raise contrast in Theme settings > Colors. For text over photos use a darker photo or a stronger overlay.
- Filters do not show: install Shopify Search & Discovery and add filters.
- Header menu is empty: create a menu in Content > Menus and select it in the Header section.
- Cart drawer does not open: check Theme settings > Cart > Cart type is Drawer.
- Quick view or sticky bar missing: they are desktop features and can be turned off in Theme settings or in the Product section.
- Page is slow: use smaller images, remove sections you do not need, limit 3D objects per page and uninstall unused apps.
- Editor labels in the wrong language: the editor uses the language of your staff account; English and Italian are included.
- A font does not load: pick another in Theme settings > Typography.

## 13. Support

Contact the theme author through the support page (https://github.com/Ezect/cimosa-theme-docs/issues). Please include your store URL, the page where the problem happens, your browser and a screenshot. We answer within 2 business days. See SUPPORT-EN.md for what is covered.
