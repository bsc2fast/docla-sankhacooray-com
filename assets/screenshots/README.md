# Screenshots for the carousel

Each shot exists twice, in `dark/` and `light/`; the landing page shows the set
that matches its current theme. Captured from the real extension (Chrome for
Testing + puppeteer, extension loaded unpacked) at **1600×1000**, with
obviously fictional demo patients/bookings seeded into `chrome.storage.local`.

| File                  | Shot                                                  |
|-----------------------|-------------------------------------------------------|
| `02-search.png`       | Search: three columns, Nawaloka + Cardiologist ticked |
| `03-calendar.png`     | Calendar: three doctors, colour-coded, all hospitals  |
| `05-appointments.png` | My appointments (demo bookings)                       |
| `06-settings.png`     | Settings → Patients (demo patients, default starred)  |
| `07-status.png`       | Settings → Status self test                           |

To add, remove, or reorder shots, edit the `SHOTS` array near the bottom of
`../../index.html`.
