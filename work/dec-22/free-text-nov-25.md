# abstract

free text for pre-print for version 1.4 of historical series. begun on 25 nov 2022 at 23.58 est in east boston, ma.

# log

1. we want to know what pre-1.4 versions of the data looked like, and ideally know a bit more about where those came from, and when,
    - so we skim pre-git-hist directory,
    - output to table 1,
    - stop output to table 1, as file-by-file listing seems to be taking to long, instead move to step 3,
2. detour at 26 nov 2022 on 0.13 to skim stuff on semantic versioning as may be helpful here,
    - *semver* seems geared towards software, so we need something geared towards data,
    - skim [klump](http://doi.org/10.5334/dsj-2021-012) for data-specific semantic versioning,
    - klump confirms no consensus best practice for versioning of data cf intro sec.,
    - klump = most recent [rda](https://www.rd-alliance.org/node/54345/outputs) output per intro sec.,
    - klump rules in *six data versioning principles* sec.,
    - stop detour on 1.46 to continue step 1,
3. skim pre-git-hist/events.tsv to output table 2,
    - break at 2.24 on 26 nov,
    - return at 2.53 on 26 nov,
    - breat at 3.12 on 26 nov,
    - return at 6.15 on 26 nov,
    - break at 7.16 on 26 nov,
    - continue at 13.22 on 26 nov,
4. xxx

# output
## table 1

| place | action | date | description | notes |
|:--|:--|:--|:--|:--|
| bz-cy | sent email | 2 October 2020 at 16:19 | re subj Questions re. World Bank Governance Indicators to fh*@gmail.com | earliest record in pre-git-hist/events.tsv |
| bz-cy | created file | 22 October 2020 at 05:04 | re tran/civil list v1 *.tsv | earliest record of file creation in pre-git-hist/events.tsv |
| bz-cy | created file | 2 November 2020 at 20:16 | re tran/bz gov ind *.tsv | addition |
| bz-cy | created file | 11 November 2020 at 19:38 | re red/gob rights practices *.tsv | addition |
| bz-cy | created file | 13 November 2020 at 22:47 | re red/integrity 2016 *.tsv | `uncertain` |
| bz-cy	| created file	 | 14 November 2020 at 20:53 | re tran/devt belize 1 *.tsv | `uncertain` |
| bz-cy	| created file | 25 November 2020 at 16:25 | re red/HURR BZ V1 *.tsv | `uncertain` |
| bz-cy	| created file	 | 10 January 2021 at 03:21 |	re tran/blue books data v1 *.tsv | `uncertain` |
| bz-cy	| created file | 10 January 2021 at 17:28 | re tran/hurr bz v2 *.tsv | `uncertain` |

## table 2

| place | date | files | dates | topics | notes |
|:--|:--|:--|:--|:--|
| bz-cy | 22 October 2020 at 05:04 | tran/civil list v1 *.tsv | 2010s | crown offices, programmes, budget | no metadata nor sources[^likely [2014 staff list](https://web.archive.org/web/20221126112141/https://nbzlive.files.wordpress.com/2015/02/gob_staff_list-1.pdf) gotten via [blog](https://nbzlive.wordpress.com/2015/02/) and [fy2020-21 govt budget](https://web.archive.org/web/20221126114232/https://www.mof.gov.bz/uploads/files/pmokx5oc.pdf) gotten via [treasury](https://www.mof.gov.bz/downloads).] |
| bz-cy | 2 November 2020 at 20:16 | tran/bz gov ind *.tsv | 1990s-2010s | govt indicators | no metadata nor sources[^likely [world bank's wdi](https://datatopics.worldbank.org/world-development-indicators/).] |
| bz-cy | 11 November 2020 at 19:38 | red/gob rights practices *.tsv | 2000s-2020s | govt rights violations | no metadata nor sources[^likely [us state reports](https://www.state.gov/reports-bureau-of-democracy-human-rights-and-labor/country-reports-on-human-rights-practices/), [vanderbilt americasbarometer](https://www.vanderbilt.edu/lapop/about-americasbarometer.php), [wjp rule of law index](https://www.worldjusticeproject.org/rule-of-law-index/).] |
| bz-cy | 13 November 2020 at 22:47 | red/integrity 2016 *.tsv | 2010s | crown financial disclosures | no metadata nor sources[^likely from physical copy obtained from integrity commission likely during 2 oct 2022 - 13 nov 2022, inclusive, of recent certifications of statutory financial disclosures by crown service.] |
| bz-cy | 14 November 2020 at 20:53 | tran/debt belize 1 *.tsv[^renderred `tran/devt belize 1 *.tsv` in pre-git-hist/events.tsv, but this likely a mistake as no such file listed in pre-git-hist/files.tsv] | 1980s-2020s | sovereign debt, defaults, credit | no metadata some sources[^sources given per table but citation not standardised nor up to par.] |
| bz-cy | 25 November 2020 at 16:25 | red/HURR BZ V1 *.tsv[^not located in pre-git-hist/red/ on 26 nov 2022 at 13.41 est.] | `uncertain` | `uncertain` | `uncertain` |
| bz-cy | 10 January 2021 at 03:21 | tran/blue books data v1 *.tsv | 1830s | crown budget, authorisations | no metadata nor sources[^likely blue books gotten via adam matthew] |
| bz-cy | 10 January 2021 at 17:28 	| tran/hurr bz v2 *.tsv | 1830s-2020s | hurricane, storm landings, official stats | no metadata nor sources[^likely noaa hurdat for hurricanes, as this series begin in 1850s, but sources uncertain for populaiton, spending, trade, gdp, though gdp data quoted as '2020 figs' while spending and trade data quoted as '2015 figs'.] |
| bz-cy | 10 January 2021 at 22:24	 | tran/Bz hurr hist 1 *.tsv | 1810s-2020s | crown authorisations, official stats, financial stats | no metadata nor sources[^possibly physical copies of the *Gazette*, likely gotten via heritage library, as one table labelled 'Gazette Reports', though one table labelled 'UN', though some official stats labelled '2020'.] |
| bz-cy | 12 January 2021 at 18:27 | tran/Hurricanes bz v2.1 *.tsv | 1790s-2020s | disaster events, official stats | some metadata[^not standardised] some sources[^not standardised, though possibly further skim contemporaneous tran/Hurricanes bz v3 writing *.tsv or red/hurr bz.rtf.] |
| bz-cy | 17 January 2021 at 22:10	 | tran/asdfsaf *.tsv | 1700s-2010s | distaster events | no metadata some sources[^though not standardised, and vars sources missing though may have been previously provided in prior files listed in this table.] |
| bz-cy | 18 January 2021 at 01:20	 | tran/dis bz v1.1 *.tsv | 1700s-2010s | disaster events | no metadata some sources[^these are sort-of standardised in tran/dis bz v1.1 D Sources-Table 1.tsv.] |
| bz-cy | 18 January 2021 at 21:39 | tran/econ bz 1700s *.tsv | 1690s | trade stats[^only one filled record available at tran/econ bz 1700s Sheet 1-Table 1.tsv] | no metadata nor sources[^tracking this sources seems really difficult as only one filled record is available] |
| bz-cy | 19 January 2021 at 22:46	 | re tran/early gdp dis bz v1 *.tsv[^given as re tran/early gdp dis bz v1 RAW *.tsv in pre-git-hist/events.tsv] | 1680s-1820s | trade stats | no metadata some sources[^though not standardised, likely from CO or CUST series via uk natl archives or adam matthews.] |
| bz-cy | 28 January 2021 at 17:38	 | red/pop bz v1.4 *.tsv | cover | desc | xx |
| bz-cy | date	 | path | cover | desc | xx |
| bz-cy | date	 | path | cover | desc | xx |
| bz-cy | date	 | path | cover | desc | xx |