# SmartGrid — Phase 1 Prototype

A responsive, browser-based prototype of the SmartGrid energy monitoring dashboard.

## Run it
Open `index.html` in a modern browser, or deploy this repository to Vercel as a static site.

## What's included
- Responsive sidebar navigation and hover/active states
- Dashboard cards, illustrative usage chart, recent activity
- Live Usage, Devices, Alerts, AI Assistant demo, Reports, Help & Safety, Settings
- Login-screen prototype
- Device onboarding preview
- Predefined local assistant responses
- CSV export of illustrative sample data
- Explicit labels distinguishing demo data from real readings

## Important limitations
This is a front-end prototype. It does **not** implement real authentication, persistent storage, Gemini, live IoT/hardware connectivity, real alerts, or a production offline/PWA service worker. All electricity readings are simulated and clearly labelled. Do not treat the interface as an electrical safety or protection system.

## Next milestones
1. Review the UI and test navigation.
2. Move to a structured app framework if needed.
3. Add authentication and persistent storage.
4. Add a secure device data endpoint and test with simulated device messages.
5. Integrate Gemini through a server-side API route.
6. Add and test offline caching and synchronization.
