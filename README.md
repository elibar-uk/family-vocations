# Family Vocations

## What Does "Vocation" Mean?

The word "vocation" traditionally means a calling, purpose, or mission. It comes from the Latin *vocare*, meaning "to call."

In the context of Family Vocations, the idea is that a family is not just a group of people living together—it has a shared calling to:

- Love and support one another.
- Build strong relationships.
- Create meaningful experiences.
- Pass on values and traditions.
- Help each family member grow and flourish.

Family holidays can be seen as one way of living out that calling. They provide dedicated time to connect, communicate, create memories, and strengthen family bonds.

## Purpose

The name **Family Vocations** reflects the idea that a family has a shared calling to grow together, support one another, create meaningful memories, and strengthen relationships. Family holidays provide valuable opportunities to live out that calling by spending intentional time together, exploring new experiences, and building lasting traditions.

This folder exists to collect and organize holiday plans, itineraries, and travel resources that help our family make the most of these shared experiences.

## Repository structure

```
family-vocations/
├── index.html              # Hub page — lists all trips
├── data/
│   └── trips.json          # Trip registry (title, slug, year, etc.)
├── assets/
│   └── css/
│       └── hub.css         # Shared styles for the hub page
└── trips/
    └── {slug}/             # One folder per holiday
        └── index.html      # Trip page (itinerary, plans, etc.)
```

Each trip uses a slug in the form `{destination}-{year}` (e.g. `portugal-2026`, `italy-2027`).

## Trips

| Trip | Page |
|------|------|
| Portugal 2026 (Caparica) | [/trips/portugal-2026/](trips/portugal-2026/) |

## Adding a new trip

1. Create a folder: `trips/{destination}-{year}/`
2. Add your trip page as `trips/{destination}-{year}/index.html`
3. Register the trip in `data/trips.json`:

```json
{
  "slug": "italy-2027",
  "title": "Italy 2027",
  "subtitle": "Tuscany · Easter 2027",
  "year": 2027,
  "destination": "Italy"
}
```

The hub page at the site root reads `trips.json` automatically — no changes to `index.html` needed.
