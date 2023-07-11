# Geospatial Metadata

The GIS project metadata is stored in a collection of the OGC API, according to the draft specification of [OGC API Records](https://github.com/opengeospatial/ogcapi-records).

The schema is an extension of the [OGC API Records Metadata Schema](https://github.com/opengeospatial/ogcapi-records/blob/master/core/openapi/schemas/recordGeoJSON.yaml)[^1].

[^1]: Last update from _OGC API Records Metadata Schema_ is https://github.com/opengeospatial/ogcapi-records/commit/35949e6fcd98347d024d28420c8dffd8b9a51c45


## Validator Notebook

You can use the code inside the Jupyter Notebook to validate JSON metadata.

```
cd metadata/schema_validate/
poetry shell
poetry run jupyter notebook
```

Replace the value of the variable `metadata_json_url` with the URL you want to validate.