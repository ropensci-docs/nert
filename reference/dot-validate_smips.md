# Validate SMIPS arguments before the API key is checked

SMIPS requires a daily `date` (the legacy `day` name is also accepted).
Invoked by
[`read_tern()`](https://docs.ropensci.org/nert/reference/read_tern.md)
via the
[.tern_datasets](https://docs.ropensci.org/nert/reference/dot-tern_datasets.md)
registry.

## Usage

``` r
.validate_smips(dots, dataset_id)
```

## Arguments

- dots:

  Named list of `...` args from
  [`read_tern()`](https://docs.ropensci.org/nert/reference/read_tern.md).

- dataset_id:

  A `character` string identifying the dataset. Accepts a short alias,
  the full TERN portal key (e.g.\\
  `"TERN/d1995ee8-53f0-4a7d-91c2-ad5e4a23e5e0"`), or the 8-character key
  prefix (e.g.\\ `"TERN/d1995ee8"`). See the **Dataset aliases** section
  for the complete table of supported aliases.

## Value

`NULL`; called for its side effects (argument validation).
