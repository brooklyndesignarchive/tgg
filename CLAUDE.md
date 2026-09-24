# The Gerardo Guide

Design criticism site by Gerardo Torres Dávila. Jekyll, hosted on GitHub Pages.

## Where it lives
- Repo: brooklyndesignarchive/tgg, branch `main`, built by GitHub Pages from the root.
- Live now at https://brooklyndesignarchive.github.io/tgg/ (so `_config.yml` has `baseurl: "/tgg"`).
- The domain thegerardoguide.com (bought at Porkbun) is not connected yet. When it is: add a `CNAME` file containing `thegerardoguide.com`, set `url` to `https://thegerardoguide.com` and `baseurl` to `""`, and point Porkbun DNS at GitHub Pages (four A records 185.199.108–111.153, `www` CNAME to brooklyndesignarchive.github.io).

## Structure
- `index.html`: the Articles list (homepage).
- `_layouts/default.html`: shell with the "The Gerardo Guide" eyebrow. `_layouts/post.html`: article header (title, dek, place and month) plus body.
- `_posts/YYYY-MM-DD-name.md`: one file per article. Front matter: `title`, `dek`, `description` (same as dek, for link previews), `place`, `permalink` (short, like `/baltimore/`).
- `assets/css/style.css`: all styling.
- Plugins: jekyll-feed, jekyll-seo-tag, jekyll-sitemap (all GitHub Pages defaults).

## Design decisions (settled; don't change without asking)
- Typeface: Iowan Old Style first, Georgia fallback. System fonts only, nothing loaded from Google Fonts. Gerardo rejected every Google Fonts option.
- Colors: graphite #232323 text on white, muted grey #7A7A7A for dateline, blue-grey #5B6773 for the eyebrow. Dark mode swaps to #121212 paper.
- Layout: single centered column (38rem). Centered header (eyebrow, headline, italic dek, spaced-caps dateline), left-aligned body.
- Hierarchy: headline regular weight, large. Section heads (`##`) are bold and smaller than the headline, so they read as a separate level. Only the eyebrow and dateline use small spaced caps.
- In articles: `* * *` makes the short centered rule; `{: .close}` under a paragraph makes the large centered closing line; `{: .sign}` makes the italic "— G." sign-off.

## Working with Gerardo
- Plain, direct writing. No flourish.
- Don't invent facts, names, dates or quotes; leave a [bracket] and ask.
- He's a designer and has strong type opinions: show options, don't lecture.

## Open items
- "1922 library" in the Baltimore piece came from research; he should verify it.
- The Baltimore draft had an "Elizabeth [last name]" maker line that was left out until he supplies it.
- Newsletter signup (Buttondown or similar) not added yet.
