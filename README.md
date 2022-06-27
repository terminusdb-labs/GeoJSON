# GeoJSON in TerminusDB

This is a schema for TerminusDB which allows Terminus to ingest
GeoJSON directly. This requires TerminusDB v10.1.0 or higher.

Example:

```shell
terminusdb db create admin/geojson
terminusdb doc insert admin/geojson -g schema < geojson.json
echo '{"type" : "Point", "coordinates" : [48.2082,16.3738]}' | terminusdb doc insert admin/geojson
```
