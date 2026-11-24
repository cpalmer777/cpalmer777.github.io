# Book cover camera

Open https://cpalmer777.github.io/ on a phone (the QR code in `assets/qr.png` points there). Tap **Start camera**, then hold the physical book cover in frame. `assets/cert.jpg` is the compiled key (`assets/cert.mind`). When the camera sees that cover, `assets/book.mp4` plays on top of it and pauses when the cover leaves the frame.

This is a static site. `index.html` stays at the repository root. Runtime files live in `assets/` and are referenced with paths relative to the page, so they resolve on `https://cpalmer777.github.io/` and also if the site is later served from a subpath. `.nojekyll` tells GitHub Pages to publish `cert.mind` and `book.mp4` unchanged.

Local preview: `npx http-server . -p 8090` and open the page on a phone on the same network. The camera needs HTTPS or localhost.
