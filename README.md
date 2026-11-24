# Booth Book

A home for every photobooth strip. Booth Book saves the soft copy of your photobooth strips in an album that looks and feels like the real thing, so you never lose one again.

## Features

- **Linen-covered album:** the cover shows your newest strip in a small window, with a bulldog clip, a tag and a ribbon bookmark.
- **Ring binder with clear sleeves:** single strips sit two to a page, and double strips get a full-page sleeve.
- **Realistic page turning:** drag a corner, swipe, or use the arrows, and the page curls as it turns.
- **Upload whole strips:** add the booth's digital file exactly as it is (one or many at once), or scan a paper strip and trim it to the edges.
- **Write on the back:** add the date, place, who was there and a note, then tap a strip to flip it over and read them.
- **Looks:** Original, Classic B&W, Warm film, Faded, Cool night and Vivid. They never change your original file.
- **Search:** find strips by friend, place, note or month.
- **Save to phone:** download any strip.
- **iPhone preview:** on a wide screen, the app shows inside an iPhone frame.

## Run it

It's a static site with no build step.

- **Locally:** open `index.html` in a browser.
- **GitHub Pages:** go to the repo's *Settings → Pages*, choose *Deploy from a branch*, then pick `main` and `/ (root)`. The site goes live at `https://<your-username>.github.io/<repo-name>/`.

## Where strips are saved

- **As a Claude artifact:** strips are saved to the owner's Claude account and sync across devices.
- **Anywhere else** (opened locally or on GitHub Pages): strips are saved in that browser only, using IndexedDB. Clearing browser data deletes them, and they don't sync between devices. Account sync would need a backend, such as Firebase or Supabase.

## Project structure

```
index.html                  the whole app (HTML, CSS, JS)
img/rings.png               metal ring bar on the binder spine
img/clip.png                bulldog clip on the cover
lib/page-flip.browser.js    StPageFlip page-turning engine
```

## Credits

- Page turning: [StPageFlip](https://github.com/Nodlik/StPageFlip) by Nodlik, MIT License (see `lib/LICENSE-page-flip.txt`).
- Fonts: Cormorant Garamond, Jost and Caveat from Google Fonts (SIL Open Font License).
- Ring bar and bulldog clip images were supplied by the project owner.
