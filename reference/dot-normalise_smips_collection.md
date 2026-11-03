# Resolve the 'smips_collection' argument to a clean vector

Resolve the 'smips_collection' argument to a clean vector

## Usage

``` r
.normalise_smips_collection(smips_collection)
```

## Arguments

- smips_collection:

  *For SMIPS datasets.* A `character` vector containing the SMIPS
  datasets to be retrieved. (Default=All SMIPS datasets.) Options:
  `"totalbucket"`, `"SMindex"`, `"bucket1"`, `"bucket2"`, `"deepD"`,
  `"runoff"`. Use `NULL` (default) or `"all"` to specify retrieval of
  all SMIPS datasets. This parameter is ignored for non-SMIPS datasets.

## Value

A `character` vector of valid SMIPS datasets (de-duplicated, order
preserved).
