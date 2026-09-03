# Atmos Search Console

A self-contained browser tool for two related Alaska / Atmos workflows:

1. finding low cash fares in **Main Cabin** while planning qualifying flight segments; and
2. launching **Atmos Rewards partner-award calendar** searches between the US, China, and Europe.

The interface is in Chinese and runs entirely from one HTML file. There is no build step, server, account login, or external dependency.

## Live page

https://gyjdb.github.io/alaska-award-search/

You can also download `index.html` and open it directly in a browser. The legacy `alaska_award_launcher.html` entry is kept in sync so old links continue to work.

## Cash Main search

- Flexible-date monthly calendar and exact-date result links.
- Custom airport search with datalist suggestions and recent routes.
- Two-ticket planner for building **2 + 2 = 4 segments**.
- East/Central-to-West fare comparison matrix.
- West Coast short-haul and Hawaii route presets.
- Main Cabin is fixed in every cash-search URL.
- Opened-route markers, copy tools, and light/dark themes.

## Price tracker

- Save a complete two-ticket plan with route, dates, both ticket prices, actual segment counts, extra costs, status, and notes.
- Live calculations for airfare per segment and all-in cost per segment.
- Candidate / booked / flown states.
- Qualifying-progress guard: only booked or flown plans whose operating eligibility was manually verified count toward the 8-segment target.
- Sort and filter saved plans, edit or delete them, and export all records as CSV.
- One-click handoff from the two-ticket planner into the tracker.

## Award search

- Custom award calendar search plus Asia/China and Europe route presets.
- Leaving-US / returning-US directions.
- Cabin and passenger controls.
- Partner labels, nearby-month comparisons, saved recent routes, and practical booking notes.

## Local data and privacy

Preferences, opened-route markers, and price-tracker records are stored only in the browser's `localStorage`. The tool does not upload or collect them and contains no credentials. Price records can be exported as CSV before changing browsers or clearing site data.

The tool only constructs Alaska search URLs. Alaska's live results and the current promotion terms remain the final source of truth for fare, routing, operating carrier, cabin, and segment eligibility.
