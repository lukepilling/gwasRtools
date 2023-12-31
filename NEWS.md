# gwasRtools 0.1.3 (27 Nov 2023)

* `get_loci()` now has the option `exclude_hla` to treat the HLA region as one continuous locus (default = FALSE). Coordinates are specified with `hla_pos = c(25e6, 34e6)` [these are the defaults]
* Minor documentation updates

# gwasRtools 0.1.2 (15 Sept 2023)

* Added `gwas_example` data for running examples
* `get_loci()` Genetic loci are now defined around variants with p-value < 5 × 10−8. The locus borders were set 500kb (`n_bases`) to each side of the highest genome-wide significant variant in each region. 
* `get_loci()` "lead" column is the best lead SNP from distance (i.e., all input SNPs) or from LD clumping (subset in reference dataset panel)
* Fixes for `get_loci()` niche cases
* Fixes for `get_nearest_gene()` niche cases

# gwasRtools 0.1.1 (30 Aug 2023)

* Fix internal -log10p calculation
* Swap most "Depends" to "Imports"
* Add dependency for {ieugwasr}
* Add `ld_clump` option to `get_loci()` function, to get independent SNPs at the same locus
* Add `use_pvalue` option to `get_loci()` function

# gwasRtools 0.1.0 (30 June 2023)

* Added a `NEWS.md` file to track changes to the package.
