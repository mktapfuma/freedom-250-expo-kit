---
title: "Freedom 250 expo — the local print order for Saturday 31 October: what to ask for, where, what it costs, and what to do if only one thing gets printed"
tags: [cmo, expo, harare, print, order, samday, freedom-250]
status: draft
created: 2026-10-30
owner: "Chiedza Marufu (CMO lane)"
responds_to: "Founder DM event a778d47d7a4a538219eaa996467c019176925fe3331409302aebc8631df7d3d8 (2026-10-30T04:36:20Z): 'Lets finalise the artwork. We need both Moses K Tapfuma and KTA Solutions graphics'"
measurement_instant: "2026-10-30 (digests measured by the CMO lane on its own host; vendor prices read from the vendors' own published pages on 2026-10-30)"
---

# The print order — Saturday 31 October, printed locally in Harare

**What this is.** One page Angeline can act on **today or first thing tomorrow**, with
the artwork already made, the sizes already matched to products that are on sale in
Harare, and the prices already published.

**What this is not.** It is not an order, and it buys nothing. **Nothing is printed until
the Founder approves the spend line by line** (B4: a US$900 cap, no purchase without his
line-item approval). The safe default if he says nothing stands: **nothing is bought,
nothing is printed, nothing is sent.**

---

## 1 · Why local and not the hosted print run

**The hosted deadlines have passed, and this changes the route, not the ambition.**

| what | when it was | state today (30 Oct) |
|---|---|---|
| RFQ quotes due | 28 Oct | passed |
| Artwork to the print host | 29 Oct 10:00 | **passed** |
| Delivery to the venue | 30 Oct | today |
| **Event** | **Sat 31 Oct, 09:00–13:00** | **tomorrow** |

A vendor asked to quote on 28 October and receive artwork on 29 October cannot be
guaranteed a Friday delivery for a Saturday morning event, and we have no quote on file.
**But Harare has same-day printing with published prices**, and our artwork sizes match
those products exactly. So the route is now: **print locally, tomorrow morning, from
artwork that already exists.**

## 2 · What to ask for, at what size, at what published price

All prices below are **published by the vendor on their own page, read 30 October 2026**,
and are stated in USD as the vendor states them.

| # | item | spec | where | published price |
|---|---|---|---|---|
| **P1** | **Executive roll-up banner, 2 m × 0.85 m** — printing + frame, **same-day service** | our file `PULLUP_850x2000mm.pdf` | Vineflex Visual Graphics, Harare CBD — WhatsApp +263 77 715 0441 | **US$75–80** (two published posts: US$75 and US$80) |
| **P2** | **X-frame banner, 180 cm × 80 cm** — printing + frame, same-day | our file `TABLE_BANNER_1x2m.pdf` (cropped to 180 × 80 cm if they prefer) | same vendor | **US$23–25** |
| **P3** | **A5 flyers, 100 copies, double-sided, full colour** | our files `A5_FLYER_FRONT` + `A5_FLYER_BACK` | any Harare print shop | **ask for a same-day quote** — no published price found |
| **P4** | **A6 cards, 20 copies, laminated, rounded** | our file `A6_CARD_105x148mm.pdf` | same | **ask for a same-day quote** |

**The fallback if only one thing gets printed: P1, the roll-up.** It is the piece a
visitor sees from across the room, it carries all three QR codes, and it is the only
item with a published same-day price. Everything else is nice-to-have. **A table with a
pull-up, a laptop and a QR card beats a table with nothing.**

**Second fallback, if even the roll-up is refused:** print **the A5 flyer (P3)** — it
carries the same three QR codes and the same call to action, and it is the thing a
visitor takes away.

## 3 · The copy-paste message for the vendor

> Hi, I need printing for **tomorrow morning** (Saturday 31 October), for an event in
> Milton Park. Same-day service if possible.
>
> 1. **One executive roll-up banner, 2 m × 0.85 m**, full colour, printing + frame. I
>    will supply the artwork as a print-ready PDF.
> 2. **Optional:** one X-frame banner, 180 cm × 80 cm, full colour, printing + frame.
> 3. **Optional:** 100 A5 flyers, double-sided, full colour; and 20 A6 cards, laminated
>    with rounded corners.
>
> Please quote each item separately, state the latest time you can have them ready
> **before 09:00 tomorrow**, and confirm whether you can accept the artwork files by
> WhatsApp email.
>
> Thank you — Angeline Tapfuma, sending this for Moses K Tapfuma.

**One thing to check before they print:** the RFQ asked for a **3 mm bleed**, and our
artwork has it. Ask them to print **"full bleed, no scaling"** — a printer who scales to
fit will shrink the type and can clip the edge.

## 4 · The artwork, and how it gets to them

**Six print-ready files, already made and already checked.** Each is a PNG and a PDF of
the same artwork, at the right physical size with a 3 mm bleed, and each carries its own
digest in the manifest.

| file | size | what it is |
|---|---|---|
| `PULLUP_850x2000mm` | 850 × 2000 mm, 150 dpi | **P1** — the roll-up banner, dark ground, three QR codes |
| `TABLE_BANNER_1x2m` | 1000 × 2000 mm, 150 dpi | **P2** — the table-front banner (or the X-frame, cropped) |
| `BACKDROP_2x3m` | 2000 × 3000 mm, 150 dpi | the 2 m × 3 m pop-up backdrop, **only if a wall is confirmed** |
| `A5_FLYER_FRONT` / `A5_FLYER_BACK` | 148 × 210 mm, 300 dpi | **P3** — the flyer, both sides |
| `A6_CARD_105x148mm` | 105 × 148 mm, 300 dpi | **P4** — the leave-behind card |

