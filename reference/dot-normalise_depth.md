# Resolve the 'depth' argument to a clean vector

Resolve the 'depth' argument to a clean vector

## Usage

``` r
.normalise_depth(depth)
```

## Arguments

- depth:

  *For SLGA datasets.* A `character` vector containing the depth
  interval(s) for the SLGA soil attributes to collect. (Default=All
  depths.) Options: `"000_005"`, `"005_015"`, `"015_030"`, `"030_060"`,
  `"060_100"`, `"100_200"`. Use `NULL` (default) or `"all"` to specify
  retrieval of all available depths. This parameter is ignored for
  non-SLGA datasets.

## Value

A `character` vector of valid soil depths (de-duplicated, order
preserved).
