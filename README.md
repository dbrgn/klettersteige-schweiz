# Klettersteige Schweiz

## Re-sorting GeoJSON

    jq '.features|=sort_by(.properties.title)' klettersteige.geojson | sponge klettersteige.geojson
