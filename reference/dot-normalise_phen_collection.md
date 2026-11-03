# Resolve the 'phenology_collection' argument to a clean vector

Resolve the 'phenology_collection' argument to a clean vector

## Usage

``` r
.normalise_phen_collection(phenology_collection)
```

## Arguments

- phenology_collection:

  *For PHENOLOGY datasets.* A `character` vector specifying the
  phenology datasets to be retrieved. (Default=All PHENOLOGY datasets.)
  Options: `"SGS"`, `"PGS"`, `"EGS"`, `"LGS"`, `"EVI1"`, `"EVI2"`,
  `"EVIP"`, `"EVII"`, `"SGS_month"`, `"PGS_month"`, `"EGS_month"`. Use
  `NULL` (default) or `"all"` to specify retrieval of all PHENOLOGY
  datasets.

## Value

A `character` vector of valid PHENOLOGY datasets (de-duplicated, order
preserved).
