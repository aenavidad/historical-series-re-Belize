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

First, building on `pre-git-hist/files/oran/found data 1.2 Partitions 6-*.tsv`, for *work* as in frbr:work, we might partition \\(E\\) as follows.

```
level . partitions . notes
0 . evidence .
1 . evidence - work not . (i), (ii)
1 . evidence - work . (iii)

notes
(i) an earlier version of this level used the *is extant* before the *is work* relation. however, membership in the *evidence - extant not* collection would be known or deemed likely via some evidence in the *evidence - extant* bin, such that the *is extant* relations seems a bit unnecessary eg Classic Mayan codices
(ii) eg archaeological, palaeolithic, etc
(iii) inc textual and non-textual, published and otherwise, recorded and otherwise, etc
```

Partition of the `evidence - work` collection might proceed in a number of ways. The following are some examples, where *manifestation* is frbr:manifestation, and likewise for group 1 frbr entities.

```
eg . lvl . partitions . notes
0 . 2 . evidence - work - manifestation not . (i)
0 . 2 . evidence - work - manifestation .
0 . 3 . evidence - work - manifestation - published not . (ii)
0 . 3 . evidence - work - manifestation - published . 
1 . 3 . evidence - work - manifestation - textual not . (iii)
1 . 3 . evidence - work - manifestation - textual .

notes
(i) eg unrecorded oral history still being orally realised, etc
(ii) eg manuscripts, etc
(iii) ie *mostly* not textual eg maps, recordings, paintings
```

### table [s 4.2]
| type[^all of these are [ioa:information content entity](http://purl.obolibrary.org/obo/IAO_0000030), but also seem [frbr:work](https://www.ifla.org/references/best-practice-for-national-bibliographic-agencies-in-a-digital-age/resource-description-and-standards/bibliographic-control/functional-requirements-the-frbr-family-of-models/functional-requirements-for-bibliographic-records-frbr/) rather than frbr:expression or other entities.] | for | prev | v 1.4 | notes |
|:--|:--|:--|:--|:--|
| calendar | well used archives[^Belize ARS, UK TNA, Spain AGI] | sort of[^Burdon's *Archives*, UK Calendar, etc] | a bit[^in 'Cartas' series, some extracts in 'Events'] | - |
| calendar | poorly used archives[^Local parish ones, etc] | sort of[^some calendars exist, some catalogued, others not] | not in | - |
| chronicle | pre 17th cent | ? | a bit[^for 16th cent in 'Events'] | - |
| chronicle | post 16th cent | ? | yes | but possy not up to par[^eg has no coding info] |
| statistics | all | sort of[^disjoint series in literature] | yes | but not up to par |
| sources | print - non official - historical | sort of[^inc maps, books, but not comprehensive] | yes | but not up to par |
| sources | print - non official - non historical[^eg archaeological, geographical, etc] | ? | no | - |
| sources | print - official | sort of[^eg UK command, parliamentary pps] | no | - |
| sources | non print | ? | yes | but possy not up to par[^eg no info on how this list built] |
| identities | natural persons | sort of[^eg Oxford DNB, RAH DBe] | no | - |
| identities | non natural persons[^eg institutions, depts, corporations, movements] | ? | no | - |
| gazetteer | points[^eg towns, buildings, etc] | sort of[^eg Antochiw atlas, Brown-Witschey Maya sites, place-name authorities] | a bit[^in 'Places'] | - |
| gazetteer | polygons[^eg town limits, extent or boundaries of states, etc] | sort of[^for modern states, post Versailles treaty states, etc] | no | - |
| metadata | all | sort of[^prefatory remarks on work] | a bit[^in 'Introduction'] | - |

where, if we were to follow [IFLA FRBR](https://www.ifla.org/references/best-practice-for-national-bibliographic-agencies-in-a-digital-age/resource-description-and-standards/bibliographic-control/functional-requirements-the-frbr-family-of-models/functional-requirements-for-bibliographic-records-frbr/)[^approved Sep 1997 most recently revised Feb 2009] -
1. for a collection of frbr:manifestations eg AGI GUATEMALA,
    1. `catalogue0` is a list of unique identifiers for each manifestation in the collection,
    2. `catalogue1` is a catalogue0 which further describes each manifestation eg by providing creation date, creator identity, and so on, but *does not* describe the contents of any manifestation,
    3. `catalogue2` is a catalogue1 which further describes the contents of each manifestation eg by summarising them, but *does not* transcribe the contents of any manifestaiton,
    4. `catalogue3` is a catalogue1 or catalogue2 which further transcribes the contents of each manifestation,
    5. `calendar0` is a chronologically ordered union of subsets of one or more catalogues2, ie describes or summarises contents of select manifestations in a chronological manner, eg [CSPC](https://www.british-history.ac.uk/catalogue/guides-and-calendars)
    6. `calendar1` is a chronologically ordered union of subsets of one or more catalogues3, ie *transcribes* contents of select manifestations in a chronological manner, eg [Camden Miscellany](https://www.british-history.ac.uk/search/series/camden-misc) now [Camden Series](https://royalhistsoc.org/publications/camden-series/), aka `transcript`,
2. xx

## presentation [s 5]
### v 1.4 [s 5.1]
#### history of v 1.4 [s 5.1.1]
xx

#### picture of v 1.4 [s 5.1.2]
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
xx
