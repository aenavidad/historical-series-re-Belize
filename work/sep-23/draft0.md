---
Created: 24 September 2023 13.36 Belmopan
Abstract: This is a draft of the preprint, ie draft number 0 ie the first draft available in the `work/sep-23` directory.
---

# sep-23/draft0

## abstract [s 1]
xx

## acknowledgements [s 2]
xx

## introduction [s 3]
xx

## context [s 4]
xx

### working model of historical reasoning [s 4.1]
What is the model of reasoning being kept in mind for this section regarding context of historical literature? 

Assume the said reasoning is *not monotonic*. Then, we would like to know what exactly is in \\(E\\) for \\(E \vDash c\\) where \\(E\\) is a set of evidence and \\(c\\) a claim. Or rather what all *could* be in \\(E\\).

First, building on `pre-git-hist/files/oran/found data 1.2 Partitions 6-*.tsv`, for *work*, *manifestation* as in frbr:work, frbr:manifestation, we might partition \\(E\\) as follows.

```
level . partitions . notes
0 . evidence .
1 . evidence - work not . (i), (ii)
1 . evidence - work . (iii)
2 . evidence - work - manifestation not . (iv)
2 . evidence - work - manifestation .

notes
(i) an earlier version of this level used the *is extant* before the *is work* relation. however, membership in the *evidence - extant not* collection would be known or deemed likely via some evidence in the *evidence - extant* bin, such that the *is extant* relations seems a bit unnecessary eg Classic Mayan codices
(ii) eg archaeological, palaeolithic, etc
(iii) inc textual and non-textual, published and otherwise, recorded and otherwise, etc
(iv) eg unrecorded oral history still being orally realised, etc 
```

Partition of the `evidence - work - manifestation` ie \\(E_i\\) collection might proceed in a number of useful ways. The following are some examples.

```
eg . lvl . partitions . notes
0 . 3 . E_i - published not . (i)
0 . 3 . E_i - published . 
1 . 3 . E_i - textual not . (ii)
1 . 3 . E_i - textual .
2 . 3 . E_i - digital not . (iii)
2 . 3 . E_i - digital . (iv)

notes
(i) eg manuscripts, etc
(ii) ie *mostly* not textual eg maps, recordings, paintings
(iii) ie manifestations with no digital item eg undigitised books, etc
(iv) inc born digital works
```

The following are some further useful partitions of some of the aforementioned level 3 collections.

```
eg . lvl . partitions . notes
0 . 4 . E_1 - published - historical not . (i)
0 . 4 . E_1 - published - historical .
0 . 4 . E_1 - published - official not . (ii)
0 . 4 . E_1 - published - official .

notes
(i) ie publications which are *not* historical works or works by historians eg archaeological literature
(ii) ie publications *not* published by crown nor parliament ie non-state publications
```

