# Atmos Rewards Award Launcher · US ↔ China / Europe

A single-page tool that quickly launches **Alaska / Hawaiian (Atmos Rewards, formerly Mileage Plan) partner award calendar searches** for travel between the US and China or Europe. Pick a direction, month, cabin, and passenger count, then click any route to open the Alaska award calendar in a new tab.

## Live page

https://gyjdb.github.io/alaska-award-search/

Or download `index.html` and open it in any browser — it's fully self-contained (no install, no dependencies, no tracking).

## What it does

- **Trans-Pacific gateways** — search the scarce long-haul leg (US ↔ HKG / Tokyo / TPE / ICN), each tagged with the Atmos partner that flies it (Cathay Pacific, Japan Airlines, Starlux, Korean Air).
- **Mainland China** — full US ↔ Shanghai (PVG) search; Alaska auto-routes through a partner hub.
- **US ↔ Europe gateways** — MAD (Iberia), HEL (Finnair), DUB (Aer Lingus), CDG (American), LHR (BA / American), FRA (Condor / American), with fuel-surcharge flags.
- **Direction toggle** — Leaving US / Back to US.
- **Cabin + passengers** — fare type and 1–4 passengers.
- **Quick months** — set to the student travel windows: go home (Dec / Jun) and return (Sep / Jan).
- **Copy all** — grab every route link for one destination to batch-open.
- Remembers your last direction / month / cabin / passengers on your device.

## Notes worth knowing

- There is no fixed "direct vs connection" label — whether a date is nonstop or connecting (and the mileage price) is what the calendar search reveals.
- Europe value tip: Iberia / Finnair / Aer Lingus and American metal avoid the fuel surcharges that British Airways metal adds (can top $500 each way).
- One free stopover per one-way award, single partner per award (mixing only AA / BA / Finnair so far), no round-trip discount. Atmos blocks many partner awards within ~72h of departure and shows occasional phantom space.
- This tool only builds search URLs and opens them on alaskaair.com. It doesn't fetch or store any data and contains no credentials.
