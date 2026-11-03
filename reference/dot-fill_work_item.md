# Fetch one work item and write its values into the output table by reference.

For a time-series work item, the row block (`length(coords)` rows) of
each date for the item is filled. For a static work item, the value is
replicated across every date. Failures leave the predeclared `NA` values
untouched and surface as a
[`cli::cli_warn()`](https://cli.r-lib.org/reference/cli_abort.html) with
the underlying error.

## Usage

``` r
.fill_work_item(out, wi, pts, n_dt, n_loc, api_key, max_tries, initial_delay)
```

## Arguments

- out:

  The output `data.table` (modified in place).

- wi:

  A work item from
  [`.build_work_items()`](https://docs.ropensci.org/nert/reference/dot-build_work_items.md).

- pts:

  A `SpatVector` of points.

- n_dt:

  Number of dates.

- n_loc:

  Number of locations.

- api_key:

  A `character` string containing your TERN API key. See
  [`get_key()`](https://docs.ropensci.org/nert/reference/get_key.md) for
  setup.

- max_tries:

  Maximum number of download retries before an error is raised.
  Default=`NULL`, in which case the maximum retry number is resolved
  from the option `nert.max_tries` if that option exists. (Defaults to 3
  retries if `nert.max_tries` has not been set.)

- initial_delay:

  Initial retry delay in seconds. Each later delay is roughly double the
  one before. Default=`NULL`, in which case the initial delay is
  resolved from the option `nert.initial_delay` if that option exists.
  (Defaults to a 1 second initial delay if `nert.initial_delay` has not
  been set.)

## Value

`invisible(NULL)`. This function is called for its side effects.
