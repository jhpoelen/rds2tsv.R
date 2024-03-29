# [rds2tsv.R](./rds2tsv.R)
Streams R Data Serialized (rds) format from stdin to stdout in tab-separated-values (tsv) using R

# Install

```bash
sudo sh -c 'curl -L https://raw.githubusercontent.com/jhpoelen/rds2tsv.R/main/rds2tsv.R > /usr/local/bin/rds2tsv.R && chmod +x /usr/local/bin/rds2tsv.R'
```

:warning: please inspect this install script before running it.

# Example

```bash 
curl -L https://open.flinders.edu.au/ndownloader/files/43331472\
 | ./rds2tsv.R\
 > beeTaxonomy.tsv
```

with first 2 lines of beeTaxonomy.tsv being:

| flags | taxonomic_status | source | accid | id | kingdom | phylum | class | order | family | subfamily | tribe | subtribe | validName | canonical | canonical_withFlags | genus | subgenus | species | infraspecies | authorship | taxon_rank | valid | notes |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|  | accepted | DiscoverLife | 0 | 4 | Animalia | Arthropoda | Insecta | Hymenoptera | Andrenidae | Panurginae | Calliopsini |  | Acamptopoeum argentinum (Friese, 1906) | Acamptopoeum argentinum | Acamptopoeum argentinum | Acamptopoeum |  | argentinum |  | (Friese, 1906) | Species | TRUE |  |

with data found in:

> Dorey, J.B., Fischer, E.E., Chesshire, P.R. et al. A globally synthesised and flagged bee occurrence dataset and cleaning workflow. Sci Data 10, 747 (2023). https://doi.org/10.1038/s41597-023-02626-w

