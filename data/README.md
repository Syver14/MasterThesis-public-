# Data Files

This folder contains the CSV input data used by the main analysis notebook.

## Files

- `water_content_raw.csv` - oven-drying measurements used to calculate water content.
- `pycnometer_processed.csv` - processed particle-density measurements from the pycnometer workflow.
- `dry_sieve_raw.csv` - retained masses from dry sieve tests.
- `wet_sieve_raw.csv` - retained masses from wet-prepared sieve tests.
- `hydrometer_bulk_raw.csv` - raw bulk hydrometer readings.
- `hydrometer_fines_raw.csv` - raw fines-only hydrometer readings.
- `hydrometer_constants.csv` - constants used for the hydrometer calculations in the notebook.
- `hydrometer_astm152h_constants.csv` - ASTM 152H hydrometer constants in CSV form.
- `loose_tapped_raw.csv` - loose and tapped bulk-density measurements.
- `mgs1_percentiles_long_fox_britt_2023.csv` - MGS-1 reference particle-size percentiles.
- `mineral_composition.csv` - mineralogical composition and density assumptions used for the particle-density plausibility check.

## Notes

Only CSV files are required to reproduce the analysis in the repository. Source spreadsheets and laboratory templates are not included in this public data folder.

The thesis describes the laboratory procedures, data processing assumptions, and method deviations. These CSV files are provided to make the calculation and plotting workflow auditable.
