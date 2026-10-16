# RoadSync mockup

A role-based product mockup of the RoadSync concept. It shows how public travelers, police, PWD, ambulance services, and the RoadSync Authority could use a shared road information platform.

## Run it

1. Install Node.js 20 or newer.
2. From this folder run `npm run dev`.
3. Open the printed local URL (normally `http://localhost:4173`).

## Explore the mockup

Use the **View as** selector in the top bar:

- **Public traveler:** browse sample incidents, change the simulated city, view proximity notices, and preview a route.
- **Police department:** submit a traffic report to the central review queue; see evidence and urgent warning placeholders.
- **PWD department:** submit a roadwork notice and inspect a sample work progress tracker.
- **Ambulance EMS:** activate and close a simulated emergency session, inspect demo route advisories, and see the privacy boundary.
- **RoadSync Authority:** start with 32 sample reports: 8 pending, 16 active, 4 rejected, and 4 resolved across Goa. Inspect each report's department, evidence note, timestamp, and coordinates, then approve, reject, request follow-up, flag a duplicate, escalate, or resolve.

Police and PWD reporting forms include **Use live location**. Clicking it asks the browser for location permission and attaches the returned latitude/longitude and accuracy to the report. If permission is denied or unavailable, the selected demo-area coordinates remain usable. Accident reports require a local image selection in the Police form; the image is not uploaded.

Department reports persist in this browser's local storage. Approval makes a report visible in the public map; resolving it removes it from active alerts. Use the browser's site data controls to reset the demo.

## What is simulated

This is a single-browser interface mockup. Role selection is not authentication or authorization. It has no Supabase, shared backend, secure evidence upload, agency identity verification, real dispatch or ambulance tracking, route engine, map tiles, live traffic data, actual emergency-publication policy, or connection to government systems. All organizations, incidents, hospital names, locations, operational status, travel times, and metrics are illustrative demo content. Ambulance coordinates and emergency activation are simulated. The map is a stylized schematic with approximate distances; route and proximity information must not be used for real travel or emergency decisions.
