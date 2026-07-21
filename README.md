# Allo — Clinic Trackers (hub)

One page, two tabs, embedding the two live dashboards:

- **Revenue** → the Clinic Pulse revenue tracker
  (https://vishesh-png.github.io/Clinic-Pulse-Tracker/)
- **Macro Analysis** → the Macro clinic-level dashboard
  (https://vishesh-png.github.io/Macro-Level-Analysis/)

Each embedded dashboard auto-refreshes daily from its own Google Sheet, so this
hub always shows current data with no build step of its own. `index.html` is a
thin shell that switches between the two in iframes (the Macro tab lazy-loads on
first open). Deployed to GitHub Pages via `.github/workflows/deploy.yml`.

To change which dashboards are embedded, edit the `SRC` map in `index.html`.
