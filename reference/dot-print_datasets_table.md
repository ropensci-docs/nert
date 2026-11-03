# Print the user-facing datasets-table summarising what will be fetched.

Print the user-facing datasets-table summarising what will be fetched.

## Usage

``` r
.print_datasets_table(
  datasets,
  depth,
  stat,
  smips_collection,
  asc_collection,
  aet_collection,
  soildiv_collection,
  phenology_collection,
  canopy_collection
)
```

## Arguments

- datasets:

  A `character` vector of dataset aliases to collect. (Default=All
  datasets.) Options: `"SMIPS"`, `"ASC"`, `"AET"`, `"AWC"`, `"CLY"`,
  `"SND"`, `"SLT"`, `"BDW"`, `"PHC"`, `"PHW"`, `"NTO"`, `"AVP"`,
  `"PTO"`, `"CEC"`, `"ECE"`, `"DUL"`, `"L15"`, `"SOILDIV"`, `"CANOPY"`,
  `"PHENOLOGY"`. Use `NULL` (default) or `"all"` to specify retrieval of
  all available datasets.

- depth:

  *For SLGA datasets.* A `character` vector containing the depth
  interval(s) for the SLGA soil attributes to collect. (Default=All
  depths.) Options: `"000_005"`, `"005_015"`, `"015_030"`, `"030_060"`,
  `"060_100"`, `"100_200"`. Use `NULL` (default) or `"all"` to specify
  retrieval of all available depths. This parameter is ignored for
  non-SLGA datasets.

- stat:

  *For SLGA datasets.* A `character` vector containing the statistic to
  retrieve for the SLGA datasets. (Default=All statistics.) Options:
  `"EV"` (estimated value), `"05"` (lower, 5th-percentile bound), `"95"`
  (upper, 95th-percentile bound); the `05` and `95` layers together span
  a 90% interval. Use `NULL` (default) or `"all"` to specify retrieval
  of all statistics. This parameter is ignored for non-SLGA datasets.

- smips_collection:

  *For SMIPS datasets.* A `character` vector containing the SMIPS
  datasets to be retrieved. (Default=All SMIPS datasets.) Options:
  `"totalbucket"`, `"SMindex"`, `"bucket1"`, `"bucket2"`, `"deepD"`,
  `"runoff"`. Use `NULL` (default) or `"all"` to specify retrieval of
  all SMIPS datasets. This parameter is ignored for non-SMIPS datasets.

- asc_collection:

  *For ASC datasets.* A `character` vector specifying the Australian
  Soil Classification Map datasets to be retrieved. (Default=All ASC
  datasets.) Options: `"EV"` (estimated soil order), `"CI"` (confusion
  index). Use `NULL` (default) or `"all"` to specify retrieval of all
  ASC datasets.

- aet_collection:

  *For AET datasets.* A `character` vector specifying the Actual
  Evapotranspiration datasets to be retrieved. (Default=All AET
  datasets.) Options: `"ETa"`, `"pixel_qa"` (quality assurance flags).
  Use `NULL` (default) or `"all"` to specify retrieval of all AET
  datasets. This parameter is ignored for non-AET datasets.

- soildiv_collection:

  *For SOILDIV datasets.* A `character` vector specifying the beta soil
  diversity NMDS axes to be retrieved. (Default=All axes/datasets.)
  Options: `"Bacteria_NMDS1"`, `"Bacteria_NMDS2"`, `"Bacteria_NMDS3"`,
  `"Fungi_NMDS1"`, `"Fungi_NMDS2"`, `"Fungi_NMDS3"`. Use `NULL`
  (default) or `"all"` to specify retrieval of all SOILDIV
  axes/datasets.

- phenology_collection:

  *For PHENOLOGY datasets.* A `character` vector specifying the
  phenology datasets to be retrieved. (Default=All PHENOLOGY datasets.)
  Options: `"SGS"`, `"PGS"`, `"EGS"`, `"LGS"`, `"EVI1"`, `"EVI2"`,
  `"EVIP"`, `"EVII"`, `"SGS_month"`, `"PGS_month"`, `"EGS_month"`. Use
  `NULL` (default) or `"all"` to specify retrieval of all PHENOLOGY
  datasets.

- canopy_collection:

  *For CANOPY datasets.* A `character` vector specifying the OzTreeMap
  canopy height composite(s) to be retrieved. (Default=All CANOPY
  datasets.) Options: `"best_pick"`, `"median"`. Use `NULL` (default) or
  `"all"` to specify retrieval of all CANOPY datasets. This parameter is
  ignored for non-CANOPY datasets.

## Value

`invisible(NULL)`. This function is called for its side effects.
