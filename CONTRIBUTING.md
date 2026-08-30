# Contributing / Doc Conventions

Personal family repo, but keeping the format consistent makes it usable years from now.

## Adding a repair

In the relevant `vehicles/<Vehicle>/README.md`, add a row to **Repair History Log** with date, service, cost, and source. If a new part number or vendor came up, add it to **Parts Inventory** too.

## Images

Save photos into `vehicles/<Vehicle>/src/` (create the folder if it doesn't exist). Name them `[system]_[part-description].jpg` — e.g. `suspension_kyb_strut_front.jpg`, `electronics_denso_starter.jpg`. Lowercase, underscores, no spaces.

## Retiring a vehicle

Move its folder from `vehicles/` to `archive/`, trim the README down to identity + final status (sold/crushed/traded, date, mileage), and update its rows in `VEHICLE-INVENTORY.md` and `VEHICLE-LOOKUP.md`.

## Commit messages

Short imperative title, one-line body on why if it's not obvious. Push directly to `main`.

## When data is uncertain

Leave it `TBD` and flag it — don't guess a VIN, plate, or part number. A wrong VIN in a maintenance record is worse than a blank one.
