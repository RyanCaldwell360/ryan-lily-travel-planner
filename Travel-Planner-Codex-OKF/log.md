# Bundle update log

## 2026-10-19 — Trip date interaction correction (agent-authored)

Reproduced the Chromium issue where clicking the date text focused the input without opening its calendar; the native calendar icon worked. Added explicit native-picker activation for clicks across each trip date field, retaining ordinary entry when the API is unavailable. Whole-trip protection chosen in a draft no longer disables the fields needed to complete it; saved protected trips still require explicit server unlock. Added a real native-calendar browser regression that saves independent synthetic Ryan/Lily Cozumel dates through the D1 fixture, reloads them, and checks saved protection. Updated production source guidance to the Cloudflare-connected `RyanCaldwell360/ryan-lily-travel-planner` import, retaining the original repository as a separate remote. Verification: 19 core/API/runtime tests, 4 browser workflows, strict TypeScript/build, and Wrangler deployment dry run passed. No production household data was used or changed during tests.

## 2026-10-17

- **Creation**: Captured the product discovery interview as an OKF v0.2 knowledge bundle.
- **Clarification**: Separated confirmed requirements, uncertain employer inputs, and proposed implementation semantics.
- **Coverage**: Added PTO/tradeoff rules, shared persistence, discovery integrations, and behavioral acceptance cases.

## 2026-10-17 — First implementation (agent-authored)

Read the supplied context before choosing a stack; the target Git repository had no commits or application files. Built React/TypeScript year planning with an Express/SQLite private server, separate identities, integer PTO ledger, setup, individual trip/day editing, explicit previews, locks, non-trip leave, school opportunities, named alternatives, full-year comparisons, multi-trip tradeoffs, revision conflicts/history, and exports. Bundled an interactive geographic map and attributed moodboard photography. Implemented replaceable travel/weather adapters with honest unavailable states. Recorded concrete architecture/accounting choices without treating tentative employer information as facts. Verification and remaining limitations are recorded in `quality/implementation-status.md`. No human verification, public hosting, real bookings, or live provider data is claimed.

## 2026-10-17 — Free deployment preparation (agent-authored)

User clarified that hosting must be free. Added a Cloudflare Worker/D1 backend, cryptographically verified household email identities through Access, atomic D1 history/revision writes, storage-neutral evidence caching, and client background-worker tradeoff search. Prepared `wrangler.jsonc`, free-account/GitHub deployment instructions, explicit quota/recovery limits, and the Access Free payment-details caveat. Preserved Node local development and all PTO semantics. Verified locally with real D1/workerd engines and independent-browser workflows. No Cloudflare account is connected; no public URL or actual external deployment is claimed. The code is ready for the owner's free account configuration.
