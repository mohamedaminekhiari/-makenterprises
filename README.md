# MAKE — Mohamed Amine Khiari Enterprises Website

Single-file static site (no build step). HTML + Tailwind CDN + vanilla JS.

## 1. File structure
```
make-site/
├── index.html          ← entire site
├── public/images/      ← put real screenshots/photos here
└── README.md
```

## 2. Run locally
Just open `index.html` in a browser, or serve it:
```
npx serve .
```

## 3. Replace before publishing
- **Contact form**: create a free account at web3forms.com, get an access key, replace
  `REPLACE_WITH_WEB3FORMS_ACCESS_KEY` in the `<input type="hidden" name="access_key">` line.
- **Images**: replace the six placeholder blocks in the "Evidence room" section with real
  `<img>` tags pointing to `/public/images/...` (see checklist below).
- **Links**: `Own Your Fund Category™` now points to `https://cal.com/ofc-access`, general consulting points to `https://calendly.com/makofficialtm`, and direct email uses `contact.makofficial@gmail.com`.
- **Analytics**: add your analytics snippet (e.g. Plausible or GA4) just before `</head>`.

## 4. Deploy free
**Vercel**: `npx vercel` from this folder, or drag-and-drop the folder at vercel.com/new.
**Netlify**: drag-and-drop the folder at app.netlify.com/drop.
No environment variables or backend required.

## 5. Asset checklist (real files only — no AI-generated screenshots)
- [ ] Founder headshot(s) — hero + about
- [ ] VC Lab / Decile evidence (certificate, program page, public reference)
- [ ] GFOIS website screenshot (Invitation Host page)
- [ ] Fiscalité Tunisienne — group screenshot + analytics/insights screenshot
- [ ] The Reserve Insights — newsletter or platform screenshot
- [ ] The Reserve Capital — site or deck screenshot (if public-facing version exists)
- [ ] Own Your Fund Category™ — any existing framework document/deck excerpt

## 6. Open items requiring your input
1. Web3Forms access key (or swap for Formspree / mailto fallback).
2. Replace `REPLACE_WITH_WEB3FORMS_ACCESS_KEY` before enabling the contact form.
3. Review all live links (`https://cal.com/ofc-access`, `https://calendly.com/makofficialtm`, LinkedIn, GFOIS, newsletter) after each deploy.
4. Keep `public/assets/make-logo-cropped.png` as the active header/favicon logo asset.
