# Validate phenology arguments before the API key is checked

Phenology requires an integer `year` in 2003–2018. The `season` and
`collection` arguments are optional and validated downstream in the
handler. Invoked by
[`read_tern()`](https://docs.ropensci.org/nert/reference/read_tern.md)
via the
[.tern_datasets](https://docs.ropensci.org/nert/reference/dot-tern_datasets.md)
registry.

## Usage

``` r
.validate_phenology(dots, dataset_id)
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
