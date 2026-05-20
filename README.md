DWL 3.0 Web Form (pixel-matched to the PDF)

What this is
- A single-page webform that uses the PDF page as a background image and overlays HTML inputs on top.
- The overlay was generated from the PDF's actual form field rectangles (so it lines up precisely).
- The Straight/Over/P.T./R.T cells use the same "dropdown -> large text" behavior as the Acrobat version.
- The No Lunch column cells are click-to-toggle "0.5".
- A top toolbar provides:
  - Reset (clears the form back to blank / dropdown state)
  - Print / Save PDF (opens the browser print dialog)

How to run
Option A (recommended): run a tiny local web server
1) Open a terminal in this folder
2) Run:
   python -m http.server 8000
3) Open:
   http://localhost:8000

Option B: host on GitHub Pages (static hosting)
- Upload these files to a GitHub repo (index.html, app.js, style.css, fields.json, dwl_page1.png)
- Enable GitHub Pages (Deploy from branch, root folder)

Notes
- "Print / Save PDF" uses the browser print dialog. On desktop Chrome/Edge, choose Destination: Save as PDF.
- The background is an image (not a CSS background), so it prints reliably.
