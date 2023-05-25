## abstract

lists output produced. created 23 may 2023 23.59 in belmopan.

## 24 may

### preprint sx

sx as per [[free-text-nov-25]] sec `log` no 6 and per [[may-23/log]] sec `24 may` no 2

```
sx
    abstract
    acknowledgements
    introduction
    context
    presentation
    conclusion
    supplement
    
where
    abstract = std sec
    acknowledgements = std sec
    introduction = std sec
    context =
        picture of bzean historiography eg accuracy as regards facts, biases or trends inc selectivity and scale, access or availability of primary sources, non interpretative secondary sources, their accuracy, and so on
    presentation =
        history of v 1.4 eg data collection, construction 
        picture of v 1.4 (notes on size, precision, accuracy, quality)
    conclusion = std sec
    supplement =
        v 1.4
        updated codebook (update of intro file fm v 1.4 inc descriptions of variables and values)
        log ie log of changers between versions, revisions, or releases ie versioning and provenance
```

### context subsx

subsx of context sec of preprint as per
- sec `preprint sx` above, 
- [[may-23/log]] sec `24 may` no 2 (SEP art on hist, WIK art of hist, Paul 2015, Bethell 1995),
- [[free-text-nov-25]] sec `output` subsec 6 `tsv 2 (literature)` (Higman 2003),[^copy of sheet in `pp.numbers`]
- [[iCloud: hist pp notes]] sec `notes` last bullet (Ashdown 1978a, Ashdown 1978b, Haug 1995, Higman 2003, Campbell 2009, Holden 2020).

| source[^where prim = primary source, nprim = not a primary source] | short | full | notes |
|:--|:--|:--|:--|
| nprim | coverage | how much of history is covered by sources eg spatially, temporally / how many prim sources are used for said coverage / what parts of either are omitted or selected | per SEP sec 1.2 |
| nprim | accuracy | as re factual data | x |
| nprim | objectivity | what are the biases, trends, interpretations observed | per SEP sec 3.2 |
| nprim | reliability | what stds of historical explanation are used / what stds of reasoning used historical claims or interpretations of human behaviour | per SEP sec 3.0 |
| nprim | reliability | what constitutes good historical explanation | per SEP sec 3.0-3.1 |
| prim | accuracy | is historical knowledge underdetermined by available evidence / how much of the past is retained in prim sources | per SEP sec 3.0 / Paul p 27 |
| nprim | synthesis | how are sm events knit together into lg events eg revolutions / any gluts or gaps in coverage of these lg events | per SEP sec 3.2, 3.4 |
| nprim | coverage | what are the fields of hist, and how well are these covered | WIK sec 1-2 |
| nprim | meta | how should nprim sources be judged / are they offering historical explanations, reasoning from empirical evidence, or building a narrative or survey | SEP sec 3.4[^cf Paul 2015 Key issues in historical theory] |
| nprim | meta | how should truth claims be judged, as opposed to nprim sources themselves / what stds of evidence and reasoning apply to truth claims in nprim sources | SEP sec 4.0 |
| nprim | moral | have morally troublesome events or parts of history not been covered in nprim sources eg slaving | SEP sec 6.0 |
| nprim | objectivity | what motivated the nprim's author's interest in the past, eg epistemic (*knowing that x*, *knowing why x*), moral (xx), political (*we did x*, nationalism, anticolonialism, ethnocentrism, political commitment, conservatism), aesthetic (narrative closure, narrative templates), or what motivated their writing | Paul p 30, 31-32, 34, 35, 56, 59, 71, 80-81 |
| nprim | meta | how will nprim sources be selected for scrutiny in preprint eg google scholar query, random selection of bibliography, all bibliography fm selected sources,[^may cf Bethell 1995, Higman 2003, Ashdown 1978a, Ashdown 1978b, Haug 1995, Cambell 2009, Holden 2020] all 21st cent sources cited for E series up to 1799 | x |

