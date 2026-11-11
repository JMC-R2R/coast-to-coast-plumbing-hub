# Coast to Coast Plumbing: location page writer notes

**Layout:** Divi "blocked drains, suburb" location page (theme builder header and footer, Divi sections, Contact Form 7 quote form, Trustindex Google reviews).
**Source pages (captured 11 Nov 2026):**
- https://coasttocoastplumbingmp.com.au/blocked-drains-blairgowrie/
- https://coasttocoastplumbingmp.com.au/blocked-drains-somers/

Both pages use the identical template. Only the hero heading and intro, the intro photo, four section headings, the steps copy and the FAQ change from suburb to suburb. Everything else is the same on every page and is copied verbatim in `skeleton.html`.

**Pages this template is for:** Plumber Aspendale, Plumber Chelsea, Plumber Parkdale, at URLs like `/blocked-drains-aspendale/`. The URL and the template are blocked drain pages, so lead with blocked drains and work "plumber in [Suburb]" in naturally (the live pages already say "our plumber in Blairgowrie"). Title tag pattern on the live site: `Blocked Drain Plumber in [Suburb] | Coast to Coast Plumbing`. Meta description pattern: `We clear blocked drains in [Suburb] with CCTV inspections, drain cleaning and pipe repair options. Contact our team to arrange a visit or request a quote.`

## Section by section

Fill only the `{{...}}` slots. Do not add, remove or reorder sections. Exactly one `<h1>`. No inline style attributes.

| # | Section | Class | Variable? | What to write |
|---|---|---|---|---|
| 1 | Hero: dark photo, H1, short intro, white phone pill, quote form card | `pg-hero cc-hero` | H1 and hero paragraph only | **H1**, 5 to 10 words, keyword plus suburb at the end. Live: "Drain Cleaning and Blocked Drain Repairs in Blairgowrie", "Blocked Drain Clearing and Pipe Repairs in Somers". **Hero P**, 20 to 30 words, one or two sentences: who we help in the suburb, what we do (blocked drains, inspections, repairs), then "Contact us to..." Background photo, phone button and form are fixed. |
| 2 | Google Reviews | `cc-sec` | No | Fixed: "EXCELLENT, Based on 16 reviews" plus four real Google reviews. Never edit or add reviews. |
| 3 | Intro: rounded photo left, H2 and two paragraphs right | `cc-sec cc-grey` / `cc-intro` | Yes | **Photo:** one client library photo of a drain, stormwater or pipework job (portrait or square works best; it is cropped to 600px tall with 100px rounded corners). Plain, descriptive alt text. **H2**, 6 to 10 words, e.g. "Clearing Blocked Drains for [Suburb] Homes and Businesses", "Drain Cleaning for [Suburb] Homes and Businesses". **P1**, 50 to 65 words: open with the customer's real problem (a drain that clears and then backs up, a sink that will not empty), then say we clear blocked drains in [Suburb] for households and businesses and name the drains (kitchen, bathroom, sewer, stormwater). **P2**, 40 to 55 words: CCTV inspections where needed, high-pressure jetting for suitable pipework, we explain repair or relining options, close with "Speak with / Contact our plumber in [Suburb] to ... arrange a visit and request a quote." |
| 4 | Why choose: 3 + 2 dark cards with white icons | `cc-why` | H2 only | **H2**, a question, 7 to 10 words: "Why Choose Our [Suburb] Plumbers for Drain Clearing?" / "Why Book Our [Suburb] Plumbers for Drain Cleaning?" The five cards are fixed copy. |
| 5 | Services grid: 16 black cards with icons | `cc-sec cc-grey` / `cc-svc` | H2 only | **H2**, 6 to 9 words: "Our Plumbing and Drainage Services in [Suburb]" / "Our Plumbing Services for [Suburb] Homes and Businesses". The 16 cards are fixed copy. |
| 6 | Steps: H2, one-line intro, three round icon pods | `cc-pods` | Yes (except the three pod titles) | **H2**, 6 to 9 words, process framing, suburb optional: "Our Steps for Inspecting, Clearing and Repairing Drains", "Our Approach to Drain Inspections, Cleaning and Repairs". **Intro P**, one sentence, 14 to 20 words. **Pod texts**, one sentence each, 14 to 18 words, under the fixed titles "CCTV Camera Diagnosis", "High-pressure Jetting", "Repair or Relining". |
| 7 | "Looking for Stress-Free Plumbing Solutions?" CTA band, then "Areas we serve" pill grid | `cc-cta`, `cc-areas` | No | Fixed copy and the 29 live suburb links. Do not add the new suburb to the grid. |
| 8 | Contact block (Call Us, Email Us, Area We Serve) with second quote form, Google map, FAQ | `cc-contact`, `cc-map`, `cc-faq` | FAQ only | FAQ heading "Frequently Asked Questions About Plumbing" is fixed. **Exactly 5 Q and A.** First item stays `open`. Questions 8 to 14 words, phrased as a customer would ask; at least two name the suburb. Answers 40 to 50 words, three sentences, starting with "We..." most of the time. Cover: a recurring blockage, sewer vs stormwater or a specific fixture, urgent or after-hours help, how pricing is worked out (no dollar figures), and repair, relining or excavation. |

