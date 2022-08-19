# work-output

## abstract

this document specifies the work output expected within three weeks.[^1]

## final

- note 0 - this section lists final standards or specifications for the work output, while sections following this one are more free-form or exploratory.
- note 1 - we divide standards into conceptual and non-conceptual, where conceptual standards or specifications determine non-conceptual ones or are more fundamental than the latter
- note 3 - in which case, conceptual standards are
	+ as per end 0 to end 2 in the `conceptually` section where, for end 2 item (iv) we let total unary function d = d: E to P(V^2) ie the powerset of the cartesian product of V and V, as we want d to give all vertices connected by any given edge, not just some vertex.
- note 4 - further, non-conceptual standards are
	+ further subdivided into algorithmic and non-algorithmic, where the former are standards for the work itself, while the latter are standards for the output.
		* algorithmic standards to be collected in `work.txt` though not added to the file as of 13 Aug 2022,
		* non-algorithmic standards are - 
			0. need all vertices and edges within at least one cs-ontology ie vocabulary ie W3C namespace
			1. need [all? some?] vertices, edges, etc matched to a globally unique persistent URI
			2. need all files encoded in UTF-8
			3. [vars other standards further down this doc]  

## conceptually

- note 0 - the work output is conceived of as a graph of unlabbelled vertices ie points and unlabelled edges from point to point ie edges ie relations, with each point or edge enumerated ie indexed by a natural number and mapped to exactly one alphanumeric string. That is, let V be a finite subset of the natural numbers {0,1,2,...} ie let V = {0,1,2,...,n}. We let E be a subset of the product V*V ... [branched into another idea]
- note 1 - okay, the work output is conceived of as a graph ie the structure G = (V,E) ie the ordered pair G = (V,E) where the first member of the pair is a set of vertoices ie points and the second member of the pair is a set of edges. as primitives we have points, [at this point unsure if edges are primitive in addition to points]
- note 2 - we probably want a finite set V and a finite set E. Further we want directed edges in E, but would this allow for edges to represent unary relations ie properties? We further want edges and points to be labelled, to build a multigraph where each edge represent distinct relations. And we allow loops ie an edge from one point to the same point. We also want a non-empty set V and non-empty set E, of course.
- note 3 - to clarify, a directed graph is one where edges have an orientation, so it seems like we would want this, but this may afford us less flexibility to encode unary relations ie loops. But directed graphs may have loops! according to https://en.wikipedia.org/wiki/Directed_graph
- note 4 - the final structure we're after seems to be a directed multigraph https://en.wikipedia.org/wiki/Multigraph and more specifically a directed multigraph permitted to have loops each of whose nodes and edges are labelled ie each has an identity
- note 5 - so the final structure we're after seems to be a quiver https://en.wikipedia.org/wiki/Quiver_(mathematics) ie a directed multigraph with labelled nodes and edges and which may have loops :) Further, our quiver is a 4-tuple G = (V, A, s, t) with V set of vertices, A set of edges, s: A to V assigning each edge its source vertex, t: A to V assigning each edge its target node ie target vertex.
- note 6 - or, alternatively, we can let graphs be 3-tuples G = (V, E, d) with d being a mapping that, somehow, interprets edges as pairs of vertices. 
- note 7 - again, alternatively, out final structure might be a directed pseudograph ie directed graph ie digraph ie quiver defined as a 3-tuple G = (V, E, d) with d: E to V^2 where V^2 is the cartesian product of V and V. See https://mathworld.wolfram.com/Pseudograph.html and further see https://ncatlab.org/nlab/show/pseudograph

- end 0 - re primitives, we have points, sets, and the like [I think].
- end 1 - re basic definitions
	(i)	let naturals set N = {0,1,2,...}, 
	(ii)	let a binary relation ~ [tilde] on set A and set B be set R = ~ a subset of A * B ie of the cartesian product of A and B where we allow A = B, 
	(iii)	let a partial unary function f from set A to set B ie a unary function f from set A to set B be a binary relation ~ on set A and set B where for any a in A if a ~ b_i and a ~ b_j then b_i = b_j if if f(a) = b_i and f(a) = b_j then b_i = b_j,
	(iv)	let a total unary function f from set A to set B be a unary function f from set A to set B where for any a in A there is at least one b such that f(a) = b.
