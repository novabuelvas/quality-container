# Quality Container

A cinematic website for Quality Container, with corrugated packaging imagery, an opening-box animation controlled by scrolling, responsive layouts, and a two-step quote form.

## Preview locally

This is a static site. No build or dependencies are required.

```sh
python3 -m http.server 4173
```

Open http://localhost:4173.

## Publish with GitHub Pages

In repository **Settings → Pages**, choose **Deploy from a branch**, select **main** and **/ (root)**, and save. The relative asset paths support a GitHub project-site URL.

## Quote requests

The form sends requests to **alex@micro-printing.com** through FormSubmit. The recipient must complete FormSubmit’s one-time email activation. Email delivery has not been verified end to end. A direct email fallback is included if a submission cannot be confirmed.

## Motion

The opening uses 121 locally hosted JPEG frames drawn to a canvas, avoiding video-seeking problems. It respects the visitor’s reduced-motion preference and includes a pause control. Scroll down and back up to open and close the box.

## Files

- `index.html` — page content and quote form
- `styles.css`, `cinema.css` — base and cinematic styles
- `app.js` — navigation and form behavior
- `cinema.js` — opening animation and scroll transitions
- `assets/` — local imagery, animation frames, and fonts
- `privacy.html` — form-data and privacy information

This export excludes private hosting configuration, credentials, and unrelated workspace files.
