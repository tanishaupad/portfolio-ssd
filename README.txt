# SSD Assignment 2 — Portfolio (Tanisha Upadhyay)

This repository contains a small portfolio + assignment demos for CS6.302 (Software System Development, Monsoon 2025). It includes interactive web demos (jigsaw puzzle, Stoplight game, data-dictionary generator, 3D bowling) and a small tracking utility.

Live demos
- Q1: https://tanishaupad.github.io/portfolio-ssd/  
- Q2: https://tanishaupad.github.io/portfolio-ssd/newssd.html  
- Q3: https://tanishaupad.github.io/portfolio-ssd/Q3/jigsaw.html  
- Q4: https://tanishaupad.github.io/portfolio-ssd/Q4/nash.html  
- Q5: https://tanishaupad.github.io/portfolio-ssd/Q5/data_dict.html  
- Q7: https://tanishaupad.github.io/portfolio-ssd/Q7/bowling.html

Files
- [index.html](index.html) — personal profile page with photo [IMG_20250712_092117_032.webp](IMG_20250712_092117_032.webp)  
- [newssd.html](newssd.html) — course site / syllabus (CS6.302)  
-  Q6: [track.js](track.js) — small event tracker that logs clicks & views to the console  
- [Q3/jigsaw.html](Q3/jigsaw.html) — Jigsaw puzzle demo (image slicing + drag/drop)  
- [Q4/nash.html](Q4/nash.html) — Stoplight game (Nash equilibrium demo)  
- [Q5/data_dict.html](Q5/data_dict.html) — Data Dictionary generator + preview / export  
- [Q7/bowling.html](Q7/bowling.html) — 3D bowling demo (Three.js)  
- [README.txt](README.txt) — original assignment README notes

Key functions / symbols (quick reference)
- [`getTimestamp`](track.js) — timestamp helper in [track.js](track.js)  
- [`logEvent`](track.js) — logs click/view events to console in [track.js](track.js)  
- [`findGrid`](Q3/jigsaw.html) — compute rows/cols for puzzle in [Q3/jigsaw.html](Q3/jigsaw.html)  
- [`startPuzzle`](Q3/jigsaw.html) — build slices & shuffle in [Q3/jigsaw.html](Q3/jigsaw.html)  
- [`renderBoard`](Q3/jigsaw.html), [`placePieceInSlot`](Q3/jigsaw.html), [`checkComplete`](Q3/jigsaw.html) — puzzle UI handlers in [Q3/jigsaw.html](Q3/jigsaw.html)  
- [`setHumanChoice`](Q4/nash.html), [`randomizeHuman`](Q4/nash.html), [`randomizeComputer`](Q4/nash.html), [`calculatePayoffs`](Q4/nash.html), [`playGame`](Q4/nash.html), [`resetGame`](Q4/nash.html) — game logic in [Q4/nash.html](Q4/nash.html)  
- [`loadExample`](Q5/data_dict.html), [`generateDictionary`](Q5/data_dict.html), [`downloadHTML`](Q5/data_dict.html), [`downloadPDF`](Q5/data_dict.html) — data-dictionary UI & export in [Q5/data_dict.html](Q5/data_dict.html)  
- [`createPin`](Q7/bowling.html), [`setupPins`](Q7/bowling.html), [`handleRollComplete`](Q7/bowling.html), [`calculateScore`](Q7/bowling.html), [`animate`](Q7/bowling.html) — bowling mechanics in [Q7/bowling.html](Q7/bowling.html)

Quick start (local)
1. Serve the folder over HTTP (recommended) and open the pages in a browser:
   - Python 3: `python3 -m http.server 8000`
   - Open: http://localhost:8000/index.html or http://localhost:8000/newssd.html
2. To see event tracking, open DevTools → Console. The tracker prints events from [`track.js`](track.js).

Notes
- The tracker [`logEvent`](track.js) prints click and "view" (IntersectionObserver) events to the console — useful to inspect user interactions on the demos.
- The data-dictionary tool in [Q5/data_dict.html](Q5/data_dict.html) generates printable HTML and PDF exports.
- The bowling demo uses Three.js (included via CDN) and is best viewed on a desktop browser.

Author
- Tanisha Upadhyay — 2025201088, campus profile and CV referenced in [index.html](index.html) and [README.txt](README.txt).

License
- Refer to repository owner for license / usage terms.