**Variable word count:** about 480 to 560 words (hero 30, intro 110, steps 65, FAQ 300, headings). With fixed copy the page renders at roughly 1,250 words.

**Tone seen on the live pages:** plain, practical and calm. First person plural ("We clear...", "We explain..."). Short declarative sentences, cautious wording ("where needed", "suitable pipework", "where appropriate", "we discuss the available options"). No hype, no superlatives, no prices, no time promises. Australian English (localised, prioritise, centre). No em or en dashes, no Oxford comma.

## Fixed copy (never rewrite)
Hero background photo, phone pill, both quote forms (field labels exactly as on the site), Google Reviews block, the five Why Choose cards, the 16 service cards, the three step titles and the jetting photo, the Stress-Free CTA band, Areas we serve heading, intro line and 29 links, the contact block and map, the FAQ heading, header and footer.

Note: the service card "Hot Water Problems &ndash; Electric, Gas &amp; Solar" contains an en dash on the live site. It is the client's own fixed copy and is kept verbatim; never introduce dashes in the copy you write.

## Facts the client's own site states (only these may be reused)
| Fact | Verbatim wording | Where it appears |
|---|---|---|
| Phone | 0437 094 448 (link `tel:0437094448`) | Header, hero, CTA, contact block and footer on both source pages |
| Email | ben@coasttocoastplumbing.com.au | Contact block and footer, both source pages |
| Experience | "With over 20 years of industry experience, we deliver dependable plumbing and gas fitting solutions backed by quality workmanship and responsive support." | Footer, every page (e.g. /blocked-drains-blairgowrie/) |
| Experience (home) | "Over 20 Years Of Experience", "Locally Owned", "24/7 Emergency Service" | https://coasttocoastplumbingmp.com.au/ |
| 24/7 | "We provide 24/7 emergency plumbing support in Blairgowrie for urgent problems, including serious blockages and overflowing toilets." | FAQ, /blocked-drains-blairgowrie/ |
| Licensed and insured | "Every one of our plumbers and gas fitters is fully licensed, insured, and exceptionally skilled." | FAQ, https://coasttocoastplumbingmp.com.au/ |
| Licensed plumbers | "our licensed plumbers are here to deliver safe, professional, and affordable support." | CTA band, both source pages |
| Reviews | "EXCELLENT ... Based on 16 reviews" (Trustindex Google widget) | Both source pages |
| Owner | Reviews name "Ben" (e.g. "Definitely recommend Ben and Coast to Coast plumbing!") | Google Reviews, both source pages |
| Legal entity | "© DowntheRoad (Vic) Pty Ltd for Coast to Coast Plumbing &amp; Gasfitting" | Footer, every page |
| Services | CCTV inspections, high-pressure jetting, repair or relining, sewer and stormwater drains, excavation and drainage repairs | Both source pages |

No licence number, address, ABN, warranty or guarantee terms, response times or prices appear on these pages. Do not invent any. "Customer Satisfaction Guaranteed" is a fixed card title only; do not expand it into a guarantee claim.

## Internal links
- Body copy on the live pages carries no inline links. Do not add links in your paragraphs.
- All internal links are in the fixed parts: CONTACT US and Submit go to `https://coasttocoastplumbingmp.com.au/contact/`, phone uses `tel:0437094448`, the Areas grid links 29 suburb pages (Mordialloc, Mentone, Seaford, Frankston are the nearest existing pages to Aspendale, Chelsea and Parkdale).
- Do not invent URLs for suburbs that have no page.

## Avoid
- Prices, timeframes ("within an hour"), guarantees, licence numbers, years other than "over 20 years".
- Naming other suburbs as if they have pages, or adding the new suburb to the Areas grid.
- Calling the page anything other than a blocked drain page in the H1.
- Extra sections, extra FAQs, lists in the intro, bold text, inline links, inline styles, a second H1.
- Copying the Blairgowrie or Somers wording; reuse the pattern, write fresh sentences.
