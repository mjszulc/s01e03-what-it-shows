# MEGA.dev S01E03 — What it shows

This repository contains the support knowledge base export and the signed incident page prepared for Challenge S01E03.

## Deliverables

- `support-kb/src/routes/kb/incidents/4471/+page.svx` — the updated KB page, with the cause table, timeline, and desk signature.
- `desk-view-4471.html` — a static preview of the page using the exported KB component logic.
- `support-kb/src/lib/data/` and `support-kb/src/lib/kb/` — the course export data and components used by the page.
- GitHub issues [#1](https://github.com/mjszulc/s01e03-what-it-shows/issues/1) and [#2](https://github.com/mjszulc/s01e03-what-it-shows/issues/2) — the two cause tracks with their report counts.

The export does not include the app's package manifest or build scripts, so the HTML preview is a static rendering of the page content and computed component values.

## Report reconciliation

The export has 427 rows and 412 unique report IDs. Fifteen rows repeat existing IDs, with no conflicting duplicate records. The tenant, form, and channel rules in `support-kb/src/lib/kb/causes.ts` place 379 reports in the shared parser group and 33 in the booking-v3 hint group.

The course's 5 October desk update says the parser fix shipped as `fix(dates): parse dd/mm for eu locales` and booking-v3 was retired. Issue #1 is closed as completed; issue #2 is closed as not planned.
