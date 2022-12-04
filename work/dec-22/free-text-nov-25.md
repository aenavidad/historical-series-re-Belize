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
    - break at 18.05 on 26 nov,
    - continue at c 19.00 to c 19.15 on 26 nov,
    - break at 19.36 on 26 nov,
    - continue at 3.12 on 27 nov,
    - break at 4.38 on 27 nov,
    - continue at 5.01 on 27 nov,
    - done at 5.40 on 27 nov,
4. may now need specifics regarding versioning and provenance needed for version 1.4,
    - earliest metadata standards possibly related to [MARC](https://en.wikipedia.org/wiki/MARC_standards) dating to 1965-1968,
    - vars metadata stds listed in [wiki article](https://en.wikipedia.org/wiki/Metadata_standard), in [ands post](https://www.ands.org.au/working-with-data/data-management/data-versioning), in [klump](http://doi.org/10.5334/dsj-2021-012) ie [rda](https://www.rd-alliance.org/node/54345/outputs),
    - vars provenance stds listed in [w3c prov](https://www.w3.org/TR/prov-overview/), [jauer](https://doi.org/10.3233/shti200380), [eu scds](https://eudatasharing.eu/technical-aspects/data-provenance-part-1), [ardc](https://ardc.edu.au/resource/data-provenance/),
5. skim vars metadata and provenance stds located in step 4 and output in this step the relevant metadata, versioning, provenance values we need for datasets listed in output table 2,
    - may be standardised or not, in human-readable format, machine-readable format,
    - must record where data comes from (origin) and how it was processed (movement),
    - may record source data licenses, esp for data in v-1.4,
    - may want to retroactively record or estimate minimal fit-for-use requirements listed by [jauer](https://doi.org/10.3233/shti200380) sec. 3, at least for those datasets in output table 2 deemed to have contributed to v-1.4,
    - may want to retroactively record or estimate the six data versioning principles listed by [klump](http://doi.org/10.5334/dsj-2021-012) seventh sec., at least for those datasets in output table 2 deemed to have contributed to v-1.4,
6. now want to skim [[iCloud:hist pp notes.md]] for model articles accompanying historical dataset releases to see what exactly our pre-print for v-1.4 should look like,
    - inc abstract, conclusion, and so on, obviously, 
    - in introductory / contextual section inc some notes on historiography eg accuracy as regards facts, eg biases or trends, eg access or availability of primary sources, non-interpretative secondary sources, their accuracy, and so on,
    - in presentation / description section inc some notes on size, precision / accuracy / quality of data in v-1.4 (picture), inc notes on data collection and construction of data in v-1.4 (history),
    - in appendix section inc codebook ie descriptions of variables and values in v-1.4 (codebook), log of changes between versions, revisions, or releases (log).
7. now want to ouput text re notes on historiography in output text 1,
8. want to output tsv data re literature to be covered in pre-print section on notes on historiography, at 20.59 on 27 nov, with output to pp.numbers,
9. stop step 8 at 21.20 on 27 nov, as seems like this could go on forever despite its serving only an auxiliary function in the pre-print, so rather pivot towards what is meant to the bulk of the pre-pring, ie presentation / description section, for which we need more detail in the step 6, so we now continue step 6,
10. re building log, as per step 6, as of 3 dec 2022 at 16.54 est, we'd like to – 
    - know whether any files created between 22 oct 2020 to 14 nov 2020 contributed anythign to v 1.4 of data,
        - files created 22 oct 2020, 2 nov 2020, 11 nov 2020[^this one re human rights had event data but seems mostly crime related so likely not included in E nor E2 series of v-1.4], 13 nov 2020, 14 nov 2020[^this one re public finances had stat and finance data but was not included in Estimate nor Finances series of v-1.4] did not from cursory skim,
        - so none of these files contributed to v-1.4 of data as per cursory skims by 3 dec 2022 on 17.11 est,
    - get lost copy of red/HURR BZ V1 *.tsv,
        - found copy at /Users/angelnavidad/Library/Mobile Documents/com~apple~Numbers/Documents/HURR BZ V1.numbers,
        - confirmed creation date of November 25, 2020 at 16:25,
        - uploaded to pre-git-hist/files/red to match events.tsv address,
        - updated output table 2,
11. as of 3 dec 2022 at 19.19 est, confirm that red/HURR BZ V1 *.tsv is earliest ancestral dataset of v-1.4, so (i think) it counts as version 0.0.0,
12. before continuing step 6, decide to transfer all data from pp.numbers as git doesn't seem to track diffs here,[^or there do seem to be tools to do this, but looks like a steep learning curve to continue with tsv files instead]
    - output to tsv 1 (log), tsv 2 (literature),
13. at 3 dec 2022 at 19.35 est, continue step 6 by building log in table 3 (log),
14. xx

# output
## table 3 (log)

| semver[^per [klump](http://doi.org/10.5334/dsj-2021-012) and [semver](https://semver.org), esp their [faq](https://semver.org/#faq)] | start | end | paths[^excluding '*.tsv' suffix] | diffs[^to 1.4] | notes[^contents *excludes* empty records] |
|:--|:--|:--|:--|:--|
| 0.1.0 | 25 Nov 2020 | 9 Jan 2021 | red/HURR BZ V1 | `missing` | cf[^cf standardised code in `missing` / in 'Storms' + 'Storms < 4' + 'Storms-1' + 'Simulated' + 'Loss' + 'NMS' = 186 storm records for 1851-2018 fm `missing` / in 'Historical' + 'BLUE-1-1' + 'BLUE' + 'GDP-Pop' = 187 stats records for 1834-2020 fm `missing` / in 'NAVAL' = 71 stats records for 1765-1938 fm `missing` / in 'Rainfall' = 56 stats records for 1961-2016 fm `missing` / in 'Graph' = 26 stats records for `uncertain`-`uncertain` fm `missing` / in 'GFM' = 17 stats records for 2014-2020 fm `missing`] |
| 0.2.0 | 10 Jan 2021 | xx | tran/blue books data v1 + tran/hurr bz v2 + tran/Bz hurr hist 1 + tran/Hurricanes bz v2.1 | `missing` | cf[^in blue books 'Govt' + blue books 'Military' = 1 stats record for 1836 fm `missing` / in hurr bz 'Sheet 1' = 186 stats records for 1834-2019 fm `missing` / in Bz hurr 'Sheet 1' = 6 authorities records for 1638-2021 fm `uncertain` / in Bz hurr 'Original' + Bz hurr 'Gazette / Reports' + Bz hurr 'Simulated' + Bz hurr 'UN' = 190 stats records for 1829-2020 fm `missing` / in Hurricanes 'xx' = xx xx records for xx fm `missing`] |
| 0.x.y | xx | xx | xx | xx |
| 0.x.y | xx | xx | xx | xx |

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

## table 2[^includes all 'created file' events in pre-git-hist/events.tsv except those described as 're pre-existing data', those with 'wiki/*' paths, those after the first 'deposited dataset' action (on 4 November 2021 at 00:00), and letters (eg tran/foi act request lett copy.rtf), free text (eg red/hurr bz.rtf), non-free text (eg extracts as in red/1700s brneys.rtf, eg structured manuscript as in red/prelim rep bz 1.1.rtf or wiki/Chetumal_Province.xml), bibliography (eg tran/My EndNote Library.xml).]

| place | date | files | dates | topics | notes |
|:--|:--|:--|:--|:--|
| bz-cy | 22 October 2020 at 05:04 | tran/civil list v1 *.tsv | 2010s | crown offices, programmes, budget | no metadata nor sources[^likely [2014 staff list](https://web.archive.org/web/20221126112141/https://nbzlive.files.wordpress.com/2015/02/gob_staff_list-1.pdf) gotten via [blog](https://nbzlive.wordpress.com/2015/02/) and [fy2020-21 govt budget](https://web.archive.org/web/20221126114232/https://www.mof.gov.bz/uploads/files/pmokx5oc.pdf) gotten via [treasury](https://www.mof.gov.bz/downloads).] |
| bz-cy | 2 November 2020 at 20:16 | tran/bz gov ind *.tsv | 1990s-2010s | govt indicators | no metadata nor sources[^likely [world bank's wdi](https://datatopics.worldbank.org/world-development-indicators/).] |
| bz-cy | 11 November 2020 at 19:38 | red/gob rights practices *.tsv | 2000s-2020s | govt rights violations | no metadata nor sources[^likely [us state reports](https://www.state.gov/reports-bureau-of-democracy-human-rights-and-labor/country-reports-on-human-rights-practices/), [vanderbilt americasbarometer](https://www.vanderbilt.edu/lapop/about-americasbarometer.php), [wjp rule of law index](https://www.worldjusticeproject.org/rule-of-law-index/).] |
| bz-cy | 13 November 2020 at 22:47 | red/integrity 2016 *.tsv | 2010s | crown financial disclosures | no metadata nor sources[^likely from physical copy obtained from integrity commission likely during 2 oct 2022 - 13 nov 2022, inclusive, of recent certifications of statutory financial disclosures by crown service.] |
| bz-cy | 14 November 2020 at 20:53 | tran/debt belize 1 *.tsv[^renderred `tran/devt belize 1 *.tsv` in pre-git-hist/events.tsv, but this likely a mistake as no such file listed in pre-git-hist/files.tsv] | 1980s-2020s | sovereign debt, defaults, credit | no metadata some sources[^sources given per table but citation not standardised nor up to par.] |
| bz-cy | 25 November 2020 at 16:25 | red/HURR BZ V1 *.tsv[^not located in pre-git-hist/red/ on 26 nov 2022 at 13.41 est.] | 1760s-2010s | storm events, vars stats | no metadata some sources[^not standardised.] |
| bz-cy | 10 January 2021 at 03:21 | tran/blue books data v1 *.tsv | 1830s | crown budget, authorisations | no metadata nor sources[^likely blue books gotten via adam matthew] |
| bz-cy | 10 January 2021 at 17:28 	| tran/hurr bz v2 *.tsv | 1830s-2020s | hurricane, storm landings, official stats | no metadata nor sources[^likely noaa hurdat for hurricanes, as this series begin in 1850s, but sources uncertain for populaiton, spending, trade, gdp, though gdp data quoted as '2020 figs' while spending and trade data quoted as '2015 figs'.] |
| bz-cy | 10 January 2021 at 22:24	 | tran/Bz hurr hist 1 *.tsv | 1810s-2020s | crown authorisations, official stats, financial stats | no metadata nor sources[^possibly physical copies of the *Gazette*, likely gotten via heritage library, as one table labelled 'Gazette Reports', though one table labelled 'UN', though some official stats labelled '2020'.] |
| bz-cy | 12 January 2021 at 18:27 | tran/Hurricanes bz v2.1 *.tsv | 1790s-2020s | disaster events, official stats | some metadata[^not standardised] some sources[^not standardised, though possibly further skim contemporaneous tran/Hurricanes bz v3 writing *.tsv or red/hurr bz.rtf.] |
| bz-cy | 17 January 2021 at 22:10	 | tran/asdfsaf *.tsv | 1700s-2010s | distaster events | no metadata some sources[^though not standardised, and vars sources missing though may have been previously provided in prior files listed in this table.] |
| bz-cy | 18 January 2021 at 01:20	 | tran/dis bz v1.1 *.tsv | 1700s-2010s | disaster events | no metadata some sources[^these are sort-of standardised in tran/dis bz v1.1 D Sources-Table 1.tsv.] |
| bz-cy | 18 January 2021 at 21:39 | tran/econ bz 1700s *.tsv | 1690s | trade stats[^only one filled record available at tran/econ bz 1700s Sheet 1-Table 1.tsv] | no metadata nor sources[^tracking this sources seems really difficult as only one filled record is available] |
| bz-cy | 19 January 2021 at 22:46	 | re tran/early gdp dis bz v1 *.tsv[^given as re tran/early gdp dis bz v1 RAW *.tsv in pre-git-hist/events.tsv] | 1680s-1820s | trade stats | no metadata some sources[^though not standardised, likely from CO or CUST series via uk natl archives or adam matthews.] |
| bz-cy | 28 January 2021 at 17:38	 | red/pop bz v1.4 *.tsv | 1630s-2020s | disaster events, trade stats | no metadata[^though short summary of dataset size provided in red/pop bz v1.4 Meta-Table 1.tsv.] some sources[^not standardised] |
| bz-cy | 30 January 2021 at 20:41 | red/shipping bz v1.1 *.tsv | 1680s-1790s | trade stats | no metadata some sources[^not standardised] |
| bz-cy | 31 January 2021 at 20:29	 | red/trade raw bz v1.4 *.tsv | 1690s-1940s | trade stats, official stats | no metadata some sources[^some sort-of standardised in red/trade raw bz v1.4 Index of Abstracts-Table 1.tsv and red/trade raw bz v1.4 Index of Reports-Table 1.tsv.] |
| bz-cy | 3 February 2021 at 00:09	 | red/trade bz v1.3 *.tsv | `null`[^no filled records] | `null`[^no filled records] | `null`[^no filled records] |
| bz-cy | 3 February 2021 at 00:12	 | red/trade bz v1.5 *.tsv | 1670s-2010s | trade, official, financial stats | no metadata some sources[^not standardised] |
| bz-cy | 3 February 2021 at 05:56	 | tran/swi cust 3 cust 17 v1.1 copy of *.tsv | 1690s-1940s | trade, official, financial stats | no metadata some sources[^sort of standardised in tran/swi cust 3 cust 17 v1.1 copy of Index of Abstracts-Table 1.tsv and tran/swi cust 3 cust 17 v1.1 copy of Index of Reports-Table 1.tsv.] |
| bz-cy | 4 February 2021 at 16:29	 | tran/trade raw bz v1.4 WORKG COPY *.tsv | 1690s-1940s | trade, official, financial stats | no metadata some sources[^sort of standardised in tran/trade raw bz v1.4 WORKG COPY Index of Abstracts-Table 1.tsv and tran/trade raw bz v1.4 WORKG COPY Index of Reports-Table 1.tsv.] |
| bz-cy | 5 February 2021 at 16:10	 | red/trade bz v1.4 WORKING *.tsv | 1670s-2020s | trade, official, financial stats | no metadata some sources[^not standardised] |
| bz-cy | 5 February 2021 at 17:03	 | red/disasters non-hurr bz v1.5 REVIEW *.tsv | 1700s-2010s | disaster events | no metadata some sources[^not standardised] |
| bz-cy | 9 February 2021 at 20:54	 | red/trade bz v2.3 *.tsv | 1630s-2010s | trade, financial, official stats | no metadata some sources[^not standardised.] |
| bz-cy | 11 February 2021 at 00:25	 | red/disasters non-hurr bz v3.3 *.tsv | 1680s-2010s | disaster events | no metadata some sources[^sort of standardised in red/disasters non-hurr bz v3.3 Boston-Table 1.tsv, red/disasters non-hurr bz v3.3 Burney-Table 1.tsv, red/disasters non-hurr bz v3.3 European-Table 1.tsv, red/disasters non-hurr bz v3.3 NYC-Table 1.tsv, red/disasters non-hurr bz v3.3 Press < 1820-Table 1.tsv, red/disasters non-hurr bz v3.3 Spanish-Table 1.tsv.] |
| bz-cy | 13 February 2021 at 22:09	 | red/dis < 1820 non-hurr 3.5 *.tsv | 1650s-1810s | disaster events | no metadata nor sources[^though likely sources from prior non-hurricane disaster datasets in this table.] |
| bz-cy | 14 February 2021 at 21:16 | red/disasters non-hurr bz v3.3 SOURCE LINKS *.tsv | 1680s-2010s | disaster events | no metadata some sources[^sort of standardised in vars tables.] |
| bz-cy | 15 February 2021 at 12:58 | red/dis < 1820 non-hurr calcs 3.3 *.tsv | 1680s-1790s | disaster events | no metadata some sources[^not standardised.] |
| bz-cy | 17 February 2021 at 05:51 | red/dis < 1820 non-hurr 3.7 sources *.tsv | 1630s-2020s | bibliographic | no metadata some sources[^sort of standardised.] |
| bz-cy | 18 February 2021 at 12:11 | red/dis < 1820 non-hurr LOSS 3.5 *.tsv | 1700s-1810s | distaster events | no metadata nor sources[^likely given in related prior datasets in this table] |
| bz-cy | 19 February 2021 at 07:50 | red/dis < 1820 non-hurr 3.6 *.tsv | 1520s-1820s | disaster events | no metadata nor sources[^likely given in related prior datasets in this table.] |
| bz-cy | 19 February 2021 at 13:05 | red/disasters non-hurr bz v3.3 copy REVIEW *.tsv | 1680s-2010s | disaster events | no metadata some sources[^sort of standardised in vars tables.] |
| bz-cy | 23 February 2021 at 23:22 | red/dis non-hurr Eng settlement 3.7 *.tsv | 1630s-1820s | disaster events | no metadata nor sources[^though likely given in related prior datasets in this table.] |
| bz-cy | 27 February 2021 at 19:28 | red/dis non-hurr Eng settlement 3.7 asdfsd.tsv[^only red/dis non-hurr Eng settlement 3.7 asdfsd.tsv listed in pre-git-hist/files/red, so 'red/dis non-hurr Eng settlement 3.7 asdfsd *.tsv' taken as misprint] | 1630s-1820s | disaster events | no metadata nor sources[^though sources likely given in relted prior datasets in this table] |
| bz-cy | 20 March 2021 at 22:24 | red/repos bz 1.1 *.tsv | 2020s[^or 2010s] | bibliographic | no metadata some sources[^not standardised.] |
| bz-cy | 21 March 2021 at 11:34 | red/prelim rep bz 1.6 *.tsv | 1600s-2020s | vars events, vars stats | no metadata some sources[^not standardised] |
| bz-cy | 21 March 2021 at 14:00 | red/prelim rep bz 1.4 WORK *.tsv | 1630s-2020s | vars events, vars stats, bibliographic | no metadata some sources[^sort of standardised] |
| bz-cy | 21 March 2021 at 14:21 | red/prelim rep 1.4 events *.tsv | 1630s-1820s | vars events | no metadata some sources[^not standardised.] |
| bz-cy | 29 March 2021 at 21:22 | red/prelim rep bz events 1.6 *.tsv | 1600s-1670s | vars events, bibliographic | no metadata some sources[^sort of standardised.] |
| bz-cy | 8 April 2021 at 00:59 | red/prelim rep bz 1.6 ctrl *.tsv | 1630s-2020s | bibliographic | no metadata some sources[^sort of standardised] |
| bz-cy | 9 April 2021 at 16:35 | tran/prelim rep bz 1.7 *.tsv | 1540s-2020s | vars events, vars stats | no metadata some sources[^sort of standardised.] |
| bz-cy | 9 April 2021 at 16:35 | tran/prelim rep bz ctrl 1.7 *.tsv | 1600s-2020s | bibliographic | no metadata some sources[^sort of standardised.] |
| bz-cy | 28 April 2021 at 16:31 | red/prelim rep bz ctrl 1.8 *.tsv | 2020s[^or 2010s] | bibliographic | no metadata some sources[^sort of standardised] |
| bz-cy | 28 April 2021 at 23:50 | red/prelim rep bz 1.8 *.tsv | 1100s-1980s | vars events, vars stats | no metadata some sources[^not standardised] |
| bz-cy | 19 May 2021 at 21:57 | red/rep bz fin pub 1.0 *.tsv | 1100s-1980s | vars events, vars stats | no metadata some sources[^sort of standardised] |
| bz-cy | 20 May 2021 at 17:24 | tran/rep bz fin pub 1.0 *.tsv | 1100s-1980s | vars events, vars stats | no metadata some sources[^sort of standardised] |
| bz-cy | 20 May 2021 at 18:53 | red/white pp pre 1 *.tsv | 0000s-2020s | crown offices, events | no metadata nor sources[^seems difficult to track sources for this.] |
| bz-cy | 22 May 2021 at 10:54 | red/rep bz fin pub 1.3 *.tsv | 1500s-2020s | vars events, vars stats, bibliographic | no metadata some sources[^sort of standardised] |
| bz-cy | 21 June 2021 at 19:02	| red/sfadfasdfasfsdfsf *.tsv | 1760s-1980s | vars events | no metadata some sources[^not standardised] |
| bz-cy | 22 June 2021 at 00:24 | red/asdfasdfasdfasdf *.tsv | 1100s-2020s | vars events, vars stats, bibliographic | no metadata some sources[^sort of standardised] |
| bz-cy | 21 August 2021 at 02:44	| blue/bz crime rep pre 1.0 *.tsv | 2010s | crime events | no metadata some sources[^not standardised.] |
| bz-cy | 3 September 2021 at 13:23 | red/bz fb prelim 1.0 *.tsv | 2020s[^or 2010s] | crown offices | no metadata no sources[^seems difficult to locate sources for these] |
| bz-cy | 5 September 2021 at 12:55	| red/bz fb pre 1.1 *.tsv | 2020s[^or 2010s] | crown offices | no metadata some sources[^sort of standardised] |
| bz-cy | 7 September 2021 at 20:12	| red/rep bz fin pub 1.3_stable.tsv[^could only find red/rep bz fin pub 1.3_stable.tsv so 'red/rep bz fin pub 1.3_stable *.tsv' taken as misprint] | 0000s-2010s | vars events, vars stts, bibliogaphic | no metadata some sources[^sort of standardised] |
| bz-cy | 7 October 2021 at 21:51	| red/rep bz fin pub 1.4 *.tsv | 0000s-2020s | vars events, vars stats, bibliographic | some metadata[^sort of standardised] some sources[^sort of standardised] |
| bz-cy | 4 November 2021 at 00:00	| harv/ *.tsv | 0000s-2020s | vars events, vars stats, bibliographic | some metadata[^sort of standardised] some sources[^sort of standardised] |

## text 1

How to measure the selectivity and coverage of sources in historical literature? eg absence of newspapers, of Spanish primary records, etc.

As here were reviewing / commenting on literature, we'd like an exhaustive bibliography of said literature, possibly beginning with most recent? This would help demonstrate the rift between Spanish and non-Spanish sources. ie we'd like a graph of the literature.

## tsv 1 (log)

```
contains tsv data for pre-print for version 1.4 of data. document created on 27 nov 2022 at 20.54 est in east boston, ma

id	cf	date	path	labelled_version	semantic_version	non-trivial_diffs_vs_id	non-trivial_diffs_intro	non-trivial_diffs_sources	non-trivial_diffs_events	non-trivial_diffs_cartas	non-trivial_diffs_weather	non-trivial_diffs_currency	non-trivial_diffs_finances	non-trivial_diffs_trade	non-trivial_diffs_towns	non-trivial_diffs_estimates	non-trivial_diffs_note	deposit_0_uri	deposit_0_date	deposit_0_licence	deposit_0_note	deposit_1_uri	deposit_1_date	deposit_1_licence	deposit_1_note	deposit_2_uri	deposit_2_date	deposit_2_licence	deposit_2_note	deposit_3_uri	deposit_3_date	deposit_3_licence	deposit_3_note	deposit_4_uri	deposit_4_date	deposit_4_licence	deposit_4_note		
0	work/dec-22/free-text-nov-25.md sec output table 2 last row	4 Nov 2021	harv/*.tsv	1.4	0.y.z	1	none	none	none	none	none	`null`	`null`	`null`	`null`	`null`	"vs id=1, assume none value for `null` values as seems correct as of 28 nov 2022 at 3.25 est"	https://github.com/aenavidad/pre-git-hist	11 Aug 2022	none	"repository created 11 Aug 2022, files last added to repository 21 Aug 2022, made public on `null`, remains public as of 27 Nov 2022"	https://dataverse.harvard.edu/privateurl.xhtml?token=135a1006-cd54-4d9e-ba7b-d961b93f1bc4	4 Nov 2021	CC0 1.0	non-public draft as of 27 Nov 2022	https://github.com/aenavidad/historical-series-re-Belize/tree/main/v-1.4	10 Aug 2022	CC0 1.0	"repository created 13 July 2022, made public on `null`, remains public as of 27 Nov 2022"	https://osf.io/rm7be/	16 Aug 2022	CC BY 4.0	"made public 16 Aug 2022, registered 16 Aug 2022 at https://osf.io/5byhm, remains public as of 27 Nov 2022"	https://osf.io/7ujq5/	`null`	CC BY 4.0	non-public draft as of 27 Nov 2022		
1	work/dec-22/free-text-nov-25.md sec output table 2 second-to-last row	7 Oct 2021	red/rep bz fin pub 1.4 *.tsv	none	0.y.z	2	`null`	"3 variables added [NAME 0, FAID, and one other], 278 records added, 333 ID values added [S 964 to S 1628, exc addition of S 402 value], vars other changes"	`null`	`null`	none	`null`	`null`	`null`	`null`	`null`	"vs id=2, assume vars value for `null` values as seems correct as of 28 nov 2022 at 3.37 est"	https://github.com/aenavidad/pre-git-hist	11 Aug 2022	none	"repository created 11 Aug 2022, files last added to repository 21 Aug 2022, made public on `null`, remains public as of 27 Nov 2022"	`null`	`null`	`null`	`null`	`null`	`null`	`null`	`null`	`null`	`null`	`null`	`null`	`null`	`null`	`null`	`null`		
2	work/dec-22/free-text-nov-25.md sec output table 2 third-to-last row	7 Sep 2021	red/rep bz fin pub 1.3_stable.tsv	none	0.y-1.z												`null`	https://github.com/aenavidad/pre-git-hist	11 Aug 2022	none	"repository created 11 Aug 2022, files last added to repository 21 Aug 2022, made public on `null`, remains public as of 27 Nov 2022"	`null`	`null`	`null`	`null`	`null`	`null`	`null`	`null`	`null`	`null`	`null`	`null`	`null`	`null`	`null`	`null`		

```

## tsv 2 (literature)

```
contains tsv data for pre-print for version 1.4 of data. document created on 27 nov 2022 at 20.54 est in east boston, ma / notes Higman = https://doi.org/10.1007/978-1-349-73776-5	

	source	type	name			
	Higman p 682	book	Humphrey's 1960 *Diplomatic History*			
	Higman p 682	book	Henderson's 1809 `null`			
	Higman p 682	book	Crowe's 1850 `null`			
	Higman p 682	book	Gibbs's 1883 `null`			
	Higman p 682	book	Burdon's 1931-5 *Archives*			
	Higman p 682	book	Caiger's 1951 `null`			
	Higman p 682	book	Waddell's 1967 `null`			
	Higman p 682	book	Clegern's 1967 `null`			
	Higman p 683	book	Dobson's 1973 *History*			
	Higman p 683	journal	*J of Belizean Affairs*			
	Higman p 683	journal	*Belizean Studies*			
	Higman p 683	journal	*BELCAST J of Belizean Affairs*			
	Higman p 683	author	Belizean Institute for Social and Research Activities			
	Higman p 683	book	Bolland's 1977 `null`			
	Higman p 683	author	Cedric Grant			
	Higman p 683	author	Assad Shoman			
	Higman p 684	journal	*Readings in Belizean History*			
	Higman p 685	author	Soc for the Promotion of Education and Research			
	Higman p 685	author	Herman Byrd			
	Higman p 685	author	Lita Hunter-Krohn			
	Higman p 685	author	James Murphy			
	Higman p 685	author	Mateo Ayuso			
	Higman p 685	author	Joseph Palacio			
	Higman p 685	author	Said Musa			
	Higman p 685	author	Historical Society [Belize]			
	Higman p 685	author	Emory King			

```