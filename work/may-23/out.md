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
11,1,1,0,0,0,0,0,0,0,0,null
12,0,0,0,0,0,0,0,0,0,0,null
13,0,1,0,0,0,0,0,0,0,0,null
14,1,1,0,0,0,0,0,0,0,0,null
15,0,0,0,0,0,0,0,0,0,0,null
16,1,1,0,0,0,0,0,0,0,0,null
17,0,1,0,0,0,0,0,0,0,0,null
18,0,0,0,0,0,0,0,0,0,0,null
19,1,1,0,0,0,0,0,0,0,0,null
20,1,1,0,0,0,0,0,0,0,0,null
21,0,1,0,0,0,0,0,0,0,0,null
22,0,0,0,0,0,0,0,0,0,0,null
23,0,0,0,0,0,0,0,0,0,0,null
24,0,1,0,0,0,0,0,0,0,0,null
25,0,0,0,0,0,0,0,0,0,0,null
26,0,0,0,0,0,0,0,0,0,0,null
27,0,1,0,0,0,0,0,0,0,0,null
28,0,0,0,0,0,0,0,0,0,0,null
29,0,1,0,0,0,0,0,0,0,0,null
30,0,0,0,0,0,0,0,0,0,0,null
31,0,1,0,0,0,0,0,0,0,0,null
32,0,0,0,0,0,0,0,0,0,0,null
33,0,0,0,0,0,0,0,0,0,0,null
34,0,0,0,0,0,0,0,0,0,0,null
35,0,1,0,0,0,0,0,0,0,0,null
36,0,1,0,0,0,0,0,0,0,0,null
37,0,0,0,0,0,0,0,0,0,0,null
38,0,0,0,0,0,0,0,0,0,0,null
39,0,1,0,0,0,0,0,0,0,0,null
40,0,0,0,0,0,0,0,0,0,0,null
41,1,0,0,0,0,0,0,0,0,0,null
42,0,0,0,0,0,0,0,0,0,0,null
43,0,0,0,0,0,0,0,0,0,0,null
44,0,1,0,0,0,0,0,0,0,0,null
45,0,0,0,0,0,0,0,0,0,0,null
46,1,0,0,0,0,0,0,0,0,0,null
47,0,0,0,0,0,0,0,0,0,0,null
48,0,0,0,0,0,0,0,0,0,0,null
49,0,0,0,0,0,0,0,0,0,0,null
50,0,0,0,0,0,0,0,0,0,0,null
```