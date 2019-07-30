# SDG Build

[![Build Status](https://travis-ci.com/open-sdg/sdg-build.svg?branch=master)](https://travis-ci.org/open-sdg/sdg-build)

SDG Build is a Python package for converting data on the Sustainable Development Goals (SDG) from one format into another. This is mainly useful to an SDG reporting platform, by providing these benefits:

1. Input of SDG data from various machine-readable formats, for human-friendly visualisation and display
2. Output of SDG data to various machine-readable formats, for interoperability with other systems
3. Validation of the data and metadata for quality control

## Inputs

SDG Build can **input** SDG data in the following formats:

* Data in CSV files (long/tidy format)
* Metadata in YAML files
* Data (and minimal metadata) from SDMX-JSON and SDMX-ML

## Ouputs

SDG Build can **output** SDG data in the following formats:

* A particular JSON structure for data and metadata, expected by the [Open SDG](https://github.com/open-sdg/open-sdg) reporting platform.

## Schemas

SDG Build requires a schema for any metadata. Currently the following formats are supported:

* YAML schema intended for Prose.io

## Upcoming integrations

Other inputs and outputs are either under development or planned for the future:

* Input and output from/to SDMX, both SDMX-JSON and SDMX-ML
* Input and output from/to CSV-W
* Input and output from/to GeoJSON

## Usage

Usage examples are available in `docs/examples`. In each of these examples, the output is generated in a `_site` folder. Before running these examples, make sure to run:

```
pip install -r docs/examples/requirements.txt
```

### Example #1: CSV + YAML to Open SDG

An example conversion from CSV data and YAML metadata into JSON suitable for the Open SDG platform:

```
python docs/examples/open_sdg.py
```

### Example #2: SDMX-JSON to Open SDG

An example conversion from SDMX-JSON (from an API endpoint) into JSON suitable for the Open SDG platform:

```
python docs/examples/sdmx_json.py
```

### Example #3: SDMX-ML to Open SDG

An example conversion from SDMX-ML into JSON suitable for the Open SDG platform:

```
python docs/examples/sdmx_ml.py
```

## License

MIT © Office for National Statistics