### table [s 4.2]
Given \\(E\\) as above outlined, we may now characterise the works we would like v 1.5 to comprise of, for *works* as [frbr:work](https://www.ifla.org/references/best-practice-for-national-bibliographic-agencies-in-a-digital-age/resource-description-and-standards/bibliographic-control/functional-requirements-the-frbr-family-of-models/functional-requirements-for-bibliographic-records-frbr/) *or* [ioa:information content entity](http://purl.obolibrary.org/obo/IAO_0000030).

| type | for | prev | v 1.4 | notes |
|:--|:--|:--|:--|:--|
| calendar | well used archives[^Belize ARS, UK TNA, Spain AGI] | sort of[^Burdon's *Archives*, UK Calendar, etc] | a bit[^in 'Cartas' series, some extracts in 'Events'] | - |
| calendar | poorly used archives[^Local parish ones, etc] | sort of[^some calendars exist, some catalogued, others not] | not in | - |
| chronicle | pre 17th cent | ? | a bit[^for 16th cent in 'Events'] | - |
| chronicle | post 16th cent | ? | yes | but possy not up to par[^eg has no coding info] |
| statistics | all | sort of[^disjoint series in literature] | yes | but not up to par |
| sources | `E_i - published - historical` | sort of[^inc maps, books, but not comprehensive] | yes | but not up to par |
| sources | `E_i - published - historical not`[^eg archaeological, geographical, etc] | ? | no | - |
| sources | `E_i - published - official` | sort of[^eg UK command, parliamentary pps] | no | - |
| sources | `E_i - published not` | ? | yes | but possy not up to par[^eg no info on how this list built] |
| identities | natural persons | sort of[^eg Oxford DNB, RAH DBe] | no | - |
| identities | non natural persons[^eg institutions, depts, corporations, movements] | ? | no | - |
| gazetteer | points[^eg towns, buildings, etc] | sort of[^eg Antochiw atlas, Brown-Witschey Maya sites, place-name authorities] | a bit[^in 'Places'] | - |
| gazetteer | polygons[^eg town limits, extent or boundaries of states, etc] | sort of[^for modern states, post Versailles treaty states, etc] | no | - |
| metadata | all | sort of[^prefatory remarks on work] | a bit[^in 'Introduction'] | - |

where, if we were to follow [IFLA FRBR](https://www.ifla.org/references/best-practice-for-national-bibliographic-agencies-in-a-digital-age/resource-description-and-standards/bibliographic-control/functional-requirements-the-frbr-family-of-models/functional-requirements-for-bibliographic-records-frbr/)[^approved Sep 1997 most recently revised Feb 2009] -
1. for a collection of frbr:manifestations ie member of \\(E_i\\) but mostly a member of `E_i - published not` eg AGI GUATEMALA,
    1. `catalogue0` is a list of unique identifiers for each manifestation or item in the collection,
    2. `catalogue1` is a catalogue0 which further describes each manifestation or item eg by providing creation date, creator identity, and so on, but *does not* describe the contents of any manifestation or item,
    3. `catalogue2` is a catalogue1 which further describes the contents of each manifestation or item eg by summarising them, but *does not* transcribe the contents of any manifestation nor item,
    4. `catalogue3` is a catalogue1 or catalogue2 which further transcribes the contents of each manifestation or item,
    5. `calendar0` is a chronologically ordered union of subsets of one or more catalogues2, ie describes or summarises contents of select manifestations or items in a chronological manner, eg [CSPC](https://www.british-history.ac.uk/catalogue/guides-and-calendars),
    6. `calendar1` is a chronologically ordered union of subsets of one or more catalogues3, ie *transcribes* contents of select manifestations or items in a chronological manner, eg [Camden Miscellany](https://www.british-history.ac.uk/search/series/camden-misc) now [Camden Series](https://royalhistsoc.org/publications/camden-series/), aka `transcript`,
    7. `calendar` is calendar0 or calendar1.
2. for a member of \\(E_i\\),
    1. `catalogue0` is a list of unique identifiers for each manifestation or item selected, where we interpret 'author-date-title' and similar strings as unique identifiers, aka `bibliography` aka `catalogue`,
    2. `sources` is catalogue0.
3. for geographic or related spatiotemporal things,
    1. `gazetteer0` is a list of toponyms or place names with no  or very minimal description of their spatiotemporal applicability, eg toponyms placed on a map where we ignore other cartographic information,
    2. `gazetteer1` is gazetteer0 with further description of spatiotemporal applicability, eg dated maps where we take into account catographic information eg borders as demarcated on the map,
    3. `gazetteer` is gazetteer0 or gazetteer1.

## presentation [s 5]
### v 1.4 [s 5.1]
#### history of v 1.4<!--eg data collection, construction, inspo--> [s 5.1.1]
xx

Table listing events related to v 1.4 construction.[^perused records from `work/dec-22/free-text-nov-25.md` s 'output' subs 2 via `work/jun-23/out.md` s 2, but claims therein are outdated so was ignored. deposit records from `work/dec-22/pp.numbers` sheet 'log' = `work/dec-22/free-text-nov-25.md` s 'output' subs 5. all file paths within the table are for `pre-git-hist/` except in footnotes *and* except for `pp.numbers` in last col.]

| place | action | date | description | notes |
|:---:|:---|:---|:---|:---|
| bz-cy | created file | 01 Oct 2020 11:02 | re `files/tran/The Baymen's experiment.rtf` | earliest record in `events.tsv` |
| bz-cy | created file | 22 Oct 2020 05:04 | re `files/tran/civil list v1 *.tsv` | earliest *tsv* record in `events.tsv`[^re 2010s crown offices, programmes, budget per `work/dec-22/free-text-nov-25.md` s 'output' subs 3.] |
| bz-cy | created file | 11 Nov 2020 19:38 | re `files/red/gob rights practices *.tsv` | *possy* earliest events record in `events.tsv`[^but possy these events did not make it into v 1.4? file is re 2000s–2020s govt rights violations per `work/dec-22/free-text-nov-25.md` s 'output' subs 3.] |
| bz-cy | created file | 14 Nov 2020 20:53 | re `files/tran/debt belize 1 *.tsv` | *possy* earliest *stats* record in `events.tsv`[^but possy these stats did not make it into v 1.4? file is re 1980s–2020s sovereign debt, defaults, credit per `work/dec-22/free-text-nov-25.md` s 'output' subs 3.] |
| bz-cy | created file | 25 Nov 2020 15:25 | re `sheets/HURR BZ V1 *.numbers` | earliest record in `sheets.tsv` |
| bz-cy | created file | 25 Nov 2020 16:25 | re `files/red/HURR BZ V1 *.tsv` | *likely* earliest *events* et *stats* in `events.tsv`[^these events almost definitely made it into v 1.4. file is re 1760s–2010s storm events, vars stats per `work/dec-22/free-text-nov-25.md` s 'output' subs 3.] |
| xx | deposited file | 4 Nov 2021 ??:?? | re `files/harv/*.tsv` | eaarlist deposit in `pp.numbers`[^deposit uri = [dataverse.harvard.edu](https://dataverse.harvard.edu/privateurl.xhtml?token=135a1006-cd54-4d9e-ba7b-d961b93f1bc4), licensed CC0 1.0, *not* public as of 27 Nov 2022, but note `pp.numbers` lists 4 later deposits, inc *public* ones under distinct licences.] |

#### picture of v 1.4<!--notes on size, precision, accuracy, quality--> [s 5.1.2]
xx

### v 1.5 [s 5.2]
#### plan for v 1.5 [s 5.2.1]
xx

#### picture of v 1.5 [s 5.2.2]
xx

### comparison table [s 5.3]
xx

## conclusion [s 6]
xx

## supplement [s 7]
### v 1.4 [s 7.1]
xx

### codebook for v 1.4<!--update of intro file fm v 1.4 inc descriptions of variables and values--> [s 7.2]
xx

### log for v 1.4<!--log of changes between versions, revisions, or releases ie versioning and provenance--> [s 7.3]
First, see series-by-series log in `v-1.4/versioning/`.[^per `work/jun-23/out.md` s 2. this log uses `pre-git-hist/sheets/` to build a log. the procedure used is in `work/may-23/log1.md` s 'tasks' n 7.] Further, see file-by-file log in `work/may-23/out1.md`.[^in s 'list source files', location obtained via `wokr/jun-23/out.md` s 2.] For file-by-file contents description and provenance, see in `work/dec-22/free-text-nov-25.md`.[^in s 'output' subs 3, location obtained via `wokr/jun-23/out.md` s 2. this list is incomplete for the relevant files. other `work/` files might also have relevant information.]

