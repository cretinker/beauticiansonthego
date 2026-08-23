# Working agreement

## Who I am building for
Every website in these projects is a **client pitch**. The user is an agency-of-one
selling website work to business owners. The deliverable is never "a website" —
it is **a marketing asset the owner can run paid traffic to in order to increase
bookings/sales**, with the user offering to run those ads as follow-on work.

This must be reflected in the design, the pitch deck, and the outreach message.

## Standard workflow for a new client site
1. **Research the current site thoroughly** — real services, real prices, real
   cities, real testimonials, real contact details, all customer segments. Never
   invent business facts. Flag anything unverified for the client to confirm.
2. **ask_user form** — positioning, booking model, pricing transparency, segments,
   aesthetic, variations, scope, imagery, copy, differentiator.
3. **2–3 homepage directions** as one options file, newest turn on top, so the
   user can pick before the full build.
4. **Build the full site** as a shell DC + one DC per page, wired with dc-import
   and an in-shell router. Always include:
   - a full-bleed hero with segment chips that deep-link into the quote builder
   - one landing page per customer segment (these become the ad campaigns)
   - published pricing wherever the client will allow it
   - a working multi-step quote builder with a live estimate and exit-intent callback
   - a team page with names, specialties and photo slots
   - a persistent booking bar after the fold
   - scroll-reveal motion, counters, sticky filtered nav with dropdown panels
5. **Copy** — declarative and selling, never describing itself. No metadiscourse,
   no self-congratulation, no arch asides. Headlines make an argument; body copy
   names the customer and what they get.
6. **index.html** — keep a copy of the shell at the project root so the folder
   drops straight into Netlify.
7. **Pitch deck** — see below.
8. **Outreach DM** — see below.

## The pitch deck (always this arc)
Never a design review. It is a business case.
1. Title — "let's fill your calendar", asset not brochure
2. **The prize** — what one extra booking a week is worth, using the client's own
   published prices. Arithmetic, not projections.
3. **The leak** — why ad spend would currently leak out: nowhere to land, nothing
   to click, nothing to measure, nothing to believe. Each with "Now: …"
4. The asset — live iframe of the homepage
5. Landing pages — live iframe, one campaign per segment
6. The quote engine — live iframe, demoed in the room. This is the closing moment.
7. The differentiator — the segment no competitor is advertising in
8. **The ad plan** — 4 campaigns mapped to channels and landing pages, offered as
   help either way
9. What happens next — three steps, two weeks, the only real ask is photography
10. Close — ask for the yes, with proof numbers

Live iframes point at the **source DC**, never at the index.html copy (which goes
stale). Header rows in flex-column slides need `flex-shrink:0` and headlines
`flex:0 0 auto; white-space:nowrap` or they get painted over.

## The DM that goes with it
Short, outcome-led, no design vocabulary. Structure:
hook about bookings → what I built → the live link → one number that shows the
prize → the ad plan as the real offer → a small, specific ask.
Never lead with "I redesigned your website."

## Design defaults that have worked
- Editorial serif display (Bodoni Moda) + clean grotesque body (Karla)
- Bone / ink / one warm accent / one gold. Max two background colours.
- Inline styles only, `minmax(0,1fr)` on any grid holding long headlines
- Photography pulled from the client's existing site first, Wikimedia/Unsplash for
  gaps, with drop-in slots for the real shoot
- Always tell the client which facts and images need their sign-off before launch
