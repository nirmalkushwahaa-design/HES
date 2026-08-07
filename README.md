# Anantya HES — Admin Dashboard Pitch

Static HTML/CSS/JS mockups for the redesigned Anantya HES (Head-End System) admin dashboard, prepared by Redmelon for the Gridcrest Technology pitch.

This is private, pre-deal pitch material — not deployed to a public URL. Open any file directly in a browser to view it locally (start with `index.html` or `dashboard.html`).

**Note:** this was briefly live on Cloudflare Pages (public URL, gate-able only via a manual dashboard step) and was taken down once we confirmed that wasn't intended. If you want a shareable live link again, it needs Cloudflare Access (or similar) configured first so it isn't open to anyone with the URL.

## Pages

- [`dashboard.html`](dashboard.html) — Operations Overview: fleet-wide KPIs, alarms by severity, recent events, communication health, data collection trend, top devices with alarms. The alarm badge count reads live from Events' data.
- [`home.html`](home.html) — System → Home: device explorer with search/filter, selected-device workspace (properties, communication, states, network & security), services (toggles persist), and risk-tagged activities (Execute runs a real Waiting → Executing → Success/Failed cycle).
- [`events.html`](events.html) — System → Events: filterable event list with live summary stats, severity/category facets, and a full Acknowledge → Assign → Resolve → Reopen workflow with notes. Use "Reset demo data" to restore the original seed data at any time.

## Persistence

Event and service-toggle changes are saved to the browser's `localStorage` (keys `hes-demo-events-v1` / `hes-demo-services-v1`), so they survive a reload and stay consistent across pages. This is demo-only persistence — per-browser, not shared between viewers, and not backed by any real database.

## Status

Pitch-stage design work — not built against the live Anantya HES platform or its real data. Content (device IDs, numbers, event examples) is representative, not production data. See the accompanying domain-knowledge documentation (KT call notes, per-screen behavior specs) for what's confirmed vs. assumed.
