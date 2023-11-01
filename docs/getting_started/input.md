# Input

MZmine's takes MS data files as input. Several MS data formats are supported (see [below](#supported-data-formats)). MS data files can be either viusally explored through several [visualization modules](../data_visualization/index.md), or processed to extract [feature lists and spectral file summaries](output.md).

## Supported data formats

MZmine supports both open and proprietary formats. In particular:

**Open formats**:

- `mzML`
- `imzML`
- `mzXML`
- `mzData`
- `netCDF`
- `aird`

**Proprietary formats**:

- Thermo Scientific (`.raw`)
- Bruker Daltonics (`.d`, `.tdf`/`.tsf`)

Raw data files from non-supported vendors must be converted to open format prior to import in MZmine (see [Data conversion](data_conversion.md) section).

## Data handling recommendations

- **LC-MS and LC-IMS-MS**. Always convert the raw data to centroided `mzML` format, except for timsTOF data, for which we recommend using the native Bruker format.
- **MS imaging**. Always convert raw data to `.imzML` format, except for timsTOF fleX data, for which we recommend using the native Bruker format.
