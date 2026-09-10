# tryalakai.com landing page

Outbound landing page for the 90-Day Trade Performance Action Cycle. Static, single file, no build step.

## Run locally

```bash
python -m http.server 8765 --directory tryalakai-landing
```

Then open http://localhost:8765/. Opening `index.html` directly from disk also works.

## Files

- `index.html` – the whole page: markup, styles, and the small script for the fit check and form.
- `assets/alakai-wordmark-blue-2x.png`, `alakai-wordmark-white-2x.png`, `alakai-logo-primary.png`, `alakai-arrow-motif.png` – brand files from the Alakai brand skill.
- `assets/post-event-insights.png`, `competitor-promotions-workflow.png`, `tpm-link-workflow.png` – product screenshots pulled from alakailabs.com.
- `assets/cam-lizenby.jpg` – founder photo from alakailabs.com.

## Before publishing

Edit the `CONFIG` block at the bottom of `index.html`:

| Key | Current value | Change to |
|---|---|---|
| `calendarUrl` | The existing Google Calendar booking link from alakailabs.com, tagged `utm_source=tryalakai` | Keep, or point at a dedicated scoping-call schedule |
| `contactEmail` | `hello@tryalakai.com` (placeholder) | The inbox that should receive scoping requests |
| `formEndpoint` | empty | A Formspree, HubSpot, or Netlify Forms endpoint. While empty the form falls back to opening a pre-filled email |

Also:

1. Add analytics and a privacy page link in the footer if you run ads to this page.
2. Refresh the banner count (currently 45) before each publish, per the Claims and Proof Register.
3. Decide whether to keep the `From ~$35K` fact tile. The register classifies price as customer-specific; the customer-facing offer sheet shows it with the same footnote used here, so it is defensible, but it is one block to delete if you prefer to hold price for the call.

## Claim discipline

Copy is drawn from the Positioning Decision Brief v0.9, the 90-Day offer sheet, the one-pager, the customer sales deck, and the objection guide. Everything on the page is either "claimable today" or "claimable with qualification" in the Claims and Proof Register, with qualifiers kept in place:

- Coverage: 45 banners and growing; weekly, store-level grocery; GTIN-level "where available".
- Competitive signal: detection and relative shopper-value change only, "within covered scope". No optimal response, no elasticity.
- Money: "annualized opportunity", never realized impact. Guarantee, target, measure hierarchy shown as a table.
- AI: the approved AI statement, verbatim. No "AI-native", "agentic", or MCP language.
- System posture: read-only, expert approval, no write-back claims.

Deliberately left off the page:

- The eight-months, seven-share-points competitive story (CLM-022, internal only until customer approval and anonymization are confirmed).
- Any prevented-loss percentage (CLM-023, do not claim).
- The encryption and isolation wording (CLM-013 and CLM-014, internal only pending security and legal review). The page links to the existing data-security page on alakailabs.com instead.
- The hero action pack is labelled "Illustrative example" and carries no dollar figures.

## Page flow

Hero (campaign line and illustrative action pack) → proof strip → the fragmentation problem → two urgency clocks → SEE / DECIDE / ACT / MEASURE → product screenshots → unit lift vs profit example → the 90-day cycle with three phases, inclusions, price footnote → success boundary table → four-gate fit check (interactive) → what Alakai is not, plus the AI statement → founder → FAQ from the objection guide → contact form and calendar → footer with claim qualifiers.
