# Resolve the 'asc_collection' argument to a clean vector

Resolve the 'asc_collection' argument to a clean vector

## Usage

``` r
.normalise_asc_collection(asc_collection)
```

## Arguments

- asc_collection:

  *For ASC datasets.* A `character` vector specifying the Australian
  Soil Classification Map datasets to be retrieved. (Default=All ASC
  datasets.) Options: `"EV"` (estimated soil order), `"CI"` (confusion
  index). Use `NULL` (default) or `"all"` to specify retrieval of all
  ASC datasets.

## Value

A `character` vector of valid ASC datasets (de-duplicated, order
preserved).
