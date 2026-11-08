# Gita Library

Modern liquid-glass Bhagavad Gita reader with all 701 shlokas (Gita Press edition, includes 13.1): Sanskrit, Hindi, Hinglish, English, transliteration, and detailed commentary. Static site, no build step, no backend.

## Run locally
`npx serve .` (or open `index.html` directly).

## Publish on GitHub Pages
Push to a public repo, then Settings > Pages > Deploy from branch `main`, folder `/ (root)`.

## Data layout
- `data/verses.js`: chapters + all verses (Sanskrit, transliteration, Hindi, English) + source names.
- `data/ch1.js` ... `data/ch18.js`: commentary, loaded only when a chapter is opened.
- Hinglish is generated in the browser by converting the Hindi text to Roman script (automatic, spelling can differ).

## Sources and licence
Data is taken from github.com/gita/gita (Unlicense). Hindi translation and commentary: Swami Ramsukhdas. English translation and commentary: Swami Sivananda. Keep this attribution. Check the copyright status of Hindi translation/commentary before relying on it commercially.

## Database later (optional)
Not needed for reading. Use Supabase only for login, bookmarks and cross-device progress; free plan is enough.
