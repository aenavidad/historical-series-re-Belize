# standards

{{TOC}}

## abstract

this file has the following contents.[^file created 16 aug 2022 in Boston MA.]

1. `standards` lists the sources of standards which were considered for inclusion in this document,
2. `process standards` lists standards accepted for work process,
3. `output standards` lists standards accepted for work output, including data and non-data output.

note these conventions.

- `work` inc only actions ie processes ie events eg thought of as an algorithm taking in data and outputing data
- `data` inc only version 1.5 data-files and metadata-files and raw-data-files
- `text` inc only pre-print and post-print ie accepted manuscripts and published manuscripts
- `work-files` inc all non-`data` and non-`text` files used or resulting from `work` eg work-log, non-versioned data-files, non-versioned-metadata-files, non-versioned-raw-data-files, and the like, but excluding third-party data or. articles used in `work` eg published books and journal articles
- `process` inc `work` and `work-files` only
- `output` inc `data` and `text` only

## standards

### all

| body | standards[^vars standards excluded for being rather programming-language specifications or dialects. relevant standards not found in [EQUATOR](https://www.equator-network.org) on 16 aug 2022 9.56.] | adoption[^inc partial adoption or adoption after interpretation or modification.] | notes |
|:--|:--|:--|:--|
| [W3C](https://www.w3.org) | [webarch](http://www.w3.org/TR/webarch/) | `yes` |‌ re web generally |
| [W3C](https://www.w3.org) | [dwbp](https://www.w3.org/TR/dwbp/) | `yes` |‌ re online data |
| [W3C](https://www.w3.org) | [ld-bp](http://www.w3.org/TR/ld-bp/) |  `yes` |‌ re linked data |
| [W3C](https://www.w3.org) | [prov](http://www.w3.org/2005/Incubator/prov/XGR-prov/) |  `yes` |‌ re data provenance |
| [OKF](https://okfn.org) | [Frictionless Standards](https://frictionlessdata.io/standards)[^ie Data Protocols announced [17 July 2012 by Rufus Pollock](https://blog.okfn.org/2012/07/17/data-protocols-community-based-light-weight-data-protocols-for-collaborative-distributed-work-with-data/).] | `yes` | `null` |
| [OKF](https://okfn.org) | [Open Definition](https://opendefinition.org) | `yes` | not reviewed as of 6.30 |
| [FOSTER](https://www.fosteropenscience.eu/about)[^EU-funded project (unincorporated body?) 2014 to present.] | [Open Science Training Handbook](https://open-science-training-handbook.gitbook.io/book/) | `null` | not reviewed as of 6.32 |
| [AHA](https://www.historians.org) | [Statement on Standards of Professional Conduct 1987-2019](https://www.historians.org/jobs-and-professional-development/statements-standards-and-guidelines-of-the-discipline/statement-on-standards-of-professional-conduct#SharedValues) | `no` | language too vague |
| [NCPH](https://ncph.org) | [Code of Ethics and Professional Conduct 2007](https://ncph.org/about/governance-committees/code-of-ethics-and-professional-conduct/) | `no` | language too vague |
| [COS](https://www.cos.io) | [TOP Guidelines](https://www.cos.io/initiatives/top-guidelines) | `yes` | not reviewed as of 6.33 |
| `null` | [Broman & Woo 2018](https://doi.org/10.1080/00031305.2017.1375989) | `null` | re tabular data |
| `null` | [Mandakers & Dillon 2004](https://doi.org/10.3200/HMTS.37.1.34-38) | `yes` | re tabular data |
| `null` | [Robertson & Mullen 2021](https://doi.org/10.1093/jsh/shab015) | `null` | re work-log and text eg pre-print etc |
| `null` | [Hoekstra & Koolen 2019](https://doi-org.ezp-prod1.hul.harvard.edu/10.1080/01615440.2018.1484676) | `yes` | re work-log and text eg pre-print etc |
| [IDS at Maastricht Univ](https://www.maastrichtuniversity.nl/research/institute-data-science) | [IDS Best Practices](https://maastrichtu-ids.github.io/best-practices/) | `null` | nor reviewed as of 7.02 |
| `null` | [Panton Principles 2009](http://www.pantonprinciples.org) | `null` | not reviewed as ot 7.00 |
| [APS](https://www.psychologicalscience.org) | [*Psychological Science* Submission Guidelines](http://www.psychologicalscience.org/publications/psychological_science/ps-submissions#DISC) | `null` | not reviewed as of 9.58 |
| [GFISCO](https://www.go-fair.org/imprint/) | [FAIR Guiding Principles](https://www.go-fair.org/fair-principles/) | `null` | not reviewed as of 14.25 |

### TOP Guidelines by COS

latest version ie [v-1.0.1](https://osf.io/9f6gx/wiki/Guidelines/) with [summary table](https://www.cos.io/initiatives/top-guidelines) viewed on 16 aug 2022 7.11. compposed of eight standards, each divided into three levels, primarily intended for journals and funders.

| standard | level | adoption[^inc partial or modified adoption though in that case notice made in `note` column.] | note |
|:--|:--|:--|:--|
| no 1 | lvl iii | `yes` | `output` must appropriately cite[^ie must cite datasets and programme code used, where citation should (may) inc persistent identifier.] |
| no 2 | lvl ii[^lvl iii only possible via third-party action as requires publishing journal to verify replicability from `data` and `work-files`.] | `yes` | `data` and `work-files` must deposit in trusted repository[^where `work-files` must inc materials and methods (eg work log, work standards) and where `data` and `work-files` must be clearly and precisely documented and maximally available and where `work-files` must inc full account of how data collected, preprocessed, cleaned, and generated and where `work-files` must inc all materials and methods information necessary to independently replicate `work` or `output` and where parts of `data` or `work-files` which may not be shared (eg for legal or ethical reasons) must be noted in `data` or `work-files` inc explanation of restrictions and description of how to access restricted parts thereof.] |
| no 3 | lvl ii | `yes` | as in no 2 |
| no 4 | lvl ii | `yes` | as in no 2 |
| no 5 | lvl iii | `yes` | `text` must inc key design and log details of `work`[^ie `text` must report exclusions from `data` and data manipulations or measures used to produce `data` and further `text` should (may) explain how sample size was determined] |
| no 6 | lvl i[^lvl ii and lvl iii only possible via third-party action] | `no`[^as this project's work began in oct 2020, it isn't possible to pre-register it, though will be registered prior to pre-print.] | `work` must be pre-registered[^ie pre-registered in independent institutional registry.] |
| no 7 | lvl i[^lvl ii and lvl iii only possible via third-party action] | `yes` | data analysis plan ie steps to produce `data` must be pre-registered[^ie deposited in independent institutional registry. this is possible since version 1.4 data have not been cleaned nor analysed, so it's still possible to pre-register any plan for cleaning or processing of those data to produce `data`] |
| no 8 | `no` | `no` | not applicable |

### webarch by W3C

latest version [15 dec 2004](http://www.w3.org/TR/2004/REC-webarch-20041215/) reviewed 16 aug 2022 10.22. composed of vars principles, constraints and good practices defined in [sec 1.1.3](https://www.w3.org/TR/webarch/#app-principles) and listed prior to sec 1. vars irrelevant principles, constrains or good practices excluded from this section (for brevity, without comment or notice).

| practice | adoption[^inc partial or modified adoption though in that case notice made in `note` column.] | note |
|:--|:--|:--|
| sec 2.1 | `yes` | `output` should identify resources with URIs |
| sec 2.3.1 | `no` | `output` should not use URI aliasses |
| sec 2.4[^prior to sec 2.4.1] | `yes` | URIs in `output` should be use existing URI schemes |
| sec 3.5[^prior to sec 3.5.1] | `yes` | URI-identified resources in `output` should be provided[^eg URIs created for resourced in `output` should be made available] |
|  sec 3.5.1 | `yes` | as sec 3.5 adding *provided consistently and predictably* |

### dwbp by W3C

latest version [31 jan 2017](https://www.w3.org/TR/2017/REC-dwbp-20170131/) reviewed 16 aug 2022 10.43. composed of 35 best practices.

| practice | adoption[^inc partial or modified adoption though in that case notice made in `note` column.] | note |
|:--|:--|:--|
| bp 1 | `yes` | `data` should inc metadata |
| bp 2 | `yes` | as bp 1 adding *inc descriptive metadata* |
| bp 3 | `yes` | as bp 1 adding *inc structural metadata* |
| bp 4 | `yes` | `data` should inc licence |
| bp 5 | `yes` | `data` should inc provenance information |
| bp 6 | `yes` | `output` should inc info re quality of `data` |
| bp 7 | `yes` | `data` should inc version indicator |
| bp 8 | `no`[^as likely not possible to provide details re data versions prior to v-1.4.] | `output` should inc version history of `data` |
| bp 9 | `yes` | `data` should inc persistent URI for `data` as whole |
| bp 10 | `yes` | `data` should inc persistent URI for (select) parts or portions or components of or within `data` |
| bp 11 | `yes` | `output` should inc URIs for each version of dataset and a URI for all existing and future versions |
| bp 12 | `yes` | `data` should inc machine-readable formats |
| bp 13 | `yes` | `data` should use location-neutral data values[^or indicate location when neutral data values not possible] |
| bp 14 | `yes` | `data` should inc multiple copies in different formats |
| bp 15 | `yes` | `data` should reference standardised vocabularies |
| bp 16 | `yes` | as bp 15 adding *vocabularies to an appropriate degree of formality* |
| bp 17 | `no`[^not relevant as regards third-party] | should provide bulk download of `data` |
| bp 18 | `no`[^as depends on third-party] | should provide subsets of `data` if too large |
| bp 19 | `no`[^not relevant as regards third-party] | `data` host should use content negotiation |
| bp 20 | `no`[^not relevant to research] | `data` should be provided in real-time |
| bp 21 | `no`[^not relevant to research] | `data` should be up-to-date |
| bp 22 | `yes` | `output` should inc explanation of unavailable data values within `data` |
| bp 23 | `no`[^as depends on third-party] | `data` should be available via API |
| bp 24 | `no`[^as depends on third-party] | as bp 23 adding *standards-compliant API* |
| bp 25 | `no`[^as depends on third-party] | as bp 23 adding *well-documented API* |
| bp 26 | `no`[^as depends on third-party] | as bp 23 adding *persistently-available API* |
| bp 27 | `no`[^as depends on third-party] | should preserve URIs |
| bp 28 | `yes` | `data` should inc info re its coverage |
| bp 29 | `no`[^as depends on third-party] | should gather feedback |
| bp 30 | `no`[^as depends on third-party] | should make feedback available |
| bp 31 | `yes` | `output` should inc further data generated from `data` if informative or enriching[^likely not needed though] |
| bp 32 | `no`[^as depends on third-party] | should provide complementary presentations |
| bp 33 | `no`[^as depends on third-party] | should provide feedback |
| bp 34 | `yes` | `output` should comply with licences of materials employed during `work` |
| bp 35 | `yes` | `output` should cite data sources |

### ld-bp by W3C

latest version [9 jan 2014](http://www.w3.org/TR/ld-bp/) reviewed 16 aug 2022 11.32. composed of 10 steps primarily for publishers of open govt data.

| step | adoption[^inc partial or modified adoption though in that case notice made in `note` column.] | note |
|:--|:--|:--|
| no 1 | `no` | re stakeholders |
| no 2 | `no` | re other datasets |
| no 3 | `yes` | `data` should inc multiple copies in different *types* of data-representation[^eg copies in tabular representations like `csv` and in graphical representations like `rdf`] |
| no 4 | `yes` | `data` should be licensed |
| no 5 | `yes` | `data` should inc URIs[^and further these should use `http`sheme and should include at least one machine-readable representation of the URI-resource and newly-minted URIs should have well-considered naming ie construction] |
| no 6 | `yes` | `data` should use standard vocabularies |
| no 7 | `yes` | `data` should inc copy in graphical data formats |
| no 8 | `no` | re machine access |
| no 9 | `no` | re publication |
| no 10 | `no` | re post-publication |

### prov by W3C

latest version [8 dec 2010](http://www.w3.org/2005/Incubator/prov/XGR-prov-20101214/) reviewed 16 aug 2022 11.50. inc vars requirements in sec 4 (table in sec 4.1) though only sec 4.2 ie content requirements are relevant here (so all others excluded without comment for brevity).

| dimension | adoption[^inc partial or modified adoption though in that case notice made in `note` column.] | note |
|:--|:--|:--|
| object | `yes` | `output` should inc URI for `data` as whole |
| attribution | `yes` | `output` should identify sources ie materials used and entities involved in `work` |
| process | `yes` | `output` should inc log of `work`[^ie of steps taken to generate `data` inc computer porgrammes, physical acts, etc whether abstractly (inc only important parts) or minutely (inc fine-grained detail) enough to replicate.] |
| versioning | `no`[^as not possible for pre-version-1.4 data.] | `output` should inc good version history |
| justificaiton | `yes` | as process adding *and reasoning or justification for decisions taken during* `work`[^ie why and how decisions made during `work`] |
| entailment | `no`[^not relevant] | re reasoning |

### Frictionless Standards by OKF

latest versions [re package 2 may 2017](https://specs.frictionlessdata.io/data-package/) and [re resource 17 april 2018](https://specs.frictionlessdata.io/data-resource/) reviewed 16 aug 2022 12.17. composed of vars technical requirements mainly for metadata.

| re | standard | adoption[^inc partial or modified adoption though in that case notice made in `note` column.] | note |
|:--|:--|:--|:--|
| package | introduction | `yes` | `data` must inc metadata for itself as a whole |
| package | descriptor | `yes` | as introduction adding *inc list and locations of* `data` *components*[^vars technical requirements and recs ignored] |
| resource | introduction | `yes` | `data` must inc metadata for its components[^vers technical requirements and recs ignored]

### Open Definition by OKF

latest [version 2.1](https://opendefinition.org/od/2.1/en/) reviewed 16 aug 2022 12.34. mainly defines open data and licences though only sec 1 relevant here (so vars excluded wihtout comment)

| requirement | adoption[^inc partial or modified adoption though in that case notice made in `note` column.] | note |
|:--|:--|:--|
| sec 1.1 | `no`[^as may depend on third-party] | `data` must be provided under open licence |
| sec 1.2 | `yes` | `data` must be provided as a whole[^at no or nominal cost and should be online and must inc all info needed for user to complay with `data` licence eg names of all contributors] |
| sec 1.3 | `yes` | `data` must be machine-readable |
| sec 1.4 | `yes` | `data` must be in open format |

### Mandakers & Dillon 2004

reviewed 16 aug 2022 12.59. composed of vars recommendations ie rules spanning all data-creation process from data-entry to data-release.

| rule | adoption[^inc partial or modified adoption though in that case notice made in `note` column.] | note |
|:--|:--|:--|
| A1 | `yes` | `output` should inc info re purpose and content of `data` |
| A2 | `no`[^as info not available in version 1.4 so likely not possible to get for `data`.] | `output` should inc extensive info re primary sources used in `work` |
| A3 | `no`[^as info not available in version 1.4 so likely not possible to get for `data`.] | as A2 adding further content requirements |
| A4 | `null`[^as not relevant] | re samples |
| B1 | `yes` | `work-files` must be editable[^to allow correction of mistaken data values at any point during `work`] |
| B2 | `no` | standardisation and integration processes within `work` should be iterative |
| B3 | `no`[^as info not available in version 1.4 so likely not possible to get for `data`.] | `working-files` or `output` should inc rules used to integrate data from disparate sources during `work` |
| B4 | `no` | `data` should use standardised spelling |
| B5 | `no`[^as info not available in version 1.4 so likely not possible to get for `data`.] | manually corrected data values within `data` should be clearly documented within `data` |
| B6 | `no`[^as info not available in version 1.4 so likely not possible to get for `data`.] | generated or inferred or estimated data values within `data` should be flagged |
| B7 | `no`[^as may not be possible for source material] | material related to `output` or `process` should be preserved |
| B8 | `yes` | `working-files` should be backed-up |
| C1 | `no`[^as depends on third-party] | re publication |
| C2 | `no`[^as depends on third-party] | re releases |
| C3 | `no`[^as depends on third-party] | re public access |
| C4 | `no`[^as depends on third-party] | re distribution |
| C5 | `yes` | variables within `data` should be standardised |
| C6 | `yes` | data values missing from `data` should be explained |
| C7 | `yes` | geographic data values within `data` should be geo-referenced |
| C8 | `no`[^as likely not needed] | re reference |
| C9 | `yes` | `output` should inc easy user versions |
| C10 | `no`[^as regards technical specification] | re metadata format |
| C11 | `no`[^as depends on third-party] | re publication |
| C12 | `no`[^as likely not needed] | re `work` log |

### Hoekstra & Koolen 2019

reviewed 16 aug 2022 13.37. vars recommendations re selection, modelling, normalisation, classification, and linking of historical data using digital tools (per sec 1 para 4).

| rule | adoption[^inc partial or modified adoption though in that case notice made in `note` column.] | note |
|:--|:--|:--|
| sec 1 | `yes` | `output` should inc explicit info re `work`[^esp log of data handling within `work` inc data selection, modelling, normalisation, classification, and linking.] |

### IDS Best Practices by IDS at Maastricht Univ

reviewed 16 aug 2022 14.02. vars recommendations re project or re research. recommendations within [sec proj subsec FAIR](https://maastrichtu-ids.github.io/best-practices/docs/fair-data) not included. vars recommendations re research not included as not relevant.

| re | sec | adoption[^inc partial or modified adoption though in that case notice made in `note` column.] | note |
|:--|:--|:--|:--|
| project | admin | `null`[^likely not needed] | `work-files` with code should be deposited in repository |
| research | ontologies | `yes` | `data` should use existing ontologies |

### FAIR Guiding Principles by GFISCO





## process standards

## output standards