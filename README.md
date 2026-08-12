# Bigme Forge

Wraps any glyph in the Bigme monochrome plate — a white squircle with a thin black outline and a centered black icon, matching the e-ink look of the Bigme OS system icons.

➡️ [**Link Here**]([https://novalauncher.com/](https://joemk88.github.io/Bigme_Forge/)) 

<img width="1156" height="1061" alt="sss8-11 231252" src="https://github.com/user-attachments/assets/a4379670-f2fe-4cd4-878c-a6975fed1259" />

It's a single self-contained HTML page. Paste app names, it finds a black-and-white glyph for each via the [Iconify](https://iconify.design) API, forges it onto the plate, and hands you back PNGs named after your input (`Spotify → Spotify.png`).

\---

## ⚠️ These icons won't work with the stock Bigme OS launcher

The default Bigme launcher doesn't let you assign a custom icon to an app. 

To use these icons you need a launcher that supports **custom per-app icons** (or icon packs). On a Bigme HiBreak / other e-ink Android device, install one of these and set it as your default home app:

* [**Nova Launcher**](https://novalauncher.com/) — long-press an app → Edit → tap the icon → pick your PNG. The most flexible option and what these plates are tuned for.
* [**Lawnchair**](https://lawnchair.app/) — free and open-source, supports custom icons and icon packs.
* [**Smart Launcher**](https://play.google.com/store/apps/details?id=ginlemon.flowerfree) — per-app icon editing, has a dedicated e-ink-friendly mode.
* [**Niagara Launcher**](https://niagaralauncher.app/) — minimal list-style launcher; custom icons in the paid tier.
* [**Kvaesitso**](https://kvaesitso.mm20.de/) — open-source, search-first, custom icons and icon packs; popular on e-ink.

Any launcher with a "change icon → choose image" feature will work — the PNGs are standard transparent-background images.

\---


## Using it

1. Type or paste app names, **one per line**, in the left box.
2. Pick a **set** (see below), then hit **Find icons**.
3. Tweak the plate — corner, outline weight, glyph scale, colours — everything previews live.
4. **Download all as ZIP**, or hover a tile and grab its **PNG** on its own.
5. In your launcher, assign each PNG to the matching app.

You can also **drop your own SVG / PNG / WebP** onto the page to forge custom art instead of a looked-up glyph.

If the auto-picked glyph isn't right, click the little **set label** under a tile to cycle through other matching sets, or **×** to remove it and try a more specific name.

## Icon sets

Iconify aggregates \~150 icon libraries, each with its own style. The **set** dropdown decides which one the picker draws from, so your whole sheet shares one look:

|Set|Best for|
|-|-|
|**smart**|Quick first pass — brands first, then clean line sets|
|**simple-icons**|Brand logos (Spotify, PayPal, Reddit) as flat silhouettes|
|**lucide** / **tabler**|Thin, even-stroke line icons — closest to stock Bigme glyphs|
|**mdi**|Material Design Icons — big, dependable, medium weight|
|**material-symbols**|Google's newer set, cleaner geometry|
|**ph** / **solar**|Rounder, more characterful line sets|

**Tip for a cohesive pack:** lock concept apps to one line set (**lucide** or **tabler**), and switch to **simple-icons** only for the brand apps.

## Plate controls

* **Corner** — Squircle (true superellipse, the Bigme curve) or plain Rounded.
* **Corner radius** — rounds the squircle; higher = softer.
* **Plate inset** — margin between the outline and the icon edge.
* **Outline weight** — the black border thickness (0 removes it).
* **Glyph scale** — how much of the plate the icon fills.
* **Force monochrome** — flattens any glyph to a single colour.
* **Swatches** — set glyph / outline / plate-fill colours independently.
* **Transparent plate** — outline only, no white fill.
* **Export size** — 128–512 px output.

The **proof grounds** (light / grey / dark / checker) preview each icon against different wallpapers before you commit.

\---

## Notes

* Runs over HTTPS (GitHub Pages is fine). It fetches glyphs from the Iconify API and JSZip from a CDN, so it needs a connection and won't do live lookups if opened as a raw local file in some browsers.
* Because the stock Bigme launcher wraps icons at runtime, a forged glyph won't be pixel-identical to what Bigme renders automatically — this is for building your own pack in a custom launcher.

## License

MIT — do whatever you like with it.

