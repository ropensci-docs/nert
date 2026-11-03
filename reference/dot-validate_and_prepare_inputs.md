# Validate and prepare date and coordinate inputs

Validates and resolves the `dates`/`date_range` arguments and parses the
coordinate inputs into a `SpatVector` of points.

## Usage

``` r
.validate_and_prepare_inputs(dates, date_range, lon, lat, xy)
```

## Arguments

- dates:

  A `Date` vector or `character` vector, indicating the exact set of
  dates for which TERN datasets should be retrieved. Takes precedence
  over `date_range` if supplied.

- date_range:

  A `Date` vector or `character` vector of length 2,
  `[start_date, end_date]`, indicating the start and end date which
  should be used for the TERN dataset retrieval. (If a vector of length
  greater than 2 is given, this parameter works exactly as `dates`
  does.) Omit if specifying exact dates via the `dates` argument
  instead.

- lon:

  Longitude(s) (WGS84, EPSG:4326). Numeric scalar or vector (same length
  as `lat`). Omit if using `xy` notation.

- lat:

  Latitude(s) (WGS84, EPSG:4326). Numeric scalar or vector (same length
  as `lon`). Omit if using `xy` notation.

- xy:

  Optional: a `data.frame`, `data.table`, or `matrix` with coordinate
  columns named `lon`/`lat` or `x`/`y`. Takes precedence over
  `lon`/`lat` when supplied.

## Value

A named list with elements `dates`, `n_dt`, `coords_df`, `n_loc`, and
`pts`.
