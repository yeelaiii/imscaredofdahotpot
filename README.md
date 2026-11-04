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

Motion: [GSAP](https://github.com/greensock/GSAP) 3.15.0 (with ScrollTrigger, MotionPath and Flip) drives the day page-flip swipe, the self-drawing route map with a travelling plane, stamp thunks, tick scribbles, polaroid drops and zoom, the flick-through photo pile, to-dos that slide down when done, the split-flap departure board and the trip book's scroll reveals. Shangri-La and Jade Dragon pages get light snow. Ideas for the departure board, photo pile, snow and circling stamp text came from [React Bits](https://github.com/DavidHDev/react-bits) (SplitFlapText, Stack, PixelSnow, CircularText), rebuilt in plain JavaScript. Everything switches off when the phone has Reduce Motion on.

Libraries (pasted into `index.html` so the page doesn't depend on a CDN, which helps in China): [GSAP](https://github.com/greensock/GSAP) ([standard license](https://gsap.com/standard-license)), [Rough.js](https://github.com/rough-stuff/rough), [Rough Notation](https://github.com/rough-stuff/rough-notation), [canvas-confetti](https://github.com/catdad/canvas-confetti). Fonts from Google Fonts (Caveat, Nunito, IBM Plex Mono, ZCOOL KuaiLe), with system fallbacks where Google is blocked.
