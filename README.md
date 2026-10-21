# DocLa — landing page

The public product page for **DocLa** (formerly Doctor Lanka), a free Chrome
extension for Sri Lanka's [eChannelling](https://www.echannelling.com).
Find a doctor by hospital, doctor or specialty, compare a week of sessions,
then check out on the official site as usual.

**Live:** https://docla.sankhacooray.com/ (privacy policy: https://docla.sankhacooray.com/privacy)

This repo is just the marketing/landing page (a single static `index.html`). The
extension itself lives in `../docla-sankhacooray-mv3`.

## What DocLa does

- **Search three ways** — hospital first, doctor first or specialty first; each
  column narrows the other two. Favourites (star) stay on top.
- **Three doctors, one week** — up to three doctors on one calendar, one colour
  each, with your picked hospitals first and their others one tick away.
- **Common time finder** — slots where every picked doctor sits at the same
  hospital on the same day.
- **My appointments** — bookings saved from the confirmation page or a lookup,
  with receipt and official PDF.
- **Patients** — several saved patients; the default one is filled into the
  booking form, others one click away.
- **Look up a booking**, **live connection check**, and **official checkout**.

## Install

From the [Chrome Web Store](https://chromewebstore.google.com/detail/mffhilimciffjoeghenlopeehocimanh).
No account and no configuration needed. Payment always happens on echannelling.com.

## Share image

`assets/og-image.png` is rendered from `og/og.html` at 1200×630 with headless
Chrome. After changing it, bump `?v=N` on `og:image` / `twitter:image` in
`index.html` so WhatsApp and others refetch.

## Develop / preview

```sh
python3 -m http.server 4655   # then open http://localhost:4655
```

## Deploy

Served at **docla.sankhacooray.com** by a Cloudflare **static-assets Worker** named
`docla` (config in `wrangler.toml`). Redeploy with:

```sh
npx wrangler deploy
```

No build step. (The old GitHub Pages copy at `bsc2fast.github.io/doctor-lanka-web`
is retired.)

## Not affiliated

DocLa is an independent helper for the public eChannelling website and is
not affiliated with, endorsed by, or operated by eChannelling PLC.
