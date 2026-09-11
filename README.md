# Doctor Lanka — landing page

The public product page for **Doctor Lanka**, a free Chrome extension that puts a
fast weekly calendar over Sri Lanka's [eChannelling](https://www.echannelling.com).
Compare doctors, hospitals and times at a glance — then check out on the official
site as usual.

**Live:** https://docla.sankhacooray.com/ (privacy policy: https://docla.sankhacooray.com/privacy)

This repo is just the marketing/landing page (a single static `index.html`). The
extension itself lives separately.

## What Doctor Lanka does

- **The whole week at a glance** — search a doctor and see every session across the
  week in one calendar, instead of paging one day at a time.
- **Compare doctors side by side** — add more than one doctor and find the times
  they share a hospital and a day.
- **Hide full sessions** — one toggle drops sold-out slots so what's left is bookable.
- **Look up a booking** — paste a reference number or summary URL to pull the receipt.
- **Pre-filled patient details** — name / NIC / mobile / email saved locally and
  filled into the booking form.
- **Official checkout** — you pick the slot here; payment finishes on echannelling.com.

## Install

Doctor Lanka is distributed as an unpacked Chrome extension.

1. **Unzip** the `doctor-lanka.zip` you were sent — you'll get a `doctor-lanka` folder.
   Move it somewhere permanent (e.g. Documents) and don't delete it.
2. Open Chrome and go to `chrome://extensions`.
3. Turn **on** *Developer mode* (top-right).
4. Click **Load unpacked** and choose the `doctor-lanka` folder.
5. Pin it (🧩 → 📌) and click the toolbar icon to open the calendar.

No account and no configuration needed. Payment always happens on echannelling.com.

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

Doctor Lanka is an independent helper for the public eChannelling website and is
not affiliated with, endorsed by, or operated by eChannelling PLC.