- end 2 - re structural definitions
	(i)	let set V = {0,1,2,...,n) for natural n>0, 
	(ii)	let set E = {0,1,2,...,m) for natural m>0,
	(iii)	let set V^2 be the cartesian product of V and V,
	(iv)	let total unary function d: E to V^2,
	(v)	let graph G = (V, E, d).

### re set V in G

- note 0 - how many vertices do we have in V, and what are they?
- note 1 - we likely have several thousand, but likely less than 100,000 vertices, so n < 100,000, likely.
- note 2 - how will we make sense of them? for this we probably need an ontology, the top level of which is entity eg https://www.wikidata.org/wiki/Q35120 or thing eg https://schema.org/docs/full.html
- note 3 - to make sense of the vertices in V ie to visualise them we'll need an ontology as defined in computer science ie a cs-ontology ie https://en.wikipedia.org/wiki/Ontology_(information_science)
- note 4 - towards building a cs-ontology it looks like we first need an upper cs-ontology ie https://en.wikipedia.org/wiki/Upper_ontology ie https://digitaltwinhub.co.uk/top-level-ontologies/ ie https://ontology4.us/english/Ontologies/Upper-Ontologies/ and it looks like we can navigate published upper cs-ontologies using software Protege https://protege.stanford.edu/ [though this software comes with a learning curve]
- note 5 - we probably want all vertices to be things, and have these split into disjoing parts with one being strings and the other being non-strings ie data and not data

- draft 0 - re level 0 of cs-ontology tree ie subsumes all vertices
	0	let entity be any vertex.
- draft 1 - re level 1 of cs-ontology tree ie partitions V into two disjoint non-empty subsets
	0.0	let extended-entity be vertices with extended referents ie vertices referring to or identifying things in spacetime ie entity per https://github.com/bfo-ontology/BFO/wiki ie entity per https://www.wikidata.org/wiki/Q35120 ie thing per https://schema.org/Thing,
	0.1	let non-extended-entity be vertices without extended referents ie vertices referring to or identifying things not in spacetime ie abstract things 
- draft 2 - re level 2 of cs-ontology tree ie partitions V into four disjoint subsets
	0.0.0	let continuant-extended entity = continuant per https://github.com/bfo-ontology/BFO/wiki
	0.0.1	let non-continuant-extended entity = occurrent per https://github.com/bfo-ontology/BFO/wiki
	0.1.0	let string-like-[stopped here]
	0.1.1	[missing]

