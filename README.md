# tryalakai.com landing page

Outbound landing page for Alakai. Static, no build step.

## Files

- `index.html` – the live page. Two screens, two calls to action: a trial-enquiry form (name, work email, phone, company) and a link to book a trial call on the calendar. Positioning: the 12-week promotion lock as the hook, the locked campaign line as the headline, SEE / DECIDE / ACT / MEASURE with buyer agreement inside ACT, and a 90-day trial paced to the customer's decision dates.
- `long-form.html` – the earlier long-form version, kept as a copy source for marketing. Not linked from the live page.
- `assets/` – brand logos and arrow motif from the Alakai brand skill; product screenshots and founder photo from alakailabs.com.

## Run locally

```bash
python -m http.server 8765 --directory tryalakai-landing
```

Then open http://localhost:8765/.

## Before publishing

Edit the `CONFIG` block at the bottom of `index.html`:

| Key | Current | Change to |
|---|---|---|
| `calendarUrl` | Existing Google Calendar booking link from alakailabs.com, tagged `utm_source=tryalakai` | Keep, or a dedicated demo schedule |
| `contactEmail` | `hello@tryalakai.com` (placeholder) | The inbox that receives trial enquiries |
| `formEndpoint` | empty | A Formspree, HubSpot, or Netlify Forms endpoint so requests land in a CRM. While empty the form opens a pre-filled email |

Refresh the banner count (currently 45) before each publish, per the Claims and Proof Register.

## Claim discipline

Copy stays inside the Claims and Proof Register v0.9: coverage limited to covered banners, deterministic calculations (footer), expert approval, read-only start, estimates labelled as annualized and never as realized impact. "Promotions typically lock about 12 weeks before they run" is a general market statement, qualified with "typically". No pricing on the page; the internal-only competitive story and prevented-loss figures are not used.
