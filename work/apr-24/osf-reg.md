# apr-24 > osf-reg
## abstract
written 11 oct 2023 17.53 belmopan. this document details the expected structure of, expected content of, expected standards for, and expected process for, version 1.5 of dataset ie data series.[^expected by 31 Dec 2024 in at least `github` at [v-1.5](https://github.com/aenavidad/historical-series-re-Belize/tree/main/v-1.5) and `osf` at [version 1.5](https://osf.io/27mx5/). this file copied to `work/apr-24` on 12 apr 2024 shortly before 02.27 benq]

## structure
version 1.5 ought to be composed of exactly six data series ie directories (`calendar`, `chronicle`, `compendium`, `catalogue`, `gazetteer`, `dictionary`) and exactly one descriptive ie introductory text file (`readme.md` or similar text file) and \\(n\\) supplementary text files *referenced* in the `readme` for \\(0\leq n\\) (eg a `licence.md` file referred to in the relevant `readme.md` section) and nothing else.

## content
each data series will contain data ie tabular data ie variable-value pairs and nothing else. the descriptive ie introductiory text file will contain at least -
- preprint content[^eg a la `oct-23/draft.tex`, itself from [[sep-23/draft0.md]] per [[oct-23/log.md]] no 1]
- provenance content
- metadata content[^incl title, URIs, licence, so on]
- versioning content
- introductory content

## standards
routed to `work/apr-24/osf-stds.tsv`, with the following notes.[^sheet created 11 oct 2023 20.58 bmp. previously in `work/oct-23/osf-stds.tsv`]

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
    - iv / `work files` are those in `historical-series-re-Belize/work/*-24` for \* = may, jun, so on, *in addition to* those in `historical-series-re-Belize/work/apr-24` created after \\(n\\) for \\(n\\) = date and time of `osf` registration submission,[^assuming submission in apr 2024 and `work` completed during \\(n\\) to 31 dec 2024.]
    - v / `pre work` is `pre source data` to `pre-git-hist` process,[^occurred oct 2020 to aug 2022.]
    - vi / `pre source data` are the books, papers, databases, manuscripts, and so on, consulted or copied during `pre work`,[^could use with less circular / primitive def here eg specify with ref to exhaustive list of these, possibly including tools / engines / libraries used to access these materials.]
    - vii / `pre work files` are those in `historical-series-re-Belize` and `pre-git-hist` other than `work files` and `v 1.5`.
4. note3 / col 'source' values = 
    - i / AEN at `work/aug-22/rules-20-aug-2022.md` s 3,
    - ii / TOP at https://www.cos.io/initiatives/top-guidelines ie https://www.cos.io/top with more verbose specification of version 1.0.1 at https://osf.io/9f6gx/wiki/home/,[^where possible, reading – article or preprint for 'article', `v 1.5` for 'data', `pre source data` or `source data` or `pre work files` or `work files` for 'materials', `work files` for 'code', `pre work` or `work` for 'design' and 'methods', `work` for 'analysis'.]
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
    - xv / LCT at https://librarycarpentry.org/Top-10-FAIR/2018/12/01/historical-research/,
    - xvi / BWO at https://doi.org/10.1080/00031305.2017.1375989,
    - xvii / DCP at https://datacarpentry.org/spreadsheet-ecology-lesson/,
    - xviii / CWP at https://www.w3.org/TR/tabular-data-primer/,
    - xix / CWM at https://www.w3.org/TR/tabular-data-model/.

## process
for data series -
1. [ ] tag files in `pre git hist` to be used for `v 1.5`[^review `work/*-23` as this task has already been started]
2. [ ] xx

for descriptive ie introductiory text file -
1. [ ] reconstruct chronological log of `pre work`, incl exhaustive list of `pre source data`[^review `work/*-23' as this task has already been started]
2. [ ] xx
