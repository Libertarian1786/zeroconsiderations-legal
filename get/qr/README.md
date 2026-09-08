# Zero Considerations — venue QR codes

Generated with Python `qrcode` (error correction **M**, quiet zone **4 modules**), PNG
rendered at **1024×1024 px**. Each PNG was round-tripped through `pyzbar` to confirm it
decodes back to the exact URL below before this file was committed. SVG files carry the
same parameters as scalable vector art (`width`/`height` set to 1024 for a predictable
default render size; the `viewBox` keeps them crisp at any size).

Every code points at a `/get/<venue>/` folder on this site, not a query string — the
folder is the mutable layer, so the destination (store links, attribution tags) can change
without ever reprinting a code. See `50_website_seo.md` §8 and `80_remote_playbook.md` §0.2
in the marketing program for why.

| Venue | File | URL |
|---|---|---|
| `targets` | `zc_qr_targets.png` / `.svg` | https://zeroconsiderations.com/get/targets/ |
| `range` | `zc_qr_range.png` / `.svg` | https://zeroconsiderations.com/get/range/ |
| `club` | `zc_qr_club.png` / `.svg` | https://zeroconsiderations.com/get/club/ |
| `counter` | `zc_qr_counter.png` / `.svg` | https://zeroconsiderations.com/get/counter/ |
| `pdf` | `zc_qr_pdf.png` / `.svg` | https://zeroconsiderations.com/get/pdf/ |
| `results` | `zc_qr_results.png` / `.svg` | https://zeroconsiderations.com/get/results/ |
| `card` | `zc_qr_card.png` / `.svg` | https://zeroconsiderations.com/get/card/ |

Each `/get/<venue>/` page routes Android to the Play `qr_target` custom listing with
`referrer=utm_source%3Drange%26utm_medium%3Dqr%26utm_campaign%3Dtargets_fall26%26utm_content%3D<venue>`,
and iOS to `https://apps.apple.com/app/id6792565250?ct=<venue>&mt=8`. The iOS `ct` value is
a placeholder until a real App Store Connect campaign link (with its `pt` provider token)
exists per `80_remote_playbook.md` W1.8 — swap it in per venue once minted, the same way a
`/get/<venue>/` folder is edited in place rather than reprinted.

`targets` is the venue embedded directly on the free printable targets page
(`/targets/`); the rest are free for print runs, club days, counter displays, exported
PDF reports and the app's own results screen as those materials are produced.
