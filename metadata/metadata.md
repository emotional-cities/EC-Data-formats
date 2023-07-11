# Geospatial Metadata

The GIS project metadata is stored in a collection of the OGC API, according to the draft specification of [OGC API Records](https://github.com/opengeospatial/ogcapi-records).

The schema is an extension of the [OGC API Records Metadata Schema](https://github.com/opengeospatial/ogcapi-records/blob/master/core/openapi/schemas/recordGeoJSON.yaml)[^1].

[^1]: Last update from _OGC API Records Metadata Schema_ is https://github.com/opengeospatial/ogcapi-records/commit/35949e6fcd98347d024d28420c8dffd8b9a51c45

## Metadata template

An example of metadata can be found [here](https://github.com/emotional-cities/EC-Data-formats/blob/main/metadata/metadata_example.json) based on [this](https://github.com/opengeospatial/ogcapi-records/blob/5e9c1e20ba1ff1739aa9161a59d1729216750e1f/core/examples/json/record.json)

More examples can be found [here](https://emotional.byteroad.net/collections/ec_catalog/items)

A basic template, to compile a metadata record, can be found [here](https://github.com/emotional-cities/EC-Data-formats/blob/main/metadata/metadata_template.json)

## Metadata schema

The schema definitions are available in two different formats [YAML](https://github.com/emotional-cities/EC-Data-formats/tree/main/metadata/yaml_schemas) and [JSON](https://github.com/emotional-cities/EC-Data-formats/tree/main/metadata/json_schemas). These schemas are useful to validate JSON files, but also as guidance, to get descriptions of different fields.

## Validator Notebook (WIP)

You can use the code inside the Jupyter Notebook to validate JSON metadata.

```
cd metadata/schema_validate/
poetry shell
poetry run jupyter notebook
```
Then run the workbook `schema_validate/validate_metadata.ipynb`

Replace the value of the variable `metadata_json_url` with the URL you want to validate.