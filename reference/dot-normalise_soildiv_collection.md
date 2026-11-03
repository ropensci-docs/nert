# Resolve the 'soildiv_collection' argument to a clean vector

Resolve the 'soildiv_collection' argument to a clean vector

## Usage

``` r
.normalise_soildiv_collection(soildiv_collection)
```

## Arguments

- soildiv_collection:

  *For SOILDIV datasets.* A `character` vector specifying the beta soil
  diversity NMDS axes to be retrieved. (Default=All axes/datasets.)
  Options: `"Bacteria_NMDS1"`, `"Bacteria_NMDS2"`, `"Bacteria_NMDS3"`,
  `"Fungi_NMDS1"`, `"Fungi_NMDS2"`, `"Fungi_NMDS3"`. Use `NULL`
  (default) or `"all"` to specify retrieval of all SOILDIV
  axes/datasets.

## Value

A `character` vector of valid SOILDIV datasets (de-duplicated, order
preserved).
