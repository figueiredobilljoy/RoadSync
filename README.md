# RoadSync quick prototype

A self-contained browser demo of the RoadSync road incident workflow. No account or external service setup is needed.

## Run it

1. Install Node.js 20 or newer.
2. From this folder run `npm run dev`.
3. Open the printed local URL (normally `http://localhost:4173`).

## Demo flow

1. Explore the preloaded, clearly labeled Goa sample incidents on the map.
2. Change the simulated location to Margao or Vasco, or choose **Use my location** and allow the browser permission.
3. Select **Report incident**, fill in the form, and submit. The report is saved as **Pending** and is hidden from the public incident list/map.
4. Open **Incident reports**, then approve or reject the pending report. Approving adds it to the active map; resolving an approved report removes it from active warnings.
5. Use the type filter, search, map zoom controls, and incident queue tabs to explore the prototype.

Reports persist in this browser's local storage. Use the browser's site data controls to reset the demo. Sample response and network insight figures are illustrative.

## Scope

This is a local, single-browser demonstrator. It has no Supabase connection, real authentication, server-side role enforcement, shared persistence, actual map tiles, official traffic feed, dispatch integration, or physical signal control. The map is a stylized Goa schematic with demo coordinates, and all reports are locally simulated. Proximity is a straight-line estimate. Do not use it for real traffic or emergency decisions.
