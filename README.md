# SmartGrid Phase 2 prototype

## Included
- Responsive dashboard with simulated usage readings and illustrative chart
- Block selector, local device labels, installation checklist, and alert history
- Rule-based demo assistant (not connected to Gemini)
- Optional JSON endpoint for readings from a server you control
- CSV export, browser local storage, and basic offline app-shell caching

## Preview and publish
Open `index.html` to preview. Service workers/offline caching require HTTPS or localhost. To publish with GitHub Pages: upload `index.html`, `manifest.webmanifest`, `sw.js`, and `README.md` to your repository root; go to **Settings → Pages**; choose **Deploy from a branch**, branch `main`, folder `/(root)`, then save.

## Optional reading endpoint
The Settings page accepts an endpoint URL you control. It should return JSON like:
`{"power_kw":2.8,"energy_today_kwh":18.4,"status":"normal","timestamp":"2026-10-15T10:00:00Z"}`
The endpoint must allow browser CORS requests.

## Limitations
Readings are simulated unless an endpoint is configured. Device registration stores labels only; no ESP32/sensor connection exists. The assistant is fixed demo text and does not call an AI service. Local storage is not a shared database or backup. Secure login, user roles, cloud storage, authenticated device ingestion, push alerts, and robust offline synchronization are not implemented. This is not an electrical safety system; use certified protection hardware and qualified professionals.