### supplement content

content as per [[v-log]] sec `records` subsec 1 `records 2`[^content for log portion of supplement ie provenance, metadata, revision, version log.][^filepaths in code block as per [[v-log]] sec `records` subsec 5 `files`]

```
for
- 0 = 0-action = 4 Nov 2021 - 4 Nov 2021 / harv/* / deposited in harv dataverse
- 1 = 1-action = 7 Oct 2021 - 3 Nov 2021 / red/rep bz fin pub 1.4 * / revised
- 2 = 2-action = 7 Sep 2021 - 6 Oct 2021 / red/rep bz fin pub 1.3_stable* / null

records for
- metadata saw 0 1 2
- sources saw 0 1
- A 0 - A 112 saw 0 1
- C 0 - C 992 saw 0 1
- E 0 - E 1076, odd E 1077 - E 2163 saw 0 1
- F 0 - F 170 saw 0 1
- L 0 - L 382 saw 0 1
- O 0 - O 37 saw 0 1
- T 0 - T 600, odd T 601 - T 781 saw 0 1
- W 0 - W 71, even W 72 - W 104 saw 0 1
```

#### supplement content M

content M for metadata, as per above, and newly created as per [[may-23/log]] sec `24 may` no 4[^id in code block = id in [[v-log]] sec `records` subsec 5 `files`, ver = is this file fit for versioning for this series (0 for file w no metadata nor metadata vars ie no dedicated space for metadata where short string metadata within data files not counted as metadata, 0 for file w no data overlap with ~~nearest ensuing ver 1~~ 00 file, 1 else), diff = list of records with diff fm nearest ensuing version w `/` separators, desc = nat lang desc of diff w `/` separators]

```
id,ver,diff,desc,note
00,1,null,null,null
01,1,none,none,null
02,1,none,none,null
03,0,null,null,null
04,0,null,null,null
05,0,null,null,null
06,1,all,additions,null,null
07,1,none,none,null
08,1,none,none,null
09,0,null,null,null
10,1,none,none,null
11,1,none,none,null
12,0,null,null,null
13,0,null,null,null
14,1,all,deletions,for * Errors-A1—14 *.tsv
15,0,null,null,null
16,1,xx,xx,for * Errors-A1—14 *.tsv
17,0,null,null,possy ver 1 for empty * Style-Table 1.tsv if it was meant as metadata space
18,0,null,null,null
19,1,xx,xx,for * Errors-A1–14 *.tsv
20,1,xx,xx,for * Errors-A1–14 *.tsv
21,0,null,null,null
22,0,null,null,null
23,0,null,null,null
24,0,null,null,null
25,0,null,null,null
26,0,null,null,null
27,0,null,null,null
28,0,null,null,null
29,0,null,null,null
30,0,null,null,null
31,0,null,null,null
32,0,null,null,null
33,0,null,null,null
34,0,null,null,null
35,0,null,null,null
36,0,null,null,null
37,0,null,null,null
38,0,null,null,where empty * Sheet 1-Table 1.tsv not taken as metadata space
39,0,null,null,null
40,0,null,null,null
41,1,xx,xx,for * Meta-Table 1.tsv where possy all diff
42,0,null,null,null
43,0,null,null,null
44,0,null,null,where empty * adsf-Table 1.tsv not taken as metadata space
45,0,null,null,null
46,1,xx,xx,possy all diff
47,0,null,null,null
48,0,null,null,null
49,0,null,null,null
50,0,null,null,null
```

#### supplement content S

content S for sources,[^understood as per [[v-log]] sec `records` subsec 4 `rules`] as per above, and newly created as per [[may-23/log]] sec `24 may` no 4[^id, diff, desc as for codeblock for metadata above, ver = is this file fit for versioning for this series (0 for file w no full citations nor dedicated space for them where short citations within data files not counted as full citations, 0 for file w no data overlap with 00 file, 1 else).]

