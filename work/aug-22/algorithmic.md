# algorithmic

## abstract

this file has the following contents[^1]
1. a list of steps to be followed to produce v-1.5 from v-1.4 data (or from v-1.4 and pre-git-hist data),
2. a list of work-procedural standards which steps in section 1 must or may meet,
3. a list of file outputs expecting from following steps in section 1,
4. a list of work-output standards which file outputs in section 3 must or may meet.

## sec 1. work flow towards v-1.5

start

1. query `v-1.4` and `pre-git-hist/files`, tagging files either as files to be mined during this work flow or not,
2. collect all files tagged file-to-be-mined,
3. extract raw data,
4. cs-clean these raw data,[^3]
5. hist-clean these cs-cleaned raw data,[^3]
6. preserve authoritative-copy of cleaned = hist-cleaned + cs-cleaned raw data, making vars working-copies of them,
7. extract vertices from working-copy of cleaned raw data while also building metadata for these vertices,
8. output vertices data and their associated metadata and validate these,
9. repeat steps 5-6 for edges,
10. repeat steps 5-6 for d-function,
11. verify compliance of steps 1-8 with all `sec. 2` standards,
12. verify compliance of `sec 3` files with `sec 4` standards.

end

## sec 2. work flow standards for sec. 1

### sec 2.1. standards for work-flow ie actions ie events

work-flow ie processes ie actions ie events in `sec 1` to must or may (as indicated) meet the following standards.

1. must be recorded ie version-controlled via git per BW,[^5]
2. must not endanger authoritative copy of cleaned raw data per BW,

### sec. 2.2. standards for intermediate files eg clean raw data

files output from `sec 1` which are not also `sec 3` files eg cs-clean raw data files must or may (as indicated) meet the following standards.

1. must be only UTF-8 encoded ie inc no markup nor formatting per BW per TCD,
2. may be stored as `csv` per TCL, BW,
3. must, if an authoritative or orginal copy eg clean raw data, be deposited in at least one repository per TCL per BW,[^6]
4. must, if an authoritative or original copy, be verifiably clean ie have passed cs-clean and hist-clean validation tests per BW,[^3]
5. must, if an authoritative or original copy, by human- and machine-readable per TCD,

## sec 3. work output from sec. 1

we expect at least the followwing files upon following sec. 1 steps.[^2]

1. one `vertices.csv` for vertices of G = (V,E,d),
2. one `edges.csv` for edges of G,
3. one `d-function.csv` for function d of G,
4. three `*.csv-metadata.json` for each `csv` file in items 1-3. 

## sec 4. work output standards for sec. 3

`sec. 3` files must or may (as indicated) meet the following standards, in addition to standards 1-[null] of `sec 2.2` (where all `sec 3` files count as "authoritative or orignal copies")

1. must use at least one controlled vocabulary ie ontology per TCL,[^4]
2. must provide at least minimal metadata per TCL,
3. must provide at least minimal explanation of missing values within metadata per BW per TCD,[^8]
4. must provide at least minimal data dictionary within metadata per BW,[^9]
5. must use at least one URI ie IRI per TCL,
6. must be translatable ie convertible to `rdf` format per TCL,[^7]
7. xxx

## authorities

