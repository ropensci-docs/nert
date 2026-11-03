# Normalise a date_range argument

If a `Date` vector or `character` vector of length 2 is given, parses
into a contiguous range of dates. If a vector of length greater than 2
is given, this function does nothing (besides the date conversion).

## Usage

``` r
.parse_date_range(date_range)
```

## Arguments

- date_range:

  A `Date` vector or `character` vector of length 2,
  `[start_date, end_date]`, indicating the start and end date which
  should be used for the TERN dataset retrieval. (If a vector of length
  greater than 2 is given, this parameter works exactly as `dates`
  does.) Omit if specifying exact dates via the `dates` argument
  instead.

## Value

A `Date` vector.
