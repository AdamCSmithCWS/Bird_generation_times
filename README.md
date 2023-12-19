Simple set of scripts to set the generation lengths for all of the taxonomic units (aka species) in the North American Breeding Bird Survey database.

The scripts imports the generation lengths published in [Bird et al. 2020](https://doi.org/10.1111/cobi.13486), then matches the generation lengths to the species units used by the BBS, based on the R package [bbsBayes2](https://github.com/bbsBayes/bbsBayes2/). The matching is based on scientific names first and then non-matches are corrected based on:

1.  alternate common english names that align in the two databases (\~ 20 species)

2.  a series of manual joins, based on recent updates to taxonomy or reconciling AOS checklist with the taxonomy used in Bird et al. These manual joins are scripted and explicit in the code.