```
id,ver,diff,desc,note
00,1,null,null,null
01,1,xx,xx,prolly revisions desc
02,1,xx,xx,null
03,0,null,null,null
04,0,null,null,null
05,0,null,null,null
06,1,xx,xx,prolly revisions desc
07,0,null,null,null
08,1,xx,xx,null
09,0,null,null,null
10,1,xx,xx,null
11,1,xx,xx,null
12,0,null,null,null
13,1,xx,xx,null
14,1,xx,xx,null
15,0,null,null,null
16,1,xx,xx,null
17,1,xx,xx,null
18,0,null,null,null
19,1,xx,xx,null
20,1,xx,xx,null
21,1,xx,xx,null
22,0,null,null,null
23,0,null,null,null
24,1,xx,xx,null
25,0,null,null,null
26,0,null,null,null
27,1,xx,xx,null
28,0,null,null,null
29,1,xx,xx,null
30,0,null,null,null
31,1,xx,xx,null
32,0,null,null,null
33,0,null,null,null
34,0,null,null,null
35,1,xx,xx,for * Index *.tsv
36,1,xx,xx,for * Index *.tsv
37,0,null,null,null
38,0,null,null,where empty * Sheet 1-Table 1.tsv not taken as sources space
39,1,xx,xx,for * Index *.tsv
40,0,null,null,null
41,0,null,null,null
42,0,null,null,null
43,0,null,null,null
44,1,xx,xx,null
45,0,null,null,null
46,0,null,null,null
47,0,null,null,null
48,0,null,null,null
49,0,null,null,null
50,0,null,null,null
```

#### supplement content M–W

content M, S, A, C, E, F, L, O, T, W for metadata (M), sources (S), and series A–W,[^statistics (precensal A), extracts (C), temporal (E), statistics (finances F), statistics (currency L), spatial (O), statistics (trade T), statistics (weather W), following [[v-log]] data categories] as per sec 2.3.0 above[^further cf data categories per [[v-log]] sec `records` subsec 4 `rules`, and note this subsec, unlike sec 2.3.1–2.3.2 above, does not include diff nor desc vars, restricting content to id, ver (labelled m–w), and note vars]

```
id,m,s,a,c,e,f,l,o,t,w,notes
00,1,1,1,1,1,1,1,1,1,1,null
01,1,1,1,1,1,1,1,1,1,1,null
02,1,1,1,1,1,1,1,0,1,1,null
03,0,1,0,0,0,0,0,0,0,0,updated s for cf*.tsv
04,0,0,0,0,1,0,0,0,0,0,null
05,0,0,0,0,0,0,0,0,0,0,null
06,1,1,1,0,1,1,1,0,1,0,null
07,1,0,0,0,1,0,0,0,0,0,null
08,1,1,1,1,1,1,1,1,1,1,null
09,0,0,0,0,1,0,0,0,0,0,null
10,1,1,1,0,1,1,1,0,1,0,null
11,1,1,1,0,1,1,1,0,1,0,null
12,0,0,1,0,1,0,0,0,0,0,null
13,0,1,0,0,0,0,0,0,0,0,null
14,1,1,0,0,0,0,0,0,0,0,null
15,0,0,1,0,1,0,1,0,0,0,null
16,1,1,0,0,0,0,0,0,0,0,null
17,0,1,0,0,1,0,0,0,0,0,null
18,0,0,0,0,1,0,0,0,0,0,null
19,1,1,1,0,1,0,1,0,0,0,null
20,1,1,1,0,1,0,1,0,0,0,null
21,0,1,0,0,0,0,0,0,0,0,null
22,0,0,0,0,1,0,0,0,0,0,null
23,0,0,0,0,1,0,0,0,0,0,null
24,0,1,0,0,1,0,0,0,0,0,null
25,0,0,0,0,1,0,0,0,0,0,null
26,0,0,0,0,1,0,0,0,0,0,null
27,0,1,0,0,0,0,0,0,0,0,null
28,0,0,0,0,1,0,0,0,0,0,null
29,0,1,0,0,1,0,0,0,0,0,null
30,0,0,0,0,1,0,0,0,0,0,null
31,0,1,0,0,1,0,0,0,0,0,null
32,0,0,0,0,0,1,1,0,1,0,null
33,0,0,0,0,1,0,0,0,0,0,null
34,0,0,0,0,0,1,1,0,1,0,null
35,0,1,0,0,0,1,1,0,1,0,null
36,0,1,0,0,0,1,1,0,1,0,null
37,0,0,0,0,0,1,1,0,1,0,null
38,0,0,0,0,0,0,0,0,0,0,null
39,0,1,0,0,0,1,1,0,1,0,null
40,0,0,0,0,0,0,0,0,1,0,null
41,1,0,1,0,1,0,0,0,1,0,null
42,0,0,0,0,0,0,0,0,1,0,null
43,0,0,0,0,0,0,0,0,1,0,null
44,0,1,0,0,1,0,0,0,0,0,null
45,0,0,0,0,1,0,0,0,0,0,null
46,1,0,1,0,1,0,1,0,1,0,null
47,0,0,1,0,1,1,1,0,1,0,null
48,0,0,1,0,1,1,0,0,1,0,null
49,0,0,0,0,0,0,0,0,0,0,null
50,0,0,1,0,1,1,1,0,1,1,null
```

