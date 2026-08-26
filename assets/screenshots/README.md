# Screenshots for the carousel

Drop the extension screenshots here. The autoplay carousel on the landing
page (`index.html`) reads this exact list — filename order = display order:

| File                    | Suggested shot                                        |
|-------------------------|-------------------------------------------------------|
| `01-week.png`           | A doctor's whole week in one calendar                 |
| `02-compare.png`        | Two/three doctors compared side by side               |
| `03-available.png`      | "Available only" toggle on — full slots hidden        |
| `04-details.png`        | Patient details / settings, pre-filled                |
| `05-checkout.png`       | Hand-off to eChannelling's official checkout          |

## Rules
- **Size:** 1600×1000 (16:10). The frame crops to 16:10 from the top.
- **Weight:** keep each under ~400 KB (PNG or JPG). Run through TinyPNG/`sips` if larger.
- **Missing files are safe:** any shot that isn't present yet shows a neutral
  "add assets/screenshots/NN-name.png" placeholder — the page never shows a
  broken image.

To add, remove, or reorder shots, edit the `SHOTS` array near the bottom of
`../../index.html`.

### Quick resize (macOS)
```sh
sips -Z 1600 raw.png --out 01-week.png     # cap long edge at 1600px
```
