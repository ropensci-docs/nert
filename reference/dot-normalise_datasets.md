# Resolve the `datasets` argument to a clean alias vector

Resolve the `datasets` argument to a clean alias vector

## Usage

``` r
.normalise_datasets(datasets)
```

## Arguments

- datasets:

  A `character` vector of dataset aliases to collect. (Default=All
  datasets.) Options: `"SMIPS"`, `"ASC"`, `"AET"`, `"AWC"`, `"CLY"`,
  `"SND"`, `"SLT"`, `"BDW"`, `"PHC"`, `"PHW"`, `"NTO"`, `"AVP"`,
  `"PTO"`, `"CEC"`, `"ECE"`, `"DUL"`, `"L15"`, `"SOILDIV"`, `"CANOPY"`,
  `"PHENOLOGY"`. Use `NULL` (default) or `"all"` to specify retrieval of
  all available datasets.

## Value

A `character` vector of recognised aliases (de-duplicated, order
preserved).
