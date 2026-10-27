# TRH — food, stays & rental

Static marketing site (HTML / CSS / JS, no build step) hosted on GitHub Pages
at `trrh.shop`.

> Generated from `C:\Users\souha\coaching-sites-factory` (content file `sites/trrh.mjs`).
> To change the content, edit that file and run `node build.mjs trrh` — editing the
> HTML here directly would be overwritten on the next build.

## Before you promote this site

| Priority | What | Where |
|---|---|---|
| 🔴 Blocking | Legal page: fill every `[BRACKET]` (legal name, address, state, payment provider). Have a lawyer review it if you can. | `legal.html` |
| 🟠 Important | `contact@trrh.shop` doesn't exist yet: set up free email forwarding in Namecheap (*Domain List → Manage → Redirect Email*). | Namecheap |
| 🟠 Important | Contact form: replace `VOTRE_ID_FORMSPREE` with your Formspree id (until then it falls back to `mailto:`). | `contact.html` |
| 🟠 Important | Add a real introduction of the coach (name, background, photo). Never invent credentials. | `about.html` |
| 🟡 Later | Prices ($Per order / $Per stay / $Declined) and plan contents should match what you actually sell. | `index.html` `#pricing` |
| 🟡 Later | Testimonials: only add real ones, with permission. Fake reviews are illegal (FTC). | — |

## Business description (Stripe, directories…)

```
We are TRH, a small family company in Wingene, West Flanders, running several things rather than one. 't smulhoekske in Tielt is a limited-service eatery with a small shop alongside it. The Cozy Relax Home in Beernem is a holiday house let to guests. And from Wingene we rent out light vehicles and caravans. Each of those sits under a different set of rules and we would rather state them than let a guest or a customer find out later. Our holiday accommodation is registered as Flemish law requires and holds the fire safety certificate issued by the commune, which is a document worth asking any accommodation for. Allergen information is given on request for everything we serve, including food that is not pre-packed. And before you tow a caravan we check your licence category, because beyond certain weights a category B licence is not enough. Site: trrh.shop
```

## Structure

```
index.html            Home: hero, programs, method, pricing, approach, FAQ
programs.html         The four programs in detail
about.html            How we work, principles
contact.html          Contact form
legal.html            Business info, privacy policy, terms of service
404.html              Error page (absolute paths)
assets/css/style.css  Brand colors at the top, shared styles below
assets/js/main.js     Menu, theme, animations, form
```

## DNS (Namecheap → Advanced DNS)

Delete the parking records, then add:

| Type | Host | Value |
|---|---|---|
| A Record | `@` | `185.199.108.153` |
| A Record | `@` | `185.199.109.153` |
| A Record | `@` | `185.199.110.153` |
| A Record | `@` | `185.199.111.153` |
| CNAME Record | `www` | `hamzaniceguy99-glitch.github.io.` |
