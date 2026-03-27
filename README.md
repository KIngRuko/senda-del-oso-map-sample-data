# La Senda del Oso Map Sample Data

Small public map dataset from [lasendadeloso.com](https://lasendadeloso.com).

This repository publishes a limited, structured sample of route segments and key access points from the public trail map without exposing editorial content, booking logic, or internal workflows.

What is included:
- `3` route segments
- `9` key stops and POIs
- simplified GeoJSON, CSV, and JSON formats

What is not included:
- long-form editorial copy
- booking or pricing logic
- internal analytics or conversion data
- unpublished map layers
- full business workflows

## Files

- `data/route_segments.csv`
- `data/key_points.csv`
- `data/trail_overview.json`
- `data/trail_map_simplified.geojson`
- `SCHEMA.md`
- `DATA-LICENSE.md`

## Selection method

The dataset is derived from public map data already used on the website:

1. Route lines are grouped by segment id.
2. All route pieces for each segment are preserved in a simplified `MultiLineString` feature.
3. Public access points and POIs are exported as point features with basic metadata.

This is a practical sample for inspection, prototyping, and map testing.

## Attribution

If you reuse the dataset, attribute it as:

[La Senda del Oso](https://lasendadeloso.com)

## Licenses

- Code/repo files: `MIT`
- Dataset in `data/`: `CC BY 4.0`