- [W3C](https://www.w3.org/TR/?tag=data&version=latest),
- [TCL](https://librarycarpentry.org/Top-10-FAIR/2018/12/01/historical-research/),
- [TCD](https://datacarpentry.org/spreadsheet-ecology-lesson/02-common-mistakes/),
- [BW](https://doi.org/10.1080/00031305.2017.1375989),
- [MD](https://doi.org/10.3200/HMTS.37.1.34-38), //needs review as of 14 aug 2022
- [HK](https://doi-org.ezp-prod1.hul.harvard.edu/10.1080/01615440.2018.1484676).//needs review as of 14 aug 2022

## references

- xxx

[^1]: file created 14 aug 2022 in boston MA.

[^2]: per `output.md`, the structure we are meant to have is a graph construed as follows (variously called a quiver ie directed pseudograph ie directed graph ie digraph ie directed multigraph eg [per wolfram](https://mathworld.wolfram.com/Pseudograph.html) and eg [per ncatlab](https://ncatlab.org/nlab/show/pseudograph).

      - take the usual mathematical primitives eg points, sets.
      - let naturals N = {0,1,2,...},
      - let a binary relation ~ on set A and set B be set R = ~ a subset of A * B ie of the cartesian product of A and B where we allow A = B,
      - let a partial unary function f from A to B ie a unary function f from A to B be a binary relation ~ on A and B where for any a in A if a ~ b_i and a ~ b_j then b_i = b_j ie if f(a) = b_i and f(a) = b_j then b_i = b_j,
      - let a total unary function f from A to B be a unary function g from A to B where for any a in A there is at least one b in B such that f(a) = g(a) = b,
      - let vertices V = {0,1,2,...,n) for natural n > 0, 
      - let edges E = {0,1,2,...,m) for natural m > 0,
      - let total unary function d: E to P(V * V) for power set P(V * V) of V * V take each edge e to the subset of V * V of exactly those vertices (v_i,v_j) where e starts at v_i and ends at v_j (again, allowing v_i = v_j),
      - let graph G = (V,E,d).

[^3]: where*cs-clean*raw data meet certain syntax, encoding, etc technical standards as given by [null] for `csv` and [null] for `md`, while*hist-clean*raw data meet certain scholarly or data quality standards as given by [null], while validation-tests for these properties check that data meet said cs-clean or hist-clean standards eg
      - ie for `csv` files ensure these meet technical `csv` specifications per [null], and further meet scholarly `csv` specifications per [null] eg use string "yyyy-mm-dd" for date-values per BW, and trim string values ie purge leading and trailing space characters eg " one " -> "one" per BW, and "avoid" [ie purge?] or do not use any special characters other than "-" and "_" per BW and TCD, and leave no empty cells per BW, and store exactly one piece of data per cell per BW and TCD, and store only one table within a file per BW per TCD, and process data with [OpenRefine](https://datacarpentry.org/OpenRefine-ecology-lesson/) per TCD, and build variable names with only letters, numerals, and underscores ie sans spaces and sans special characters other than underscores per TCD,
      - ie for `json` [null],
      - ie for `md` [null].

[^4]: the most useful of which seem to be the following.

      - those built or used in programming language specifications, eg for [TEI](https://tei-c.org/release/doc/tei-p5-doc/en/html/index.html), RDF, XML, JSON, JSON-LD, CSV, OWL,
      - upper level ontologies eg [BFO](http://xmlns.com/foaf/spec/) or [schema.org](https://schema.org) or [wikidata](https://www.wikidata.org/wiki/Wikidata:Main_Page) or commonest ones as per the [LOV directory](https://lov.linkeddata.es/dataset/lov/),
      - vars lower level ontologies or vocabs eg those
             + for authorities ie authors etc eg [LCNAF](http://id.loc.gov/authorities/names.html), [VIAF](https://viaf.org/), ISNI,
             + for human networks ie human-human edges etc eg [FOAF](http://xmlns.com/foaf/spec/),
             + ISO-related ones eg [ISO 639](https://www.loc.gov/standards/iso639-2/php/code_list.php) for languages, [null] for dates, [null] for [null],
             + geographic eg [Getty TGN](http://www.getty.edu/research/tools/vocabularies/tgn/index.html), [GeoNames](https://www.geonames.org),
             + bibliographic-cataloguing eg [LCSH](http://id.loc.gov/authorities/subjects.html) or its derivative [FAST](https://www.oclc.org/research/areas/data-science/fast.html), [UNESCO](http://vocabularies.unesco.org/thesaurus), [ICPSR](https://www.icpsr.umich.edu/icpsrweb/ICPSR/thesaurus/index), [CIDOC CRM](https://cidoc-crm.org),
             + for metadata eg [Dublin Core](https://www.dublincore.org), [IOA](https://ontobee.org/ontology/IAO), [DDI](http://www.ddialliance.org/controlled-vocabularies), [SKOS](http://www.w3.org/2004/02/skos/core),
             + for licensing eg [CC](https://lov.linkeddata.es/dataset/lov/vocabs/cc).

[^5]: eg following [Robertson best practices](http://sethrobertson.github.io/GitBestPractices/).

[^6]: eg raw data files deposited in [CoreTrustSeal-certified repositories](https://www.coretrustseal.org/why-certification/certified-repositories/) eg [DANS](https://easy.dans.knaw.nl/ui/home) eg [Zenodo](https://zenodo.org).

[^7]: esp by machines eg [OpenRefine](https://openrefine.org).

[^8]: BW suggest string "NA" for missing data, and not blank cells nor number -999 nor number 999 for missing data. TCD suggest a blank cell, "NA", "na", or "NULL" and not -999 nor 999.

[^9]: where per BW minimal data dictionary explains all variables used eg lists exact variable name as used in data files, give any alternative variable names used elsewhere, an explanation [definition? elucidation?] of the variable, measurement units of the variable, min and max values of the variable values.