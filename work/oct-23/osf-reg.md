# oct-23 > osf-reg
## abstract
written 11 oct 2023 17.53 belmopan. this document details the expected structure of, expected content of, expected standards for, and expected process for, version 1.5 of dataset ie data series.[^expected by 31 Dec 2023 in at least `github` at [v-1.5](https://github.com/aenavidad/historical-series-re-Belize/tree/main/v-1.5) and `osf` at [version 1.5](https://osf.io/27mx5/).]

## structure
version 1.5 ought to be composed of exactly six data series ie directories (`calendar`, `chronicle`, `compendium`, `catalogue`, `gazetteer`, `dictionary`) and exactly one descriptive ie introductory text file (`readme.md` or similar text file) and \\(n\\) supplementary text files *referenced* in the `readme` for \\(0\leq n\\) (eg a `licence.md` file referred to in the relevant `readme.md` section) and nothing else.

## content
xx

## standards
routed to `work/oct-23/osf-stds.tsv`, with the following notes.[^sheet created 11 oct 2023 20.58 bmp.]

1. note0 / conventions, etc = 
    - i / 'na' and '999' are null vals, cols with names starting in '\*' are working cols,
    - ii / col 'no' identifies the corresponding standard number per `work/aug-22/rules-20-aug-2022.tsv` for nos=1-316 or assigns an identifying number for the same if not available, 
    - iii / col 'top' identifies the subsuming top level ie first order standard from nos=1-3, 
    - iv / col 'varid' identifies the standard by a variant id eg that assigned by the source of the standard,
    - v / col 'source' identifies the standard's original source. 
2. note1 / sources = 
    - i / nos=1-10, 400 from `work/aug-22/rules-20-aug-2022.md` s 3,
    - ii / nos=1-316 from `work/aug-22/rules-20-aug-2022.tsv`.[^with col 'varid' vals adapted from col 'standard' vals, and col 'adoption' vals 'full' or 'part' from col 'adoption' val 'yes', and val 'none' from val 'no']
3. note2 / defined terms in cols 'standard', 'elucidation', 'notes' = 
    - i / `work` is `pre-git-hist` to `historical-series-re-Belize/v-1.5` process,[^occurring oct 2023 to dec 2023, assuming `work` completion by 31 dec 2023.] 
    - ii / `v 1.5` is `historical-series-re-Belize/v-1.5`, 
    - iii / `source data` is `pre-git-hist`, 
    - iv / `work files` are those in `historical-series-re-Belize/work/*-23` for \* = nov or dec *in addition to* those in `historical-series-re-Belize/work/oct-23` created after \\(n\\) for \\(n\\) = date and time of `osf` registration submission,[^assuming submission in oct 2023 and `work` completed during \\(n\\) to 31 dec 2023.]
    - v / `pre work` is process to `pre-git-hist`.[^occurred oct 2020 to aug 2022.]
4. note3 / col 'source' values = 
    - i / AEN at `work/aug-22/rules-20-aug-2022.md` s 3,
    - ii / TOP at https://www.cos.io/initiatives/top-guidelines ie https://www.cos.io/top with more verbose specification of version 1.0.1 at https://osf.io/9f6gx/wiki/home/,[^where possible, reading – article or preprint for 'article', `v 1.5` for 'data', `source data` or `work files` for 'materials', `work files` for 'code'.]
    - iii / AWI at http://www.w3.org/TR/webarch/,
    - iv / NDP at https://web.archive.org/web/20220808095409/https://www.springernature.com/gp/authors/research-data-policy/,[^archived content significantly different to live version]
    - v / DWP at https://www.w3.org/TR/dwbp/,
    - vi / LDP at http://www.w3.org/TR/ld-bp/
    - vii / PXG at http://www.w3.org/2005/Incubator/prov/XGR-prov/,
    - viii / OFS at https://specs.frictionlessdata.io/data-resource/ and https://specs.frictionlessdata.io/data-package/,
    - ix / OOD at https://opendefinition.org/od/2.1/en/
    - x / MDP at https://doi.org/10.3200/HMTS.37.1.34-38,
    - xi / HKD at https://doi.org/10.1080/01615440.2018.1484676,
    - xii / IDP at https://maastrichtu-ids.github.io/best-practices/docs/,
    - xiii / FAI at https://www.go-fair.org/fair-principles/,
    - xiv / PSG at http://www.psychologicalscience.org/publications/psychological_science/ps-submissions,
    - xv / LCT at https://librarycarpentry.org/Top-10-FAIR/2018/12/01/historical-research/.

## process
xx
