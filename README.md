# ID Logistics — Global Convention 2026

Email assets and Brevo template for the *Save the Date* communication.

## Layout

- `01_Assets/Header-ID-log-1360.png` — email header banner (1360 × 502 px, 2× export for retina)
- `email/save-the-date.html` — Brevo-ready HTML template
- `email/save-the-date.ics` — calendar invite (June 16, 2026, 14:00–15:30 Europe/Paris)

## CDN URLs (jsDelivr)

- Header: `https://cdn.jsdelivr.net/gh/WMH-Project/ID-Logistique@main/01_Assets/Header-ID-log-1360.png`
- ICS: `https://cdn.jsdelivr.net/gh/WMH-Project/ID-Logistique@main/email/save-the-date.ics`

> jsDelivr caches aggressively. When updating an asset, either rename the file or pin to a commit SHA in place of `@main` to bust the cache.

## Brevo setup

1. In Brevo, *Campaigns → Email templates → New template → Import HTML*.
2. Paste the contents of `email/save-the-date.html`.
3. The `{{ contact.FIRSTNAME }}`, `{{ unsubscribe }}` and `{{ mirror }}` tags are resolved by Brevo at send time.
4. The "Add to my calendar" button links directly to the hosted `.ics` — no attachment needed.
