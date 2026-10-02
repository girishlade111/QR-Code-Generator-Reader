# QR Code Hub — Generator & Reader

A lightweight, zero-build web app that generates and reads QR codes entirely in the browser. Includes a bonus word & character counter tool. No dependencies to install, no server, no tracking — open the page and use it.

## Features

**Generator**
- Encode URLs or plain text into QR codes instantly
- Customize size, foreground/background colors, and error-correction level (L / M / Q / H)
- Overlay a logo image at the center of the code
- Download the result as **PNG, JPEG, or SVG**
- Generation history saved in `localStorage` (clearable)

**Reader**
- Decode QR codes two ways: upload an image file, or scan live with your device camera
- Decoded text shown with copy support

**Bonus tool**
- Word & character counter (`/word-counter/`) — live counts for words, characters (with/without spaces), sentences, and estimated reading time

**UI**
- Light / dark mode toggle
- Fully responsive, single-file pages

## Tech Stack

- Plain HTML, CSS, and vanilla JavaScript — no build step
- QR encoding: `qrcodejs` (CDN)
- QR decoding: `jsQR` (CDN)

## Quick Start

No installation needed. Either:

```bash
# open directly
open index.html
```

or serve the folder with any static server:

```bash
npx serve .
# or
python3 -m http.server 8000
```

Camera scanning requires a secure context (HTTPS or localhost) for `getUserMedia` to work.

## Project Structure

```
QR-Code-Generator-Reader/
├── index.html                  # QR Code Hub (generator + reader)
└── word-counter/
    └── index.html              # word & character counter tool
```

## Deploy

Static site — deployed on GitHub Pages from the `main` branch (root path `/`).

---

Built by Girish Lade — https://ladestack.in
