# algorithmic

- [algorithmic](#algorithmic)
  - [abstract](#abstract)
  - [sec 1. work flow towards v-1.5](#sec-1-work-flow-towards-v-15)
  - [sec 2. work flow standards for sec. 1](#sec-2-work-flow-standards-for-sec-1)
    - [sec 2.1. standards for work-flow ie actions ie events](#sec-21-standards-for-work-flow-ie-actions-ie-events)
    - [sec. 2.2. standards for intermediate files eg clean raw data](#sec-22-standards-for-intermediate-files-eg-clean-raw-data)
  - [sec 3. work output from sec. 1](#sec-3-work-output-from-sec-1)
  - [sec 4. work output standards for sec. 3](#sec-4-work-output-standards-for-sec-3)
  - [authorities](#authorities)
  - [references](#references)
  - [footnotes](#footnotes)

## abstract

this file has the following contents.[^1]
1. a list of steps to be followed to produce v-1.5 from v-1.4 data (or from v-1.4 and pre-git-hist data),
2. a list of work-procedural standards which steps in section 1 must or may meet,
3. a list of file outputs expecting from following steps in section 1,
4. a list of work-output standards which file outputs in section 3 must or may meet.

## sec 1. work flow towards v-1.5

start[^12]

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

1. must be recorded ie version-controlled via git per BW per HK per MD,[^5]
2. must not endanger authoritative copy of cleaned raw data per BW,

### sec. 2.2. standards for intermediate files eg clean raw data

files output from `sec 1` which are not also `sec 3` files eg cs-clean raw data files must or may (as indicated) meet the following standards.

1. must be only UTF-8 encoded ie inc no markup nor formatting per BW per TCD per W3C in tabular-data-model,
2. may be stored as `csv` per TCL per BW per W3C in tabular-data-primer,
3. must, if an authoritative or orginal copy eg clean raw data, be deposited in at least one repository per TCL per BW per W3C in dwbp,[^6]
4. must, if an authoritative or original copy, be verifiably clean ie have passed cs-clean and hist-clean validation tests per BW per W3C in tabular-data-primer,[^3]
5. must, if an authoritative or original copy, by human- and machine-readable per TCD per W3C in dwbp,

## sec 3. work output from sec. 1

we expect at least the followwing files upon following sec. 1 steps.[^2]

1. one `vertices.csv` for vertices of G = (V,E,d),
2. one `edges.csv` for edges of G,
3. one `d-function.csv` for function d of G,
4. three `*.csv-metadata.json` for each `csv` file in items 1-3. 

## sec 4. work output standards for sec. 3

`sec. 3` files must or may (as indicated) meet the following standards, in addition to standards 1-[null] of `sec 2.2` (where all `sec 3` files count as "authoritative or orignal copies")

1. must use at least one controlled vocabulary ie ontology per TCL per W3C in dwbp per W3C in ld-bp per W3C in ldp-bp,[^4]
2. must provide at least minimal metadata per TCL per W3C in dwbp per W3C in tabular-data-primer per FD in table-schema per FD in tabular-data-resource per FD in tabular-data-package,
3. must provide at least minimal explanation of missing values within metadata per BW per TCD per W3C in dwbp per FD in table-schema per MD,[^8]
4. must provide at least minimal data dictionary within metadata per BW,[^9]
5. must provide at least minimal data provenance and quality information within metadata per W3C in dwbp per W3C in prov-overview,
6. must provide at least minimal data version and version-history information within metadata per W3C in dwbp,
7. must provide at least minimal data coverage information within metadata per W3C in dwbp,[^11]
8. must provide at least minimal `csv` dialect information within metadata per FD in csv-dialect,
9. must use at least one persistent resolvable URI ie IRI per TCL per W3C in webarch per W3C in dwbp per W3C in ld-bp per W3C in tabular-data-primer per W3C in cooluris per W3C in ldp-bp,[^10]
10. must be translatable ie convertible to `rdf` format per TCL per W3C in dwbp per W3C in ld-bp per W3C in tabular-data-primer,[^7]
11. xxx

## authorities

- [W3C](https://www.w3.org/TR/?tag=data&version=latest),
- [TCL](https://librarycarpentry.org/Top-10-FAIR/2018/12/01/historical-research/),
- [TCD](https://datacarpentry.org/spreadsheet-ecology-lesson/02-common-mistakes/),
- [DDI](https://en.wikipedia.org/wiki/Data_Documentation_Initiative),//needs review as of 14 aug 2022
- [BW](https://doi.org/10.1080/00031305.2017.1375989),
- [MD](https://doi.org/10.3200/HMTS.37.1.34-38), //needs review as of 14 aug 2022 - started but unfinished as of 21.10
- [RM](https://doi.org/10.1093/jsh/shab015)//needs review as of 14 aug 2022
- [HK](https://doi-org.ezp-prod1.hul.harvard.edu/10.1080/01615440.2018.1484676),//needs review as of 14 aug 2022 - finished 19.49
- [IDS](https://maastrichtu-ids.github.io/best-practices/blog/2021/03/18/build-a-kg/)//needs review as of 14 aug 2022 - finishd 19.18
- [KBHS](https://link-springer-com.ezp-prod1.hul.harvard.edu/chapter/10.1007/978-3-319-49304-6_31)//needs review as of 14 aug 2022 - finished 19.02
- [MHJN](https://www.researchgate.net/publication/329031219_Csv2rdf_Generating_rdf_data_from_csv_file_using_semantic_web_technologies)//needs review as of 14 aug 2022 - finished prior to 18.54
- [BGT](http://search.proquest.com.ezp-prod1.hul.harvard.edu/scholarly-journals/migrating-complex-classification-scheme-semantic/docview/2543608213/se-2?accountid=11311)//needs review as of 14 aug 2022 - finished 18.53
- [LOA](http://search.proquest.com.ezp-prod1.hul.harvard.edu/scholarly-journals/rdfizing-biosynthetic-pathway-i-e-coli-o-antigen/docview/2611239195/se-2)//needs review as of 14 aug 2022 finished 18.39
- [ADBD](http://search.proquest.com.ezp-prod1.hul.harvard.edu/scholarly-journals/evaluation-uplift-mapping-languages/docview/1966401153/se-2?accountid=11311)//needs review as of 14 aug 2022 finished 18.27
- [GBSL](http://search.proquest.com.ezp-prod1.hul.harvard.edu/scholarly-journals/shexml-improving-usability-heterogeneous-data/docview/2463305655/se-2)//needs further review as of 14 aug 2022 finished 18.14
- [CF](https://www.semantic-web-journal.net/content/enhancing-virtual-ontology-based-access-over-tabular-data-morph-csv-0)//needs further review as of 14 aug 2022 - review started 17.44 finished 18.03
- [ASW](https://github.com/semantalytics/awesome-semantic-web/blob/master/README.md)//needs further review as of 14 aug 2022 - review started null finished 17.11
- [MHJN](http://www.jatit.org/volumes/Vol96No20/19Vol96No20.pdf)//needs further review as of 14 aug 2022 - review finished 17.32
- [FD](https://frictionlessdata.io)//needs further review as of 14 aug 2022 - review done
- [OGC](https://en.wikipedia.org/wiki/Open_Geospatial_Consortium),
- [JT](https://github.com/JeniT/linked-csv)//needs review as of 14 aug 2022
- [SW](https://csvw.org)//needs review as of 14 aug 2022 - finished 17.42
- [TO](https://core.ac.uk/display/301654646)//needs review as of 14 aug 2022 - finished 20.18
- [PH](http://programminghistorian.org/en/about)//needs review as of 14 aug 2022 - finished 14 aug 2022
- [AHA](https://www.historians.org/jobs-and-professional-development/statements-standards-and-guidelines-of-the-discipline)
- [UKDA](https://www.data-archive.ac.uk/managing-data/standards-and-procedures/)
- [COS](https://www.cos.io/initiatives/top-guidelines]).

## references

- W3C in [webarch](https://www.w3.org/TR/webarch/),
- W3C in [dwbp](https://www.w3.org/TR/dwbp/),
- W3C in [ld-bp](https://www.w3.org/TR/ld-bp/),
- W3C in [sdw-bp](https://www.w3.org/TR/sdw-bp/),
- W3C in [prov-overview](http://www.w3.org/TR/prov-overview/),//needs review as of 14 aug 2022
- W3C in [tabular-data-primer](https://www.w3.org/TR/tabular-data-primer/),
- W3C in [tabular-data-model](https://www.w3.org/TR/tabular-data-model/),
- W3C in [csv2json](https://www.w3.org/TR/2015/REC-csv2json-20151217/),
- W3C in [csv2rdf](http://www.w3.org/TR/csv2rdf/),
- W3C in [tabular-metadata](https://www.w3.org/TR/2015/REC-tabular-metadata-20151217/),
- W3C in [rdb-direct](http://www.w3.org/TR/rdb-direct-mapping/),//possibly not relevant as regards SQL skimmed on 14 aug 2022 - though may become relevant if it proves easier to store data in SQL rather than CSV, or if CSV -> SQL -> RDF proves easier than CSV -> RDF eg possibly using [PostgreSQL](https://www.postgresql.org) or MySQL per [Stack](https://insights.stackoverflow.com/survey/2021#section-most-loved-dreaded-and-wanted-databases)
- W3C in [mull](https://www.w3.org/TR/?tag=data&status=REC&version=latest).//needs review as of 14 aug 2022
- W3C in [cooluris](https://www.w3.org/TR/cooluris/)//needs review as of 14 aug 2022
- W3C in [ldp-bp](https://www.w3.org/TR/ldp-bp/)//needs review as of 14 aug 2022 - review started 14.09 finished 14.19
- W3C in [ld-glossary](https://www.w3.org/TR/ld-glossary/),
- FD in [data-resource](https://specs.frictionlessdata.io/data-resource/)//needs review as of 14 aug 2022 - superseded by FD in tabular-data-resource
- FD in [data-package](https://specs.frictionlessdata.io/data-package/)//needs review as of 14 aug 2022 - superseded by FD in tabular-data-package
- FD in [csv-dialect](https://specs.frictionlessdata.io/csv-dialect/)
- FD in [table-schema](https://specs.frictionlessdata.io/table-schema/)
- FD in [tabular-data-resource](https://specs.frictionlessdata.io/tabular-data-resource/)
- FD in [tabular-data-package](https://specs.frictionlessdata.io/tabular-data-package/)
- AHA in [statement](https://www.historians.org/jobs-and-professional-development/statements-standards-and-guidelines-of-the-discipline/statement-on-standards-of-professional-conduct#SharedValues)//needs review as fo 14 aug 2022 - finished 21.35 but found no suitable standards
- COS in [top](https://osf.io/9f6gx/wiki/Guidelines/)//needs review as of 14 aug 2022

## footnotes

[^1]: file created 14 aug 2022 in boston MA. file may use terms as in W3C in ld-glossary.

[^2]: per [[output.md]], the structure we are meant to have is a graph construed as follows (variously called a quiver ie directed pseudograph ie directed graph ie digraph ie directed multigraph eg [per wolfram](https://mathworld.wolfram.com/Pseudograph.html) and eg [per ncatlab](https://ncatlab.org/nlab/show/pseudograph).

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
      - ie for `md` [null],
      - ie for `rdf` [null] further validated eg by [W3C RDF-validator](http://www.w3.org/RDF/Validator/)
      - ie for spatial data ensure values meet technical specifications per W3C in sdw-bp or tech specs for [GeoJSON](https://geojson.org) or tech specs for [GeoPackage](https://en.wikipedia.org/wiki/GeoPackage) or tech specs for [ArcGIS Online](http://desktop.arcgis.com/en/arcmap/10.3/manage-data/geodatabases/what-is-a-geodatabase.htm) or [ArcGIS Hub](https://doc.arcgis.com/en/hub/content/add-and-manage-groups.htm#ESRI_SECTION1_D0B2443A64F349BD95ED2094D9A80912) or [GDAL-accepted formats](https://gdal.org/drivers/vector/csv.html),//though GDAL or GeoJSON most preferred, and ArcGIS least preferred as of 14 aug 2022
      - ie for textual quote ie transcription data ensure values meet technical specs per TEI,
      - ie for date-time data ensure values meet technical specs per [null].

[^4]: the most useful of which seem to be the following.

      - those built or used in programming language specifications, eg for [TEI](https://tei-c.org/release/doc/tei-p5-doc/en/html/index.html), [RDF](http://www.w3.org/TR/rdf-primer), [RDF Schema](https://en.wikipedia.org/wiki/RDF_Schema) ie [RDFS](https://www.w3.org/TR/rdf-schema/), [RDF Data Cube](https://www.w3.org/TR/vocab-data-cube/), [XML](https://en.wikipedia.org/wiki/XML), [XML Schema](https://en.wikipedia.org/wiki/XML_Schema_(W3C)), [JSON](https://en.wikipedia.org/wiki/JSON) and [RDF Data Cube extensions](https://www.w3.org/TR/qb4st/), [JSON-LD](https://en.wikipedia.org/wiki/JSON-LD), [CSV by W3C](https://www.w3.org/2013/csvw/wiki/Main_Page), [CSV by FD](https://specs.frictionlessdata.io//tabular-data-package/), [CVS by JT](https://github.com/JeniT/linked-csv), [OWL](http://www.w3.org/TR/owl-overview), inc namespace namespaces ie QNames for [XML](http://www.w3.org/TR/xml-names11) inc language-independent namespaces eg [CURIEs](http://www.w3.org/TR/curie)
      - upper level ontologies eg [BFO](http://xmlns.com/foaf/spec/) or [schema.org](https://schema.org) or [wikidata](https://www.wikidata.org/wiki/Wikidata:Main_Page) or its derivative [DBpedia](https://www.dbpedia.org/about/) or [gist](https://www.semanticarts.com/gist/) or commonest ones as per the [LOV directory](https://lov.linkeddata.es/dataset/lov/),
      - vars lower level ontologies or vocabs eg those
             + for authorities ie authors etc eg [LCNAF](http://id.loc.gov/authorities/names.html), [VIAF](https://viaf.org/), ISNI, and further for non-natural persons eg [ORG](http://www.w3.org/TR/vocab-org/)
             + for human networks ie human-human edges etc eg [FOAF](http://xmlns.com/foaf/spec/),
             + ISO-related ones eg [ISO 639](https://www.loc.gov/standards/iso639-2/php/code_list.php) for languages, [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) for date-times, [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html) for currency, [ISO 3166](https://www.iso.org/iso-3166-country-codes.html) for countries, [null] for [null],
             + geographic eg [Getty TGN](http://www.getty.edu/research/tools/vocabularies/tgn/index.html), [GeoNames](https://www.geonames.org), [LinkedGeoData](http://linkedgeodata.org),
             + bibliographic-cataloguing eg [LCSH](http://id.loc.gov/authorities/subjects.html) or its derivative [FAST](https://www.oclc.org/research/areas/data-science/fast.html), [UNESCO](http://vocabularies.unesco.org/thesaurus), [ICPSR](https://www.icpsr.umich.edu/icpsrweb/ICPSR/thesaurus/index), [CIDOC CRM](https://cidoc-crm.org), [EAD](https://en.wikipedia.org/wiki/Encoded_Archival_Description),
             + for metadata eg [Dublin Core ie DCMI](https://www.dublincore.org), [IOA](https://ontobee.org/ontology/IAO), [DDI](http://www.ddialliance.org/controlled-vocabularies), [SKOS](http://www.w3.org/2004/02/skos/core), [DCAT](https://www.w3.org/TR/vocab-dcat/), [VOID](http://www.w3.org/TR/void/) (a derivative of Dublin Core and RDF Schema), [QUDT](https://www.qudt.org) (eg for datatypes),
             + for licensing eg [CC](https://lov.linkeddata.es/dataset/lov/vocabs/cc).

[^5]: eg following [Robertson best practices](http://sethrobertson.github.io/GitBestPractices/) though HK further require or recommend use of work-process-history to report and discuss and explicitly describe data transformations inc data selection, modelling, normalisation, classification, and linking eg within journal article per HK while TO further require or recommend discussion of data-source and data-discovery-tools biases, limitations etc inc repository collection policies, digitisaiton procedures, OCR quality, catalogue or finding aid quality, error correction and search ie query procedures per TO further eg when choosing amongs [PH-listed tools](http://programminghistorian.org/en/lessons/?topic=web-scraping) per PH and further MD require or recommend information re source selection and critaria, data entry, integration, standardisation, and storage, and enrichment and release actions be divulged per MD.//TO and HK and MD**standards not met**by git-versioning and so not met by `sec 1` process as of 14 aug 2022 - addendum 0 at 22.10 - may need to keep something akin to a lab-notebook ie a log of all work done eg in the [OSF online log by the COs](https://www.cos.io/initiatives/top-guidelines) or to adopt [COS in top](https://osf.io/9f6gx/wiki/Guidelines/) standards - addendum 1 at 22.33 - will likely need to amend `sec 2` to conform to science-like standards eg registration in the OSF registry of the research project

[^6]: eg raw data files deposited in [CoreTrustSeal-certified repositories](https://www.coretrustseal.org/why-certification/certified-repositories/) eg [DANS](https://easy.dans.knaw.nl/ui/home) eg [Zenodo](https://zenodo.org) further eg deposit in API-equipped repositories per W3C in dwbp further eg[*Nature*-listed repositories](https://www.nature.com/sdata/policies/repositories) further eg [Google-indexed repositories](https://developers.google.com/search/docs/advanced/structured-data/dataset) further eg [LOD Cloud-indexed dataset](https://lod-cloud.net).

[^7]: esp by machines eg [OpenRefine](https://openrefine.org) and esp to RDF as this facilitates (vs allows?) translation to XML or JSON-LD per W3C in ld-bp [sec convert](https://www.w3.org/TR/ld-bp/#CONVERT) and further browse list of translators, processors ie parsers, etc in [ASW](https://github.com/semantalytics/awesome-semantic-web/blob/master/README.md) and further browse list of vars standard translation algorithms per GBSL.

[^8]: BW suggest string "NA" for missing data, and not blank cells nor number -999 nor number 999 for missing data. TCD suggest a blank cell, "NA", "na", or "NULL" and not -999 nor 999.

[^9]: where per BW minimal data dictionary explains all variables used eg lists exact variable name as used in data files, give any alternative variable names used elsewhere, an explanation [definition? elucidation?] of the variable, measurement units of the variable, min and max values of the variable values.

[^10]: eg use up to one [and at least one?] URI per resource eg per vertex, edge, record, dataset-splice or series, dataset, etc where said URI uses [IANA-registered scheme](http://www.iana.org/assignments/uri-schemes/uri-schemes.xhtml) per W3C in webarch eg [PURL](https://purl.archive.org) per W3C in ld-bp eg [PermID](http://permid.org/) per ASW eg [W3ID](https://rml.io/yarrrml/matey) per IDS.

[^11]: W3C in dwbp no 28 give eg as preserving ie archiving all or at least at-risk third-party (online) resources which are referenced by dataset.

[^12]: compare to other processes in eg
       - in MHJN (journal article pub 31 oct 2018) used `csv` to `rdf` via three algorithms ie `cvs` is parsed -> embedded metadata created or approximated in `json` -> data converted to `rdf` where algorithms written in Java and named CSV2RDF though name is ambiguous as of 14 aug 2022
       - in SW (non-journal article by UK for-profit Swirrl) recommends `csv` to `rdf` via metadata manually created inc first- and third-party URIs -> input `csv` and `json` into a [validator or converter](https://csvw.org/tools.html) -> validate -> convert to `rdf`,
       - in CF (preprint article pub 11 jun 2020 or 6 nov 2020) used `csv` to `sql` to `rdf` via algorithm written in SPARQL and named [Morph-CSV](https://morph.oeg.fi.upm.es/tool/morph-csv) //this seems well-documented and tested as of 14 aug 2022 18.02
       - in GBSL (journal article pub 23 nov 2020) used `xml` + `json` to `rdf` but listed vars standard translation ie transformation algorithms in pages 3-6,
       - in ADBD (journal article pub 2017) used `csv` to `rdf` via algorithm written in `null` called FunUL though could not located this in `github` nor elsewhere online as of 14 aug 2022
       - in LOA (journal article pub 2021) used `csv` to `rdf` via standardising data-values in defined programming-language -> manually creating URIs via third-party -> input `csv` into Python-based converted called [RDFLib](https://gitlab.com/lsunmyoung/rdfization) -> get `rdf` in Turtle dialect -> validate output via SPARQL,
       - in BGT (journal article pub 2021) used `csv` to `skos` via `.NET`-based [STELETO](https://github.com/cbinding/STELETO/) transformation tool,
       - in KBHS (journal article pub 2016) used `csv` to `rdf` though does not cover the full process in detail,
       - in IDS (non-journal article by non-profit institute) used `csv` to `rdf` via YARRRML-based programme [Matey](https://rml.io/yarrrml/matey),
       - in [null]