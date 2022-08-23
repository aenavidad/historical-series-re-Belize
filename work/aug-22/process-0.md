# process

## abstract

this file is intended to finalise work process and output standards as gathered in prior files.[^inc in order of preference [[standards.md]] and [[algorithmic.md]]. this file created 16 aug 2022 15.10 in Boston MA.]

note

- `pre-git-work` is relevant work during 1 oct 2020 to 8 aug 2022 which resulted in `pre-git-files` inc `v-1.4` of data,[^ie all files in [`git/pre-git-hist/files`](https://github.com/aenavidad/pre-git-hist/tree/main/files) ie all files in [`osf/working-files/oct-20-to-jul-22`](https://osf.io/7ujq5/). further `v-1.4` files copied to `git/historical-series-re-Belize/v-1.4` and to `osf/v-1.4` and to `osf/version_1.4`. original (private) deposit of `v-1.4` files in `harvard_dataverse/version_1.4`.]
- `pre-work` is relevant work during 9 aug 2022 to 17 aug 2022 resulting in `pre-work-files`,[^ie three files in [`pre-git-hist`](https://github.com/aenavidad/pre-git-hist) which aren't in `/files` and all files in [`historical-series-re-Belize/work`](https://github.com/aenavidad/historical-series-re-Belize/tree/aug-work/work) and the `readme` files in `/v-1.4` and `/v-1.5` of [`historical-series-re-Belize`.](https://github.com/aenavidad/historical-series-re-Belize/tree/main).]
- `work` is relevant work during 18 aug 2022 to 1 sep 2022 resulting in `work-files` inc `v-1.5` of data,
- `post-work` is relevant work during 1 sep 2022 to 15 sep 2022 resulting in `pre-print` manuscript inc any supplements,
- `standards` are those standards made or adopted for `work` and `post-work` inc their output,

## pre-work

start[^started 9 aug 2022 in Boston MA upon adoption of `git` for version-control.]

1. adopt `git` for version control,
2. flag all local files output from `pre-git-work`,
3. translate flagged files to `tsv` and related formats,
4. archive translated files as `pre-git-files`,
5. write relevant `readme` files,
6. flag all third-party standards relevant to `work`,
7. adopt `osf` for archiving,
8. start `osf` registration for `work`,
9. write `process` file.

end

## work

start[^started 16 aug 2022 in Boston MA upon writing [[standards]].]

1. complete `process` file,[^inc all standards and relevant info from [[algorithmic.md]], [[output.md]], [[prospectus.md]], [[standards.md]].]
2. complete `osf` registration for `work`,
3. start `log` file,[^to log each working session inc date-times, `git` and `osf` checks, actions started or complete, and specifications of these.]
4. if `v-1.5` exists, skip to step 9, else to step 5,
5. log session start,[^inc routine checks]
6. run session,[^where sessions are expected to involve at least all of - querying `v-1.4` and `pre-git-hist/files` for files to be mined, extracting data from tagged files, cleaning ie standardising these data, building metadata, filling gaps in data and metadata, modelling these as a graph.]
7. log session end,[^inc routine checks]
8. return to step 4,
9. verify `standards` compliance,
10. complete `log` file.

end

## post-work

start

1. draft `pre-print`,
2. distribute `pre-print`.

end

## standards

note references to sec standards of [[standards.md]] used in the `from` columns in this section.

| no | standard | from |
|:--|:--|:--|:--|
| 1 | `work` must be replicable | vars |
| 2 | `v-1.5` must be human-readable | Mandakers & Hoekstra 2004 C9 |
| 3 | `v-1.5` must be machine-readable | dwbp bp 12, ld-bp no 3, ld-bp no 7, Open Definition sec 1.3, Open Definition sec 1.4, dwbp bp 13, dwbp bp 14, dwbp bp 15, dwbp bp 16, ld-bp no 6, Mandakers & Hoekstra 2004 C5, Mandakers & Hoekstra 2004 C7, IDS Best Practices re research sec ontologies, FAIR I1 |

### no 1

| no | standard | from |
|:--|:--|:--|
| 1.1 | `work-files` must cite sources | TOP no 1 lvl iii, webarch sec 2.1, webarch sec 2.4, webarch sec 3.5, webarch sec 3.5.1, dwbp bp 5, dwbp bp 34, dwbp bp 35, prov attribution, FAIR F1 |
| 1.2 | `work-files` must be archived | TOP no 2 lvl ii, TOP no 3 lvl ii, TOP no 4 lvl ii, Open Definition sec 1.2, Mandakers & Hoekstra 2004 B8 |
| 1.3 | `pre-print` must report `log` | TOP no 5 lvl iii, dwbp bp 22, dwbp bp 31, prov process, prov justification, Mandakers & Hoekstra 2004 C6, Hoekstra & Koolen 2019 sec 1 |
| 1.4 | `work` must be registered | TOP no 7 lvl i |
| 1.5 | `pre-git-files` and `pre-work-files` and `work-files` must be licensed | dwbp bp 4, ld-bp no 4 |
| 1.6 | `work-files` must be citeable | dwbp bp 7, dwbp bp 9, dwbp bp 10, dwbp bp 11, ld-bp no 5, prov object, FAIR F3 |
| 1.7 | `v-1.5` must inc metadata | dwbp bp 1, dwbp bp 2, dwbp bp 6, dwbp bp 28, dwbp bp 3, Frictionless Standards re package std introduction, Frictionless Standards re package std descriptor, Frictionless Standards re resource std introduction, Mandakers & Hoekstra 2004 A1, FAIR F2, FAIR R1 |

### third-party

adopted third party standards[^from [[standards.md]] as of 16 aug 2022 18.37.]

| standards | no | note |
|:--|:--|:--|
| COS TOP | no 1 lvl iii | `work-files` or `pre-print` must appropriately cite[^ie must cite datasets and programme codes used in `work` or `post-work`, where citation should (may) inc persistent identifier.] |
| COS TOP | no 2 lvl ii | `null` |
| COS TOP | no 3 lvl ii | `null` |
| COS TOP | no 4 lvl ii | `null` |
| COS TOP | no 5 lvl iii | `null` |
| COS TOP | no 7 lvl i | `null` |
| W3C webarch | sec 2.1 | `null` |
| W3C webarch | sec 2.4 | `null` |
| W3C webarch | sec 3.5[^inc sec 3.5.1] | `null` |
| W3C dwbp | bp 1 | `null` |
| W3C dwbp | bp 2 | `null` |
| W3C dwbp | bp 3 | `null` |
| W3C dwbp | bp 4 | `null` |
| W3C dwbp | bp 5 | `null` |
| W3C dwbp | bp 6 | `null` |
| W3C dwbp | bp 7 | `null` |
| W3C dwbp | bp 9 | `null` |
| W3C dwbp | bp 10 | `null` |
| W3C dwbp | bp 11 | `null` |
| W3C dwbp | bp 12 | `null` |
| W3C dwbp | bp 13 | `null` |
| W3C dwbp | bp 14 | `null` |
| W3C dwbp | bp 15 | `null` |
| W3C dwbp | bp 16 | `null` |
| W3C dwbp | bp 22 | `null` |
| W3C dwbp | bp 28 | `null` |
| W3C dwbp | bp 31 | `null` |
| W3C dwbp | bp 34 | `null` |
| W3C dwbp | bp 35 | `null` |
| W3C ld-bp | no 3 | `null` |
| W3C ld-bp | no 4 | `null` |
| W3C ld-bp | no 5 | `null` |
| W3C ld-bp | no 6 | `null` |
| W3C ld-bp | no 7 | `null` |
| W3C prov | object | `null` |
| W3C prov | attribution | `null` |
| W3C prov | process | `null` |
| W3C prov | justification | `null` |
| OKF Frictionless Std | re package std intro | `null` |
| OKF Frictionless Std | re package std descriptor | `null` |
| OKF Frictionless Std | re resource std intro | `null` |
| OKF Open Def | sec 1.2 | `null` |
| OKF Open Def | sec 1.3 | `null` |
| OKF Open Def | sec 1.4 | `null` |
| Mandakers & Dillon | A1 | `null` |
| Mandakers & Dillon | B1 | `null` |
| Mandakers & Dillon | B8 | `null` |
| Mandakers & Dillon | C5 | `null` |
| Mandakers & Dillon | C6 | `null` |
| Mandakers & Dillon | C7 | `null` |
| Mandakers & Dillon | C9 | `null` |
| Hoekstra & Koolen | sec 1 | `null` |
| IDS Best Practices | re research sec ontologies | `null` |
| GFISCO FAIR | F1 | `null` |
| GFISCO FAIR | F2 | `null` |
| GFISCO FAIR | F3 | `null` |
| GFISCO FAIR | I1 | `null` |
| GFISCO FAIR | R1 | `null` |