- note 6 - after some time writing draf 0 to draft 2 I think it might be better to keep level 0 of draft 0, and skip intermediate levels in draft 1 and draft 2 to simply get to some specific-enough level n. though at this point, at level n, would we like non-empty disjoint subsets of V? possibly we might use BFO for all upper level cs-ontology, though BFO 2.0 does not include mathematical structures [though BFO authors suggest https://ontobee.org/ontology/IAO for a mostly-compatible lower level cs-ontology].

- end 0 - re BFO upper level cs-ontology
	0	let entity = http://purl.obolibrary.org/obo/BFO_0000001
	0.0	let continuant = http://purl.obolibrary.org/obo/BFO_0000002
	0.1	let occurrent = http://purl.obolibrary.org/obo/BFO_0000003
- end 1 - re lower level cs-ontology, likely use IAO for data and OWL https://www.w3.org/TR/owl2-overview/ [also https://www.w3.org/TR/owl2-quick-reference/] or RDF https://www.w3.org/TR/rdf-schema/ by W3C for metadata definitions?

### re set E in G

- note 0 - how many edges do we have in E, and what are they? 
- note 1 - note 0 query likely to be answered in the same way proposed in end 0 and end 1 of above section re set V in G.

### re total unary funtion d in G

- note 0 - this should be as simple as specifying d fully.

## specification

- note 0 - how do we visualise or draw or write out the structure we will build?
- note 1 - wiki said [any? some?] graph may be fully specified by an adjacency matrix https://en.wikipedia.org/wiki/Adjacency_matrix
- note 2 - must follow W3C data recommendations https://www.w3.org/TR/?tag=data&status=REC&version=latest esp best practices https://www.w3.org/TR/2017/REC-dwbp-20170131/ and vars others

## best practices 

- do use git https://en.wikipedia.org/wiki/Git for version control. Best practices at http://sethrobertson.github.io/GitBestPractices/
- do use UTF-8 https://en.wikipedia.org/wiki/UTF-8 for encoding.

### FAIR
#### https://librarycarpentry.org/Top-10-FAIR/2019/09/05/linked-open-data/ re linked data

- note 0 - skimmed but did not list these standards as they seem similar to W3C ones.

#### https://librarycarpentry.org/Top-10-FAIR/2018/12/01/historical-research/ re historical research

- do make data findable per Thing 1 eg deposite in CoreTrustSeal-certified repositories https://www.coretrustseal.org/why-certification/certified-repositories/ eg DANS EASY https://easy.dans.knaw.nl/ui/home and further eg https://zenodo.org
- do provide metadata for dataset per Thing 2
- do get a persistent URI for dataset per Thing 3 eg a DOI
- do make data as open as possible per Thing 4,
- do structure and organise data well per Thing 5 though note many historians capture data in spreadsheets per https://doi.org/10.1080/00031305.2017.1375989
- do use controlled vocabs or ontologies per Thing 6 eg CIDOC CRM for concepts http://www.cidoc-crm.org/concept-search, VIAF or LC for authorities, UNESCO history thesaurus http://vocabularies.unesco.org/browser/thesaurus/en/page/concept302, GeoNames for locations https://www.geonames.org/ or eg using Swoogle directory http://swoogle.umbc.edu/2006/ or eg using LOV directory https://lov.linkeddata.es/dataset/lov/,
- do convert raw data into an RDF format per Thing 7 eg using OpenRefine http://openrefine.org/ or other sofware,
- do licence your data per Thing 8 eg use https://creativecommons.org/choose/,
- do properly cite data you used for your dataset per Thing 9,
- do follow relevant data-availability policies per Thing 10,

### Broman and Woo
#### https://doi.org/10.1080/00031305.2017.1375989 ie tsv or csv humanities data

- do use spreadsheet programs for data entry and storage [ie for authoritative copy of data], and use non-authoritative copies of your data for analysis and visualisation, preferrably in non-spreadsheet programs,
- do be consistent in whatever you do eg use for categorical values eg for missing values eg for variable names eg for real-world-things identifies, for file names, for dates, for phrases within natural language notes,
- do explain missing data values in a separate place, using a consistent fixed code for missing data eg "NA" for R-language processing, but not -999 nor 999,
- do prefer the standard yyy-mm-dd for dates,
- do avoid extraneous spaces in strings eg "glucose" vs "glucose ",
- do avoid all special characters other than underscores and hyphens
- do fill in all cells ie leave no empty cells eg enter "NA" for missing data,
- do put just one piece of data in a cell eg do not include notes about a data-value within the cell containing that data-value itself,
- do place only one table per sheet,
- do write a data dictionary in a separate file explaining all variables eg include exact variable name as used in datafiles, any alternative variable names used elsewhere, an explanation of the variable, measurement units of the variable, min and max values of the variable,
- do not include any calculations ie formulas in raw data files ie primary data file should be "a pristine store of data" which is write-protected ie locked, backed up, and not to be touched, eg for analysing your data make copies of it and use those,
- do not use font colour nor highlighting as data,
- do make regular backups of data eg use git [which is not ideal for data files] or dat https://datproject.org/
- do validate your data to avoid errors eg use automated data validation tools
- do save datafiles in csv files

### Data Carpentry
#### https://datacarpentry.org/spreadsheet-ecology-lesson/02-common-mistakes/ re tsv or csv data

- do not create multiple tables wihtin one spreadsheet,
- do not create multiple tabs within your spreadsheet-program eg instead add another column to your existing table,
- do not leave blank cells,
- do not use problematic null values eg -999 to represent missing data-values, eg use data-cleaning tool OpenRefine http://www.datacarpentry.org/OpenRefine-ecology-lesson/, rather use a clearly defined and consistent null indicator eg [a blank cell], "NA", "na", or "NULL",
- do not use text formatting to convey information eg cell highlighting, italics, etc,
- do not enter more than one piece of information per cell
- do use descriptive variable names, but exclude spaces, numbers [though "Obervation_01" given as a good variable name example], and special characters other than underscores
- do not use special characters in your data eg line breaks, em-dashes, accents, delimiters [commas, tabs] etc.
- do not include metadata in your data file itself eg adding legend within your data-containing csv, rather store in a separate file, preferably in plain text

### W3C

- note 0 - publishes vars relevant standards per https://www.w3.org/TR/?tag=data&status=REC&version=latest inc
	- DCAT https://www.w3.org/TR/2020/REC-vocab-dcat-2-20200204/
	- Data on the Web BP https://www.w3.org/TR/2017/REC-dwbp-20170131/
	- Generating JSON from Tabular Data on the Web https://www.w3.org/TR/2015/REC-csv2json-20151217/
	- Generating RDF from Tabular Data on the Web https://www.w3.org/TR/2015/REC-csv2rdf-20151217/
	- Model for Tabular Data and Metadata on the Web https://www.w3.org/TR/2015/REC-tabular-data-model-20151217/
	- Metadata Vocab for Tabular Data https://www.w3.org/TR/2015/REC-tabular-metadata-20151217/
	- A Direct Mapping of Relational Data to RDF https://www.w3.org/TR/2012/REC-rdb-direct-mapping-20120927/
	- various vocabs or ontologies called "namespaces" eg namespace `rdfs` = http://www.w3.org/2000/01/rdf-schema#

#### https://www.w3.org/TR/webarch/ ie general online-resources good practices

- do use exactly one URI for each online resource inc data strings, records, data series, etc
- do use only IANA-registered URI schemes http://www.iana.org/assignments/uri-schemes/uri-schemes.xhtml

#### https://www.w3.org/TR/dwbp/ ie general data best practices

- do follow https://www.w3.org/TR/webarch/ principles [good practices?],
- do use [standardised, published] vocabularies and standards eg https://www.w3.org/TR/2017/REC-dwbp-20170131/#namespaces eg directory https://lov.linkeddata.es/dataset/lov/
- do provide descriptive structured metadata [er best practices 1-3 inc in human and machine readable formats eg using vocabularies DCMI or DCAT, though DCAT recommended by W3C for descriptive metadata for datasets
- do provide data licence info [in metadata] per best practice 4,
- do provide data provenance info per best practice 5,
- do provide data quality info per best practice 6, eg using vocab DQV,
- do provide a version indicator per best practice 7,
- do provide a version history per best practice 8,
- do use persistent URIs for and within dataset per best practices 9-11 [inc dataset versions and sub-dataset series],
- do use machine-readable location-neutral standardised data formats per best practices 12-13, though include location metadata for data formats which cannot be location-neutral eg strings of natural language,
- do provide data in multiple formats per best practice 14,
- do reuse vocabularies ie ontologies preferrably standardised ones per best practice 15,
- do opt for vocabularies ie ontologies that fit both data and use per best practice 16 [eg following other historical datasets],
- do provide bulk dataset download per best pract 17,
- do provide subsets for large datasets per best practice 18 eg using slices as defined in http://www.w3.org/TR/vocab-data-cube/,
- do use content negotiation when serving data per best pract 19,
- do provide data in real time or near real time per best practice 20,
- do provide up-to-date data per best practice 21,
- do provide an explanation for data that is not available per best practice 22,
- do make data available via a well-documented standards-compliant API per best practices 23-27,
- do preserve data identifiers esp URIs per best practice 27,
- do assess dataset coverage per best practice 28 eg preserve all third-party resources referenced from the data,
- do gather feedback from data users per best practice 29,
- do make feedback available per best practice 30,
- do enrich data by generating new data that complements existing data per best practices 31-32,
- do provide feedback to publishers of data used in your dataset per best practice 33,
- do follow licensing terms per best practice 34,
- do cite the ogirinal source of data per best practice 35.

#### https://www.w3.org/TR/ld-bp/ ie linked data best practices

- do use URIs eg https://purl.archive.org for vars strings per https://www.w3.org/TR/ld-bp/#HTTP-URIS
- do use standardised vocabs ie cs-ontologies per https://www.w3.org/TR/ld-bp/#VOCABULARIES
- do plan on converting raw data for G to RDF language using any of vars automated translation tools per https://www.w3.org/TR/ld-bp/#CONVERT, esp as RDF language may be [automatically] converted to XML and JSON-LD.

#### https://www.w3.org/TR/sdw-bp/ ie spatial data best practices

- do use a coordinate reference system eg WGS 84 https://en.wikipedia.org/wiki/World_Geodetic_System and further see coordinate reference systems directory http://www.epsg.org/ and further eg Web-Mercator http://epsg-registry.org/?display=entity&urn=urn:ogc:def:crs:EPSG::3857 for spatial data as a raster image
- do useg globally unique http URIs for and within datasets per best practice ie bp 1 eg DBPedia, GeoNames,
- do make spetial data indexable by search engines per bp 2 eg by pushing an html page for the dataset and each spatial thing it describes, and further making sure said page is crawled,
- do link to third-party online resources per bp 3,
- do represent spatial data in a way that fits its target audience per bp 4 eg in HTML per https://www.w3.org/TR/sdw-bp/#table-formats-matrix,
- do provide sufficiently-specified machine-readable geometric data per bp 5-6 eg GML https://www.w3.org/TR/sdw-bp/#bib-GML or GeoJSON https://www.w3.org/TR/sdw-bp/#bib-RFC7946 or further eg for points http://geohash.org/ or for sub-divisions eg http://gadm.geovocab.org
- do use coordinate reference systems suitable to your users per bp 7
- do state how coordinate values are encoded per bp 8 eg label lat and long, label their units, and give the datum used by the relevant coordinate reference system in metadata
- do provide relative positioning data per bp 9,
- do use proper relation-types to link spatial data per bp 10
- vars other bp [stopped reading here]

#### https://www.w3.org/TR/prov-overview/ ie data provenance best practices

#### https://www.w3.org/TR/tabular-data-primer/ ie csv best practices

- do use csv per section ie sec 1.1
- do provide a metadata file in JSON for entire table and columns within it, and further validate metadata and csv with an automated validator, eg using Dublin Core, DCAT, schema.org per sec 1.2-1.3 and 2.1-2.3,
- do include table, range, or cell annotations in the metadata file per section 2.4
- do validate csv files per sec 3.1-3.14,
- do transform [copies of] csv files to JSON and RDF
- do use vars vocabs ie "namespaces" for your csv metadata eg RDF https://www.w3.org/2011/rdfa-context/rdfa-1.1
- [vars other standards in sec 4 re specific data values and their metadata for correct translation]


#### https://www.w3.org/TR/tabular-data-model/ ie csv best practices too

- do annotate ie provide metadata for cells, rows, columns, tables ie csv files, and groups of tables ie csv files ie your dataset per sec 4,
- do only use Unicode characters to input strings in csv per sec 4 prior to sec 4.1,
- do use UTF-8 encoding per sec 7.2,
- [pers note] may want string values even in csv to follow XML format eg input "&amp;" to encode "&" etc per https://en.wikipedia.org/wiki/XML maybe following additionally TEI Guidelines https://tei-c.org/release/doc/tei-p5-doc/en/html/index.html eg with customised schema https://tei-c.org/about/frequently-asked-questions/


[^1]: This txt file created 12 August 2022 in Boston MA by A Navidad.