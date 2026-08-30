# Contributing / Doc Conventions

Personal family repo, but keeping the format consistent makes it usable years from now.

## Vehicle folder naming

`vehicles/<Make>_<Model>_<Year>` (e.g. `Lexus_ES330_2004`, `Toyota_Sienna_2003`). Include the trim/edition if the vehicle has a distinguishing one: `Ford_Transit_150_2018`, `Honda_Accord_2000_SpecialEdition`. Archive folders follow the same pattern.

## Adding a repair

1. Add a row to the vehicle's **Repair History Log** (date, order #, service, cost).
2. Add a row per part to `vehicles/<Vehicle>/parts.md` — one table, columns: `Part | Brand | Part # | Qty | Price | Order Date | Order # | Source | Installed | Status | Notes`. If the real install date isn't known, assume shortly after the order date and flag it as assumed in Notes.
3. If the vehicle has interval checklists (see below), add or update the relevant `intervals/<mileage>mi.md` file to mark the matching tasks done.

## Interval checklists

For vehicles with mileage tracked, `vehicles/<Vehicle>/intervals/` holds **one file per ~3,000-mile checkpoint** (e.g. `133000mi.md`), not per interval *type*. Each file lists standard maintenance tasks (oil/filter, tire rotation, fluid check, brake inspection, cabin/engine air filter, etc.) as a checklist with a Done column and a Date column, plus whatever was actually confirmed done from real orders. When the exact odometer reading at a service date isn't known, interpolate it from known checkpoints and say so — an estimated mileage beats no mileage.

## Images

Save photos into `vehicles/<Vehicle>/src/` (create the folder if it doesn't exist). Name them `[system]_[part-description].jpg` — e.g. `suspension_kyb_strut_front.jpg`, `electronics_denso_starter.jpg`. Lowercase, underscores, no spaces.

## Retiring a vehicle

Move its folder from `vehicles/` to `archive/`, trim the README down to identity + final status (sold/crushed/traded, date, mileage), and update its rows in `VEHICLE-INVENTORY.md` and `VEHICLE-LOOKUP.md`.

## Commit messages

Short imperative title, one-line body on why if it's not obvious. Push directly to `main`.

## When data is uncertain

Leave it `TBD` and flag it — don't guess a VIN, plate, or part number. A wrong VIN in a maintenance record is worse than a blank one. For dates that genuinely can't be pinned down (e.g. an install date vs. order date), an approximate date close enough in time is fine — just mark it as assumed/estimated rather than presenting it as exact.