## 25 may

### supplement content

continues output fm s 2.3 above

#### list source files

list of all files to be used in producing record-by-record versioning, as per [[may-23/log]] s xx no 1[^xx]

```
00-cartas-series-c-0—992---data-on-buccaneering-or-piratical-activity-in-the-bay-of-honduras-from-spanish-correspondence.-19.06.10.tsv
00-currency-series-l-0—382---currency-and-exchange.-19.06.11.tsv
00-estimates-series-a-0—112---pre-censal-or-pre-statistical-estimates-of-population,-trade,-public-finances,-and-related-matters..tsv
00-events-2-series-e-1—2163---events-certainly-not-involving-loss-of-life,-limb-or-property..tsv
00-events-series-e-0—1076---events-possibly-or-definitely-involving-loss-of-life,-limb-or-property..tsv
00-finances-series-f-0—170---public-finances.-19.06.10.tsv
00-introduction-loss-of-life-or-property-in-belize-from-1630-to-present..tsv
00-sources-2-series-s-1—583---primary-sources-which-are-deposited-series-or-collections..tsv
00-sources-series-s-0—1628---primary-and-secondary-sources-which-are-not-deposited-series-or-collections..tsv
00-towns-series-o-0–37---settlements-present-or-established-post-columbus..tsv
00-trade-2-series-t-1—781---foreign-markets..tsv
00-trade-series-t-0—600---foreign-trade..tsv
00-weather-2-series-w-1—7167---sub-annually-resolved-meteorological-data.tsv
00-weather-series-w-0—1042---annually-resolved-meteorological-data..tsv
01-asdfasfasdfasfasfasdfasdfsaf.tsv
01-cartas-series-c-0—992---data-on-buccaneering-or-piratical-activity-in-the-bay-of-honduras-from-spanish-correspondence..tsv
01-copy-introduction-loss-of-life-or-property-in-belize-from-1630-to-present.-copy.tsv
01-currency-series-l-0—382---currency-and-exchange..tsv
01-estimates-series-a-0—112---pre-censal-or-pre-statistical-estimates-of-population,-trade,-public-finances,-and-related-matters..tsv
01-events-2-series-e-1—2163---events-certainly-not-involving-loss-of-life,-limb-or-property..tsv
01-events-series-e-0—1076---events-possibly-or-definitely-involving-loss-of-life,-limb-or-property..tsv
01-finances-series-f-0—170---public-finances..tsv
01-introduction-loss-of-life-or-property-in-belize-from-1630-to-present..tsv
01-sources-2-series-s-1—583---primary-sources-which-are-deposited-series-or-collections..tsv
01-sources-series-s-0—1628---primary-and-secondary-sources-which-are-not-deposited-series-or-collections..tsv
01-towns-series-o-0–37---settlements-present-or-established-post-columbus..tsv
01-trade-2-series-t-1—781---foreign-markets..tsv
01-trade-series-t-0—600---foreign-trade..tsv
01-weather-2-series-w-1—7167---sub-annually-resolved-meteorological-data.tsv
01-weather-series-w-0—1042---annually-resolved-meteorological-data..tsv
02.tsv
03--cf-table-1.tsv
03--contact-table-1.tsv
03-all-table-1.tsv
04-all-table-1.tsv
04-dept-table-1.tsv
04-gg-table-1.tsv
04-jud-table-1.tsv
04-local-table-1.tsv
04-min-table-1.tsv
04-parl-table-1.tsv
04-quas-table-1.tsv
05-2019-table-1.tsv
06-a-estimates-series-a-0—93---pre-censal-or-pre-statistical-estimates-of-population,-trade,-public-finances,-or-related-matters..tsv
06-clusters-table-1.tsv
06-e-events-0-series-e-0—548---events..tsv
06-e-events-1-series-e-0—548---events..tsv
06-f-finances-series-f-0—170---public-finances..tsv
06-introduction-loss-of-life-or-property-in-belize-from-1630-to-present..tsv
06-l-currency-series-l-0—382---currency-and-exchange..tsv
06-s-sources-0-series-s-0—435---primary-and-secondary-sources..tsv
06-s-sources-1-series-s-0—435---primary-and-secondary-sources..tsv
06-t-trade-series-t-0—300---trade..tsv
07-clusters-table-1.tsv
07-introduction-loss-of-life-or-property-in-belize-from-1630-to-present..tsv
08-cartas-series-c-0—992---data-on-buccaneering-or-piratical-activity-in-the-bay-of-honduras-from-spanish-correspondence..tsv
08-currency-series-l-0—382---currency-and-exchange..tsv
08-estimates-series-a-0—107---pre-censal-or-pre-statistical-estimates-of-population,-trade,-public-finances,-and-related-matters..tsv
08-events-2-series-e-0—1767---events-certainly-not-involving-loss-of-life,-limb-or-property..tsv
08-events-series-e-0—988---events-possibly-or-definitely-involving-loss-of-life,-limb-or-property..tsv
08-finances-series-f-0—170---public-finances..tsv
08-introduction-loss-of-life-or-property-in-belize-from-1630-to-present..tsv
08-sources-2-series-s-0—421---primary-sources-which-are-deposited-series-or-collections..tsv
08-sources-series-s-0—960---primary-and-secondary-sources-which-are-not-deposited-series-or-collections..tsv
08-towns-series-o-xxx---settlements-present-or-established-post-columbus..tsv
08-trade-2-series-t-1—xxx---foreign-markets..tsv
08-trade-series-t-0—600---foreign-trade..tsv
08-weather-2-series-w-1—7167---sub-annually-resolved-meteorological-data.tsv
08-weather-series-w-0—1042---annually-resolved-meteorological-data..tsv
09-government-table-1.tsv
09-history-table-1.tsv
09-sheet-1-table-1.tsv
10-2-a-estimates---series-a-0—93-_-p-table-1.tsv
10-2-clusters-table-1.tsv
10-2-e-events---series-e-0—548-_-eve-table-1.tsv
10-2-export-summary-table-1.tsv
10-2-f-finances---series-f-0—170-_-p-table-1.tsv
10-2-introduction---loss-of-life-or--table-1.tsv
10-2-l-currency---series-l-0—382-_-c-table-1.tsv
10-2-s-sources---series-s-0—435-_-pr-table-1.tsv
10-2-sheet-1-1-1-1-1-1-1-1-1-table-1.tsv
10-2-t-trade---series-t-0—300-_-trad-table-1.tsv
11-a-estimates-series-a-0—93---pre-censal-or-pre-statistical-estimates-of-population,-trade,-public-finances,-or-related-matters..tsv
11-clusters-table-1.tsv
11-e-events-series-e-0—548---events..tsv
11-f-finances-series-f-0—170---public-finances..tsv
11-introduction-loss-of-life-or-property-in-belize-from-1630-to-present..tsv
11-l-currency-series-l-0—382---currency-and-exchange..tsv
11-s-sources-series-s-0—435---primary-and-secondary-sources..tsv
11-t-trade-series-t-0—300---trade..tsv
12-clusters-c-1—47---event-clusters..tsv
12-events-<-1800-e-1—320---events..tsv
12-events-<-pres-e-1—320---events..tsv
12-loans-l-1—3---pre-statistical-estimates-of-sovereign-loans..tsv
12-p-estimates-p-1—50---pre-censal-estimates-of-population-or-of-proxies-for-population..tsv
12-redwoods-r-1—8---new-world-redwoods..tsv
12-t-estimates-t-1—15---pre-statistical-estimates-of-trade,-wealth,-and-the-like..tsv
13-primary-ms-c1—30---online-collections-of-archival-material..tsv
13-primary-p-c1—30---online-collections-of-archival-material..tsv
13-secondary-peer-c1—30---online-collections-of-archival-material..tsv
13-secondary-print-c1—30---online-collections-of-archival-material..tsv
14-availble-b1—25---catalogues-and-repositories-of-archival-material..tsv
14-collections-c1—30---online-collections-of-archival-material..tsv
14-errors-a1—14---false-positives-or-false-negatives-in-archival-material..tsv
14-hidden-b1—25---catalogues-and-repositories-of-archival-material..tsv
14-local-c1—30---online-collections-of-archival-material..tsv
14-peer-c1—30---online-collections-of-archival-material..tsv
14-primary-c1—30---online-collections-of-archival-material..tsv
14-print-c1—30---online-collections-of-archival-material..tsv
15-clusters-c-1—47---event-clusters..tsv
15-events-e-1—320---events..tsv
15-loans-l-1—3---pre-statistical-estimates-of-sovereign-loans..tsv
15-p-estimates-p-1—50---pre-censal-estimates-of-population-or-of-proxies-for-population..tsv
15-places-r-1—8---new-world-redwoods..tsv
15-population-g1—383---population..tsv
15-redwoods-r-1—8---new-world-redwoods..tsv
15-t-estimates-t-1—15---pre-statistical-estimates-of-trade,-wealth,-and-the-like..tsv
15-treasury-rate-h1—383---treasury-rate..tsv
16-availble-b1—25---catalogues-and-repositories-of-archival-material..tsv
16-collections-c1—30---online-collections-of-archival-material..tsv
16-errors-a1—14---false-positives-or-false-negatives-in-archival-material..tsv
16-hidden-b1—25---catalogues-and-repositories-of-archival-material..tsv
16-peer-c1—30---online-collections-of-archival-material..tsv
16-press-c1—30---online-collections-of-archival-material..tsv
16-print-c1—30---online-collections-of-archival-material..tsv
17-events-table-1.tsv
17-peer-table-1.tsv
17-print-table-1.tsv
17-style-table-1.tsv
18-disastrous-table-1.tsv
18-not-disastrous-table-1.tsv
19-collections-c1—30---online-collections-of-archival-material..tsv
19-disasters-e1—48---disasters..tsv
19-errors-a1—14---false-positives-or-false-negatives-in-archival-material..tsv
19-estimates-d1—29---pre-censal-estimates-of-population-or-of-proxies-for-population..tsv
19-events-f1—170---events..tsv
19-non-press-sources-c1—30---online-collections-of-archival-material..tsv
19-population-g1—383---population..tsv
19-press-sources-c1—30---online-collections-of-archival-material..tsv
19-repositories-b1—25---catalogues-and-repositories-of-archival-material..tsv
19-timeline-g1—383---population..tsv
19-treasury-rate-h1—383---treasury-rate..tsv
20-disasters-1-e1—48---disasters..tsv
20-disasters-e1—48---disasters..tsv
20-disastrous-even-e---disastrous-events..tsv
20-estimates-d1—29---pre-censal-estimates-of-population-or-of-proxies-for-population..tsv
20-non-disastrous-odd-e---non-disastrous-events..tsv
20-population-g1—383---population..tsv
20-treasury-rate-h1—383---treasury-rate..tsv
21-sheet-1-table-1.tsv
22.tsv
23-<-1820-table-1.tsv
23-<-pres-table-1.tsv
23-clustering-table-1.tsv
23-loss-£-est-table-1.tsv
23-loss-£-table-1.tsv
23-loss-text-table-1.tsv
24-<-1820-table-1.tsv
24->-1820-table-1.tsv
24-boston-table-1.tsv
24-burney-table-1.tsv
24-european-table-1.tsv
24-nyc-table-1.tsv
24-press-<-1820-table-1.tsv
24-spanish-table-1.tsv
25-<-1700-table-1.tsv
25-<-1820-table-1.tsv
25-<-pres-table-1.tsv
25-clustering-table-1.tsv
26-sheet-1-2-table-1.tsv
26-sheet-1-table-1.tsv
27-press-table-1.tsv
27-print-table-1.tsv
27-state-table-1.tsv
28-sheet-1-table-1.tsv
29-<-1820-table-1.tsv
29->-1820-table-1.tsv
29-boston-table-1.tsv
29-burney-table-1.tsv
29-european-table-1.tsv
29-nyc-table-1.tsv
29-press-<-1820-table-1.tsv
29-spanish-table-1.tsv
30-calendar-table-1.tsv
30-hostilities-table-1.tsv
30-other-table-1.tsv
30-wars-table-1.tsv
31-<-1820-table-1.tsv
31->-1820-table-1.tsv
31-boston-table-1.tsv
31-burney-table-1.tsv
31-european-table-1.tsv
31-nyc-table-1.tsv
31-press-<-1820-table-1.tsv
31-spanish-table-1.tsv
32-activities-table-1.tsv
32-financials-hon-table-1.tsv
32-financials-table-1.tsv
32-fx-table-1.tsv
32-gdp-hon-table-1.tsv
32-log-f-all-table-1.tsv
32-t---f-hon-table-1.tsv
32-t-eng-table-1.tsv
32-t-gb-table-1.tsv
32-t-scot-table-1.tsv
33-<-1820-table-1.tsv
33->-1820-table-1.tsv
34-financials-table-1.tsv
34-fx-table-1.tsv
34-log-f-all-table-1.tsv
34-t---f-hon-table-1.tsv
34-t-eng-table-1.tsv
34-t-gb-table-1.tsv
34-t-scot-table-1.tsv
35-abstracts-table-1.tsv
35-cust-14-table-1.tsv
35-cust-17-table-1.tsv
35-cust-3-table-1.tsv
35-cust-4-table-1.tsv
35-index-of-abstracts-table-1.tsv
35-index-of-reports-table-1.tsv
35-reports-table-1.tsv
36-abstracts-table-1.tsv
36-cust-14-table-1.tsv
36-cust-17-table-1.tsv
36-cust-3-table-1.tsv
36-cust-4-table-1.tsv
36-index-of-abstracts-table-1.tsv
36-index-of-reports-table-1.tsv
36-reports-table-1.tsv
37-financials-hon-table-1.tsv
37-financials-table-1.tsv
37-fx-table-1.tsv
37-gdp-hon-table-1.tsv
37-log-f-all-table-1.tsv
37-t---f-hon-table-1.tsv
37-t-eng-table-1.tsv
37-t-gb-table-1.tsv
37-t-scot-table-1.tsv
38-sheet-1-table-1.tsv
39-abstracts-table-1.tsv
39-cust-14-table-1.tsv
39-cust-17-table-1.tsv
39-cust-3-table-1.tsv
39-cust-4-table-1.tsv
39-index-of-abstracts-table-1.tsv
39-index-of-reports-table-1.tsv
39-reports-table-1.tsv
40-all-to-england-&-wales-table-1.tsv
40-log-to-colonies-table-1.tsv
40-log-to-england-&-wales-table-1.tsv
41-<-1790-table-1.tsv
41->-1790-table-1.tsv
41-exports-table-1.tsv
41-meta-table-1.tsv
41-sum-table-1.tsv
42-forms-conversion-table-1.tsv
42-forms-cust-16-table-1.tsv
42-forms-cust-17-1-table-1.tsv
42-forms-cust-17-table-1.tsv
42-forms-cust-3->-62-table-1.tsv
42-forms-cust-3->-65-table-1.tsv
42-forms-cust-3-table-1.tsv
42-forms-cust-boston-table-1.tsv
42-forms-cust-jam-table-1.tsv
42-forms-cust-jamaica-1-table-1.tsv
42-forms-cust-jamaica-table-1.tsv
42-forms-mahogany-thesis-table-1.tsv
42-forms-text-table-1.tsv
42-forms-tonnes-table-1.tsv
42-raw-cust-16-2-table-1.tsv
42-raw-cust-16-table-1.tsv
42-raw-cust-17-table-1.tsv
42-raw-cust-3->-62-table-1.tsv
42-raw-cust-3->-65-table-1.tsv
42-raw-cust-3-table-1.tsv
42-raw-cust-boston-table-1.tsv
42-raw-cust-co-table-1.tsv
42-raw-cust-jam-table-1.tsv
42-raw-cust-jamaica-table-1.tsv
42-raw-cust-span---hon-table-1.tsv
42-raw-mahogany-thesis-table-1.tsv
42-raw-text-table-1.tsv
42-raw-tonnes-table-1.tsv
43-sheet-1-table-1.tsv
44-adsf-table-1.tsv
44-d-citations-table-1.tsv
44-d-deaths-table-1.tsv
44-d-sources-table-1.tsv
45-sheet-1-table-1.tsv
46-cpi-table-1.tsv
46-disasters-table-1.tsv
46-formulas-table-1.tsv
46-fx-table-1.tsv
46-metadata-table-1.tsv
46-population-table-1.tsv
46-storm-damages-table-1.tsv
46-storm-deaths-table-1.tsv
46-storm-history-table-1.tsv
46-storms-table-1.tsv
46-trade-+-gdp-2020-table-1.tsv
46-trade-+-gdp-table-1.tsv
47-gazette---reports-table-1.tsv
47-original-table-1.tsv
47-sheet-1-table-1.tsv
47-simulated-table-1.tsv
47-un-table-1.tsv
48-sheet-1-table-1.tsv
49-govt-table-1.tsv
49-military-table-1.tsv
50---blue-1-1-table-1.tsv
50---blue-table-1.tsv
50---gdp-pop-table-1.tsv
50---gfm-table-1.tsv
50---graph-table-1.tsv
50---historical-table-1.tsv
50---loss-table-1.tsv
50---naval-table-1.tsv
50---nms-table-1.tsv
50---rainfall-table-1.tsv
50---simulated-storms-w-in-150-nautical-miles-of-belize..tsv
50---storms-1-storms-w-in-150-nautical-miles-of-belize..tsv
50---storms-2-storms-w-in-150-nautical-miles-of-belize..tsv
50---storms-<-4-storms-w-in-0-nautical-miles-of-belize..tsv
50---storms-storms-w-in-150-nautical-miles-of-belize..tsv
```