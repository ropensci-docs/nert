# Internal handler for retrieving the AET data

Internal handler for retrieving the AET data

## Usage

``` r
.read_tern_aet(did, dots, api_key, max_tries, initial_delay)
```

## Arguments

- did:

  Normalised 8-char dataset ID (unused; uniform handler signature).

- dots:

  Named list of `...` args from
  [`read_tern()`](https://docs.ropensci.org/nert/reference/read_tern.md).

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

A
[terra::SpatRaster](https://rspatial.github.io/terra/reference/SpatRaster-class.html)
object for the requested AET collection/date.
