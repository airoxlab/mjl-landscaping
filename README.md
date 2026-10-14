# MJL Landscaping — Pittsburg, CA

Single-page sample site for a licensed C-27 landscaping contractor in Pittsburg,
California (East Contra Costa County). Built as a free sample for an SMS lead who
already has a website "in the works".

## Business details

| | |
|---|---|
| Business | MJL Landscaping |
| Owner | **Not public** — ask him (the initials suggest a personal name) |
| Phone | (925) 787-2220 (mobile — call and text both offered) |
| Email | mjlandscape781@gmail.com |
| Location shown | Pittsburg, CA |
| Website | None — "Not yet, we are working on it" |
| Google Maps | **Not listed** |

## Licence — verified twice

Checked against the CSLB database on **2026-10-14**, licence **#1107968**:

- **MJL LANDSCAPING**, 1107 Bending Willow Way, Pittsburg, CA 94565
- Business phone (925) 787-2220 — matches the number he was texted on
- Issued **08/01/2023**, expires **08/31/2027**
- **This licence is current and active.**
- Classification **C-27 — Landscaping**
- Contractor's bond with **Merchants Bonding Company (Mutual)**, **$25,000**,
  effective 07/11/2025
- **Workers' compensation** with National Specialty Insurance Company,
  policy #NXTD99YQ7P00WC, effective 02/05/2026 to **02/05/2027**

He carries real workers' comp, so he has a crew, and the site says
**"licensed, bonded and insured"**.

### A conflict worth knowing about

A third-party site, **contractorlicenseca.com, describes him as a "Suspended
Landscaping Contractor"**. That is **out of date**. CSLB — the authoritative
source — was queried twice and both times returned *"This license is current and
active."*

The likely explanation is visible in the dates: his bond took effect 07/11/2025
and his current comp policy 02/05/2026. He was probably suspended briefly before
those filings, and the scraper never refreshed.

**The site's "active" claim is correct**, but if a customer ever raises it, the
answer is the CSLB page itself. Worth mentioning to him — he may not know a
directory is publishing that about his business.

## What was deliberately not built

- **No reviews or testimonials.** His Yelp listing exists but has few or no
  reviews, BBB blocked direct access (Cloudflare), and MapQuest returned an
  unrelated business in the Netherlands. Nothing verifiable to quote.
- **No BuildZoom score or BBB rating.** The brief cites BuildZoom 93 / top 27%
  and BBB B+, but neither could be loaded first-hand (BuildZoom is geo-blocked
  from this machine, BBB blocked the request). Not claimed on the site.
- **No owner name.** Not published anywhere.
- **No street address.** 1107 Bending Willow Way is residential; the site shows
  "Pittsburg, CA" and a service area.
- **"Licensed since 2023" is used** — that one is straight from CSLB and is a
  genuine advantage over the newer contractors in this collection.

## Images

`img/` — five stock photos (Unsplash). He has no photos of his own online.
Disclosed under the gallery and in the footer.

Two stock candidates were discarded for showing the wrong subject (a living room
labelled "patio", and call-centre staff labelled "backyard").

**Job photos are the biggest single upgrade available.**

## The estimate form

His competitors on Google Maps take online bookings, so the site has a proper
estimate form rather than just a phone number. On submit it builds a pre-filled
**email** to mjlandscape781@gmail.com with name, phone, city, job type and
details, and prompts the visitor to attach a photo.

Email rather than SMS here (All Pacific Roofing uses SMS) because he has a
published business email and landscaping enquiries are less urgent than a roof
leak — but the form also tells people they can text photos to his mobile.

**Tested functionally in a browser:**

| Test | Result |
|---|---|
| Submit with empty fields | Rejected — "Please add your name and a phone number." |
| Honeypot field filled (bot) | Silently accepted, nothing sent |
| Valid submission | Correct `mailto:` with subject and all fields formatted |
| JS errors | None |

## Design

Deliberately distinct from Valencia Landscaping, the other C-27 site in this
collection (maroon and lettuce green, bilingual):

- Deep pine `#11261D` navbar and bands, fern green `#2E7D52`, harvest gold
  `#D9A021` on a cool off-white.
- Outfit (display) + Source Sans 3 (body).
- Inline SVG two-leaf roundel.
- Nine sections: hero, credential strip, services, residential/commercial band,
  process, licensing, work gallery, service areas, estimate form, contact.
- Full dark mode, sticky header, `scroll-margin-top` anchors, reduced-motion
  respected, inline CSS, no build step.
- Sendra visit-tracking script before `</body>`.

## Open questions for the client

1. **His first name** — "MJL" reads like initials.
2. **Job photos.**
3. **Residential or commercial focus** — which does he want more of?
4. **Does the site he is building already have a domain?** If so, this can point
   at it rather than starting over.
5. **Is he aware** a directory lists his licence as suspended? (See above.)

## The name problem

There is a **"MJ Landscaping" / "MJ Landscaping Inc" in the same town**
(122 Alberts Ave and 640 Bailey Rd, Pittsburg) — a different business with a
near-identical name. Customers searching for MJL can easily land there.

He also has **no Google listing at all**. A search for "MJL Landscaping
Pittsburg" returns competitors instead: Unified Landscape Management (4.9★, takes
online bookings), J & M Landscape (5.0★) and Mike McCall Landscape (3.1★).

So two rivals are being handed his traffic: one by name similarity, the others by
map presence. **A verified Google Business Profile is the highest-value next
step**, and he has the licence history (2023) and insurance to look stronger than
most once he is listed.
