# Schema

## route_segments.csv

- `segment_id`: stable segment key
- `name`: display name
- `distance_km`: route distance in kilometers
- `profile`: short difficulty/profile label
- `estimated_time`: practical duration label
- `best_for`: suggested use case
- `color`: map color used on the site
- `parts`: number of line pieces grouped into the simplified geometry

## key_points.csv

- `id`: stable point key
- `type`: `stop` or `poi`
- `poi_type`: optional subtype for POIs
- `name`: display name
- `segment_ids`: related segment ids
- `lat`: latitude
- `lon`: longitude
- `summary_es`: short Spanish summary

## trail_overview.json

Top-level JSON payload with dataset metadata, route segments, and key points.

## trail_map_simplified.geojson

`FeatureCollection` with:
- `3` `MultiLineString` features for route segments
- `9` `Point` features for stops and POIs
