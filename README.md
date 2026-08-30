# CheapAzGarage

> Family vehicle maintenance archive — repair logs, parts sourcing, and VIN lookups for every car the family has owned, wrenched on, or is currently building.

Cost-conscious, DIY-first documentation. If it's cheaper at RockAuto than the dealer, that's the plan.

## What's here

| | |
|---|---|
| [`VEHICLE-INVENTORY.md`](VEHICLE-INVENTORY.md) | Every vehicle — current, archived, and in-progress — with ownership and IDs |
| [`VEHICLE-LOOKUP.md`](VEHICLE-LOOKUP.md) | Look up any vehicle by VIN, plate, or year/make/model |
| [`vehicles/`](vehicles) | Active maintenance folders — repair history, parts, known issues, cost tracking |
| [`archive/`](archive) | Vehicles no longer in the family (sold, crushed, retired) |

## Current fleet

| Vehicle | Owner | Status |
|---|---|---|
| 2004 Lexus ES330 | Bao | Active — 145K+ mi |
| 2018 Ford Transit 150 | Bao | Active |
| 2003 Toyota Sienna | Family | Active |
| Honda Odyssey EV Conversion | Family ("Justine's van") | In-progress build |

Full details, VINs, and plates: [`VEHICLE-INVENTORY.md`](VEHICLE-INVENTORY.md).

## Folder layout

```
vehicles/<Make>_<Model>_<Year>/README.md    — overview, repair history log, cost analysis, known issues
vehicles/<Make>_<Model>_<Year>/parts.md     — one table, every part purchased (brand, part #, price, order, install date)
vehicles/<Make>_<Model>_<Year>/intervals/   — one file per ~3,000-mile checkpoint, task checklist with done/date
archive/<Make>_<Model>_<Year>/README.md     — retired vehicle record (ID + final status only)
```

## Using this on a phone

Every doc is plain markdown — GitHub's mobile app and web view render it fine in the garage. Tables are kept narrow so they're readable without much horizontal scrolling.

## Contributing

Just Bao and family for now. See [`CONTRIBUTING.md`](CONTRIBUTING.md) for doc conventions (image naming, commit style, how to log a repair).
