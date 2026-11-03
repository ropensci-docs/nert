# Resolve the 'canopy_collection' argument to a clean vector

Resolve the 'canopy_collection' argument to a clean vector

## Usage

``` r
.normalise_canopy_collection(canopy_collection)
```

## Arguments

- canopy_collection:

  *For CANOPY datasets.* A `character` vector specifying the OzTreeMap
  canopy height composite(s) to be retrieved. (Default=All CANOPY
  datasets.) Options: `"best_pick"`, `"median"`. Use `NULL` (default) or
  `"all"` to specify retrieval of all CANOPY datasets. This parameter is
  ignored for non-CANOPY datasets.

## Value

A `character` vector of valid CANOPY datasets (de-duplicated, order
preserved).
