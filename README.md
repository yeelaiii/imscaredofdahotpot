# imscaredofdahotpot
Jus a lil smt to log and plan my trip with my mushroom head

A scrapbook-style trip companion for our Chongqing → Yunnan trip (28 Dec 2026 – 8 Jan 2027).

## What's in it
- **Today**: countdown before the trip; during the trip, what's on now and next, weather and what to wear, tonight's bed.
- **Days**: one page per day with times and tickable stops. Swipe to flip days. Each page has a photo scrapbook (polaroids) and a "best moment" note from each of us.
- **Map**: hand-drawn route (Rough.js) and five city stamps to collect. Every place has English and Chinese names, a big "Show driver" card for Didi, and Amap links.
- **Ideas**: wishlist, must-eat food list (with spice levels) and a photo-spot shot list.
- **Trip**: bookings, to-dos and packing list.
- **Money**: who paid what and who owes who, in CNY and SGD.
- **Trip book** (`#summary`): an end-of-trip summary to screenshot.

## How it runs
`index.html` is published as a Claude artifact. Shared data (ticks, wishlist, to-dos, expenses, photos, notes and bookings) lives in the artifact's database and asset store, not in this repo, so booking references stay out of the code.

Opened anywhere other than claude.ai, the page still shows the plan, map, places and driver cards, but lists and photos won't load or save.

Libraries (loaded from jsDelivr): [Rough.js](https://github.com/rough-stuff/rough), [Rough Notation](https://github.com/rough-stuff/rough-notation), [canvas-confetti](https://github.com/catdad/canvas-confetti). Fonts from Google Fonts: Caveat, Nunito, IBM Plex Mono, ZCOOL KuaiLe.
