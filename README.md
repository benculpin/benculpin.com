# benculpin.com (static)

A static rebuild of [benculpin.com](https://www.benculpin.com) so the site can leave Webflow (~$363/yr) for Cloudflare Pages (~$0 + domain).

This skeleton preserves live copy, URL paths, nav, footer, films, and photography layout. Remaining notebook bodies and some photos can be filled in next.

## Develop

```bash
npm install
npm run dev
```

Open the local URL printed in the terminal.

## Build

```bash
npm run build
npm run preview
```

- Build command: `npm run build`
- Output directory: `dist`

## Cloudflare Pages

1. Connect this repo (or upload `dist`).
2. Build command: `npm run build`
3. Output directory: `dist`
4. Point the domain at Cloudflare. Free plan is enough.

## Contact form

The About form currently posts to `#`. To receive messages, create a Formspree form and set the form `action` in `src/pages/about.astro` to `https://formspree.io/f/YOUR_ID` (method POST).

## Known differences vs live

- Footer **Freelance** now links to `/notebook/freelance` (live `/words/freelance` 404s).
- Photography heading **Saudi Arabia** (live has the typo "Suadia Arabia").
- CV Drive link is kept as on live (`https://drive.google.com/file/d/1E0UvrLqd9Nw9O6z6KIwy-ewdUo8w1zpV/view?usp=drive_link`) but that file currently 404s — re-upload when you have a new CV.
- About bio is the live copy, unchanged.
- Some notebook posts are title/date stubs until remaining bodies are ported.
- Contact form is a stub until Formspree is wired.

## Paths

`/` · `/about` · `/notebook` · `/notebook/{slug}` · `/home` · `/films` · `/photography/nuance-of-experience`
