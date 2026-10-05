# twincue.app

The website for [Twincue](https://twincue.app), a teleprompter for iPhone that shows the
script next to the camera while you record. Served by GitHub Pages from `main`.

- `index.html` is the home page: icon, tagline, App Store badge.
- `privacy/` and `terms/` are the privacy policy and the terms. The app and its store listing
  link to these two addresses. Their source is `docs/legal/` in the app repository: change the
  text there first, then here.
- `support/` is the support page with the contact address. The store listing's Support URL
  points to it.
- `404.html` is the page GitHub Pages serves for any other address.

## The OG image

`assets/og.jpg` is rendered by Chrome from `build/og.html`:

```bash
"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" --headless=new --hide-scrollbars \
  --force-device-scale-factor=1 --window-size=1200,630 \
  --screenshot=build/og.png "file://$PWD/build/og.html"
```

then converted to JPEG at quality 88 and `build/og.png` deleted. The icon beside it,
`build/icon-1024.png`, is `docs/design/icon-previews/default-27.png` from the app repository.
