# Simtech Computers – Website

A one-page website for **Simtech Computers**, Jayanagar, Bengaluru.
The shop sells Grade A+ certified refurbished laptops, MacBooks, desktops, workstations and mobiles, and offers service and upgrades. It has been open since 2007.

---

## Files

| File | What it is |
|---|---|
| `simtech-computers.html` | The complete website: layout, styles, scripts and all photos in one file |
| `README.md` | This guide |

The site has no build step, framework or server code. All store photos are embedded inside the HTML file, so it works on its own. It only needs an internet connection to load its fonts from Google Fonts. If the fonts can't load, it falls back to system fonts.

---

## Preview it

Double-click `simtech-computers.html` to open it in any browser (Chrome, Edge, Firefox or Safari).

---

## Put it online

The site is a single static file, so any static host works. Rename the file to **`index.html`** first, so it loads as the home page.

**Netlify Drop (easiest, free)**
1. Go to https://app.netlify.com/drop
2. Drag a folder containing `index.html` onto the page.
3. Netlify gives you a live link. You can connect your own domain later.

**GitHub Pages (free)**
1. Create a repository and upload `index.html`.
2. Go to **Settings → Pages**, choose the `main` branch, and save.
3. The site goes live at `https://<username>.github.io/<repo>/`.

**Your own hosting (cPanel, Hostinger, GoDaddy and similar)**
Upload `index.html` to the `public_html` folder using the File Manager.

---

## Page sections

| Section | What it shows |
|---|---|
| Header | Logo, Kannada name, menu (becomes a ☰ button on phones) |
| Opening section | Headline, Call and Directions buttons, 4.8★ rating, and three store photos shown inside laptop screens on a wooden shelf |
| Brand strip | Scrolling list: MacBook, Lenovo, Dell, HP, Acer, Asus, MSI |
| Stats | Since 2007 · 1,425 reviews · 4.8★ · Grade A+ |
| Products | Laptops & MacBooks, Desktops, Workstations, Phones & tablets, Bulk orders, Service |
| MacBook | MacBook Air and Pro cards, photos, WhatsApp enquiry button |
| Find a laptop | Customer picks a use; the page shows the specs to look for and sends the enquiry on WhatsApp |
| On the shelf | Typical configurations (examples, not live stock) |
| Showroom | Gallery of five photos; tap a photo to enlarge it |
| Why Simtech | Rating card and four reasons to buy |
| FAQ | Six common questions that open and close |
| Visit | Address with a copy button, two phone numbers, hours, Google Maps link, storefront photo |
| Phone bar | Call / WhatsApp / Directions bar fixed to the bottom of the screen on phones |

The page has no prices anywhere.

---

## Editing common details

Open `simtech-computers.html` in a text editor such as VS Code or Notepad++. Use **Find & Replace** (Ctrl+H).

| To change | Search for |
|---|---|
| Main phone number | `919632178786` (links) and `96321 78786` (visible text) |
| Second phone number | `919986916076` and `99869 16076` |
| WhatsApp number | `wa.me/919632178786`. It currently uses the main number, so change it if your WhatsApp uses a different one |
| Opening hours | `closes 7 pm` |
| Address | `680/58, 30th Cross` |
| Google rating / review count | `4.8` and `1,425` / `data-count="1425"` |
| MacBook models | `MacBook Air` / `MacBook Pro` cards in the `id="macbook"` section |
| Laptop finder suggestions | `var DATA = {` in the script near the bottom of the file |
| FAQ answers | `<details>` blocks in the `id="faq"` section |

Phone numbers in links must keep the `+91` / `91` country code with no spaces, for example `tel:+919632178786`.

---

## Replacing photos

The photos are embedded as long `data:image/jpeg;base64,...` strings, so the site stays a single file. To use your own photo files instead:

1. Put the photos in an `images/` folder next to `index.html`.
2. In the HTML, replace the matching `src="data:image/jpeg;base64,....."` with `src="images/your-photo.jpg"`. Gallery photos also have a matching `data-full="..."` attribute; change that too.
3. Upload the `images/` folder together with `index.html`.

Use wide photos (about 1600 × 1000 px) for the sharpest result. Some of the current photos are small, so they look slightly soft when shown large.

---

## Before going live, check:

- [ ] Both phone numbers are correct, and **96321 78786** is on WhatsApp
- [ ] Full weekly opening hours, including Sunday
- [ ] MacBook models and chips match what you actually stock
- [ ] The brands listed (Lenovo, Dell, HP, Apple, Acer, Asus, MSI) are right
- [ ] Rating and review count are current (update them now and then)

---

## Features

- Works on phones, tablets and desktops; nothing scrolls sideways on small screens
- Light and dark mode, following the visitor's device setting
- Animations when the page loads and as you scroll; turned off for visitors who choose "reduce motion" on their device
- Can be used with a keyboard (visible focus outlines; the photo viewer closes with Esc)
- Text and labels for screen readers on images and buttons

---

© 2026 Simtech Computers · 680/58, 30th Cross, Swagath Road, 4th T Block East, Jayanagar, Bengaluru 560041
