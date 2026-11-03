# Resolve the 'stat' argument to a clean vector

Resolve the 'stat' argument to a clean vector

## Usage

``` r
.normalise_stat(stat)
```

## Arguments

- stat:

  *For SLGA datasets.* A `character` vector containing the statistic to
  retrieve for the SLGA datasets. (Default=All statistics.) Options:
  `"EV"` (estimated value), `"05"` (lower, 5th-percentile bound), `"95"`
  (upper, 95th-percentile bound); the `05` and `95` layers together span
  a 90% interval. Use `NULL` (default) or `"all"` to specify retrieval
  of all statistics. This parameter is ignored for non-SLGA datasets.

## Value

A `character` vector of valid statistics (de-duplicated, order
preserved).
