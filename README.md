# House Hunt: handoff packet for ChatGPT
Date: Sun Oct 25, 2026. Owner: David ("Dad"). Written by Grok Bot.

## What this is
Dad's house-search website. It is one standalone HTML file (dark mode, no build step) with 107 home cards. He opens it in Chrome on his laptop and on his iPhone.
- Live link: https://p7b7volmgd8iuf0y48ywum9o.deed.page/ (unlisted, set to noindex)
- Laptop copy: C:\Users\david\HouseHunt\HouseHunt.html
- Every version is also saved in Dropbox as a new numbered file, e.g. /HouseHunt_v16_2026-10-24.html. Never overwrite an older version.
- GitHub repo (source of truth, ChatGPT/Codex and Grok Bot can both edit): https://github.com/jwdavidho/house-hunt
- GitHub Pages site (auto-updates on every push to main): https://jwdavidho.github.io/house-hunt/
- Repo layout: index.html = the live page; versions/ = every numbered version (never overwrite); robots.txt blocks search engines.

## What Dad is looking for
- A single-story (one-floor) house at or under $1M.
- Areas: Irvine, Lake Forest, Orange, Tustin, Anaheim (including Anaheim Hills). He chose to keep a few Mission Viejo and Laguna Hills homes too.

## What each card shows
- Photo, price, beds, baths, square feet, address.
- Public schools (elementary, middle, high) with GreatSchools ratings, verified against the district's own lookup.
- Nearest private schools with parent-review scores, colored green (4.5 and up), yellow (4.0 to 4.49), red (under 4.0) or gray (no score).
- Buttons: Open on Redfin, Zillow, Google Maps (https://www.google.com/maps/search/?api=1&query=<address>), Google Earth (https://earth.google.com/web/search/<address>).
- A color picker so Dad can mark homes. Each home gets ONE color only: Red, Orange, Yellow, Green, Blue or Purple.

## Page features
- A Filters panel (city, price, beds, schools, and more). It includes multi-select color chips, so Dad can show several colors at once. "No color" is also a chip. Picking no chips shows all homes.
- On iPhone, a blue "Done, show N homes" button closes the filters panel.
- Sort and Search.
- Card colors are saved in the browser's localStorage under the key `housesearch-colors-2026-10-24`. Each home is keyed by its Redfin URL.
- The "Send colors" button makes a link that carries all colors to another device. It replaces the colors there, including cleared ones.
- v17 (being built Oct 25) adds automatic online color sync between laptop and iPhone, with no button needed. Most recent change wins, and clearing a color syncs too.

## Dad's rules (please follow)
1. Short, plain replies. When he asks for "only the link," send one clickable link.
2. No color legend anywhere on the page.
3. Each home keeps one color. Only the filter allows several colors at once.
4. Every new version gets a new number (v17, v18, ...). Never overwrite old files.
5. Before Dad sees any new version, it is tested both as an iPhone (390x844) and as a laptop, and the data is checked. Report only what's wrong.
6. Mobile tap targets must be at least 44px. Use a solid top bar with no blur effects (blur froze iPhone Safari/WebKit).
7. Never put passwords, tokens or keys in the page or in chat.
8. Don't state school boundaries as fact unless the district's own locator confirms them; otherwise label them.
9. No opinions on which house to buy unless Dad asks.

## Known open items
- 74 homes are not yet verified as single-story.
- 32 homes have no Zillow link.
- The About section should match the real listing count (107).

## How to hand work back
If ChatGPT writes a new version, give the full HTML file named HouseHunt_vN_YYYY-MM-DD.html (or commit it to the GitHub repo: put it in versions/ AND copy it over index.html on a branch, then open a pull request). Grok Bot / the House Hunt bot will test it and then publish it to the live link, the laptop and Dropbox.