**Where they are:** `OUTBOX/FREEDOM_250_EXPO_ARTWORK_2026_10_30/` on the Founder's
machine, with `MANIFEST.json` carrying every file's bytes and sha256, and
`VERIFY_RECEIPT_20261030T050317Z.json` carrying the verification.

**How they get to Harare — the constraint, stated plainly.** The relay's media host
**accepts images only**: a `.pptx` was refused as a zip container and a `.pdf` was refused
as a type on this project. So the **PNGs can travel over Buzz**; the PDFs cannot. The
PNGs are print-resolution, so **the PNG is a legitimate print file** — send the PNG if
the channel is WhatsApp or email, and the PDF if you can hand over a file directly.

**One thing to tell the printer, because it matters.** The relay's media store
**rejects PNG files carrying metadata**, so the copies that travel over Buzz are
**pixel-identical to the print files with the DPI chunk stripped** (measured: every
transport copy's pixel array is byte-for-byte equal to its source). **A PNG without a DPI
chunk can be interpreted at 72 dpi, which would make the pull-up 1.8 m wide instead of
0.85 m.** So either hand over the **PDF** from the artwork folder — which carries the
physical size — or give the printer this table and the pixel dimensions:

| file | pixel dimensions | print at exactly |
|---|---|---|
| `PULLUP_850x2000mm` | 5056 × 11 847 px | **850 × 2000 mm** (0.85 m × 2 m) |
| `TABLE_BANNER_1x2m` | 5942 × 11 847 px | **1000 × 2000 mm** (1 m × 2 m) |
| `BACKDROP_2x3m` | 11 847 × 17 753 px | **2000 × 3000 mm** (2 m × 3 m) |
| `A5_FLYER_FRONT` / `_BACK` | 1818 × 2550 px | **148 × 210 mm** (A5) |
| `A6_CARD_105x148mm` | 1310 × 1818 px | **105 × 148 mm** (A6) |

**And tell them: "full bleed, no scaling"** — 3 mm bleed is already in the files, and a
printer who scales to fit shrinks the type and clips the edge.

## 5 · What is on the artwork, and what is deliberately not

**On it:** the approved Moses K Tapfuma mark and wordmark; the three approved QR
destinations (site, writing, LinkedIn); the six published service lines; the call to
action that is already in the leave-behind card copy; and a **KTA Solutions** lockup.

**The KTA Solutions lockup is provisional and needs the Founder's eye.** The KTA logo
files live in the 2024 Drive folder and are **not on this host**, so what is on the
artwork is **type, set in the KTA palette recorded in the brand register** (Black Pearl
`#04041C`, Eucalyptus `#248056`) — not the actual KTA logo. **If he wants the real logo
on the artwork, he sends the file and it is swapped in; that is a five-minute change and
a rebuild, and it must happen before printing, not after.**

**Deliberately not on it:** no price, rate, package or discount; no client, partner or
vendor logo; no claim of Zimbabwe presence, delivery, local staff or local clients; **no
phone number** (the card carries a ruled blank the Founder writes by hand); and no
attendee-count or room-size claim.

**One line to check before printing.** The flyer and the card say **"Not yet serving
clients inside Zimbabwe — here to start that, properly."** With Angeline now the
Founder's interim COO for KTA Solutions in Zimbabwe, **that sentence is the honest one
and should stay** — it claims a beginning, not a presence. If he wants a different line,
it is one edit and one rebuild.

## 6 · The money, against the cap he approved

**Cap: US$900 total, one traveller, no contractor build, no paid extras, nothing bought
without his line-item approval.**

| line | USD | class |
|---|---:|---|
| P1 roll-up banner | 75–80 | **published price** |
| P2 X-frame banner | 23–25 | **published price** |
| P3 A5 flyers ×100, double-sided | 10–35 | **ESTIMATE** from a weak published per-page rate |
| P4 A6 cards ×20, laminated | 10–25 | **ESTIMATE** |
| Data for two devices | 18–26 | published bundle prices |
| Day cash: airtime, taxis, water | 40–60 | ESTIMATE |
| **Print + day subtotal** | **≈ 176–251** | |
| Travel — the Founder drives | see the revised budget | the Founder's own vehicle, no flight, no hotel, no insurance |
| **Contingency (10%)** | ≈ 18–25 | rule, not a measurement |
| **TOTAL if the Founder drives** | **≈ 200–280** | **well inside the US$900 cap** |

**The cap is not the constraint any more — the clock is.** The US$900 was sized around a
flight and a hotel; with him driving and staying with family, **the whole event now
costs roughly a quarter of the cap**, and the remaining risk is entirely on the print
and the furniture questions (B2), not on money.

## 7 · What is still open, and who owns it

| # | open | owner | by when |
|---|---|---|---|
| 1 | **Approve the print spend line by line** — P1 at minimum | Founder | **today** |
| 2 | **The KTA logo file**, if he wants the real logo on the artwork rather than the type lockup | Founder | before printing |
| 3 | **B2 — does the invitation's table come with furniture, power and a banner-hanging point?** and whether the venue's own market stall is rentable | Founder / Angeline, with the organiser | today |
| 4 | **Send the RFQ / local print request** (B3 — Angeline) | Angeline | today |
| 5 | **The brief is R6, and it is unsigned** — the Head of Content and Presence's byte sign-off on the pinned pair is still open, and the pin moved to R8 with it | Head of Content and Presence | today, or the printed card is knowingly accepted as unsigned |
| 6 | **The Founder's approval of the brief** and of the card words | Founder | today |

**Owner of this document:** CMO lane. **Next safe step from me:** the artwork is done and
verified; the byte sign-off request for the R6 pair goes out today; and the spend
decision is one line from the Founder.

**Cash $0 — nothing printed, nothing ordered, no vendor contacted, nothing sent.**
