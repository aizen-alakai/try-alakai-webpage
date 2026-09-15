# tryalakai.com landing page

Outbound landing page for Alakai. Static, no build step.

## Files

- `index.html` – the live page. Positioned on the MVP product brief: an individual subscription for account teams at FMCG manufacturers, delivered through the Alakai connector and skills in a personal Claude account. Sections: hero with an illustrative weekly brief, why weekly, what is in the brief, five steps from signup to first brief, four Pro insights, plans and prices with a monthly/annual toggle, FAQ, final call to action.
- `long-form.html` – the earlier long-form version of the planning-cycle positioning, kept as a copy source. Not linked from the live page.
- `assets/` – brand logos and arrow motif from the Alakai brand skill; product screenshots and founder photo from alakailabs.com (the screenshots show the earlier planning product and are not used on the live page).

## Run locally

```bash
python -m http.server 8765 --directory tryalakai-landing
```

Then open http://localhost:8765/.

## Before publishing

Edit the `CONFIG` block at the bottom of `index.html`:

| Key | Current | Change to |
|---|---|---|
| `signupUrl` | `https://app.tryalakai.com/signup` (placeholder) | The real account-creation URL. The page appends `?plan=trial|basic|pro` and UTM tags |
| `calendarUrl` | Existing Google Calendar booking link, tagged `utm_source=tryalakai` | Keep, or a dedicated Enterprise call schedule |

Refresh the banner count (currently 45) before each publish, per the Claims and Proof Register.

## Claim discipline

Copy stays inside the MVP product brief and the Claims and Proof Register: coverage limited to observed banners with store counts, geography and dates shown; observed prices and offers only; stacking combined only when verified; missing observations distinct from no change; no funding, lift, margin or ROI inference; assortment appearance and disappearance described as observations. "About ten minutes" to first brief is the brief's design target and is phrased as such. Prices and plan limits match the brief's plans table and coverage defaults. Claude access is stated as separate, and the footer disclaims affiliation with Anthropic.
