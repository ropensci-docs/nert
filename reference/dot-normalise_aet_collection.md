# Resolve the 'aet_collection' argument to a clean vector

Resolve the 'aet_collection' argument to a clean vector

## Usage

``` r
.normalise_aet_collection(aet_collection)
```

## Arguments

- aet_collection:

  *For AET datasets.* A `character` vector specifying the Actual
  Evapotranspiration datasets to be retrieved. (Default=All AET
  datasets.) Options: `"ETa"`, `"pixel_qa"` (quality assurance flags).
  Use `NULL` (default) or `"all"` to specify retrieval of all AET
  datasets. This parameter is ignored for non-AET datasets.

## Value

A `character` vector of valid AET datasets (de-duplicated, order
preserved).
