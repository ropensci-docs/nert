# Normalise coordinate input

Normalise coordinate input

## Usage

``` r
.parse_coordinates(lon, lat, xy)
```

## Arguments

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

A 2-column `data.table` with columns `lon`, `lat`.
