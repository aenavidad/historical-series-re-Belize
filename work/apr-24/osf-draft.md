# apr-24 > osf-draft

## abstract

this file written 10 oct 2023 18.28 belmopan as part of [[work/oct-23/log.md]] no 15. contains free-text for an `osf` registration.[^for `osf` project [7UJQ5](https://osf.io/7ujq5/) with one prior registration [5BYHM](https://doi.org/10.17605/OSF.IO/5BYHM) *once* said project has been updated as per (i) to (vi) for (i) a data-component 'version 1.5' has been added to the project to hold the expected data output; (ii) two sub-project components 'pre-git work' and 'post-git work' have been added to hold all working files; (iii) all `pre-git-hist` files have been copied into component 'pre-git work'; (iv) all `historical-series-re-Belize` files have been copied into component 'post-git work'; (v) github copy of `pre-git-hist` has been linked to 'pre-git work'; (vi) github copy of `historical-series-re-Belize` has been linked to 'post-git work']

## free-form reasoning

we'd like to know
1. sx of 1.0.0-alpha
2. standards to be met by 1.0.0-alpha
3. standards for and steps in `pre-git-hist` to 1.0.0-alpha process

now, will we update or withdraw the 16 aug 2022 registration https://doi.org/10.17605/OSF.IO/5BYHM
- this registraiton is for 1.5 ie 1.0.0 ie human-and-machine readable dataset
- withdrawal deletes content, so we may not really wanna do that
- so we must update the current registration or create a completely new one
- updates seem to be for extenuating circumstances only, but that doesn't seem to apply in this case,
- so we ought to create a new registration for the same project
- suitability of multiple registrations for the same project confirmed in https://nyu-dataservices.gitlab.io/rdm-instruction/project-management-with-the-osf.html
- see how-to at https://help.osf.io/article/345-create-registrations
- seems we'll want an open-ended registration type

to assign correct licence, we need a list of publicly shared copies of data and working files and their licences[^note any deposit of `v-1.4` would state in the introductory `tsv` file that the dataset was licensed CC BY NC 4.0. this file *might not* be the only one to declare a licence.]
- `osf` project [7UJQ5](https://osf.io/7ujq5/) deposited 16 Aug 2022, made fully public 11 Oct 2023 with CC BY 4.0, but prior made partially public 16 Aug 2022 with CC BY 4.0,[^project component [`version 1.4`](https://osf.io/rm7be/) was the only project portion to be made public prior to 11 Oct 2023]
- `osf` registration [5BYHM](https://osf.io/5byhm) registered 16 Aug 2022, made public 16 Aug 2022 with CC BY 4.0,[^`osf` registrations include a 'frozen-in-time' snapshot ie archive of their associated project and its files]
- `harvard` dataverse [hsbz](https://dataverse.harvard.edu/dataverse/hsbz) deposited 4 Nov 2021 but not yet made public as of 11 Oct 2023,[^however, draft copy of a portion of the dataverse [v 1.4](https://dataverse.harvard.edu/privateurl.xhtml?token=135a1006-cd54-4d9e-ba7b-d961b93f1bc4) *was* privately shared via email etc to select persons and thereby disseminated as draft with licence CC0 1.0. The hyperlink to access the dataverse portion v 1.4 was furthermore included in files made public via `osf` and `github`. further portions of the dataverse [foundation 1.2](https://dataverse.harvard.edu/privateurl.xhtml?token=64fefd3c-0916-4658-821b-4268f2125b32) and [1638 1.5](https://dataverse.harvard.edu/privateurl.xhtml?token=85f85706-c4f7-4105-8a64-9c988cf1a1c3) *may* have likewise been so disseminated as drafts with licences CC0 1.0 and CC0 1.0, but can recall no instance of this.]
- `github` repository [pre-git-hist](https://github.com/aenavidad/pre-git-hist) initialised 11 Aug 2022, made public `null` with no licence (likely), has no licence as of 11 Oct 2023,[^date made public not available in `work/dec-22/pp.numbers` sheet 'log', but per the same was public by 27 Nov 2022. date made public does not seem recoverable from `github` as of 11 oct 2023 14.26]
- `github` repository [historical-series-re-Belize](https://github.com/aenavidad/historical-series-re-Belize) initialised 13 Jul 2022, made public `null` with no licence (likely), has no licence as of 11 Oct 2023,[^date made public not available in `work/dec-22/pp.numbers` sheet 'log', but per the same was public by 27 Nov 2022. date made public does not seem recoverable from `github` as of 11 oct 2023 14.26. further note a portion of this repo [v-1.4](https://github.com/aenavidad/historical-series-re-Belize/tree/main/v-1.4) was imported from `harvard` with the attendant licence CC0 1.0 attached]

seems we ought to issue all code under some MIT licence, but there is no code so this is moot. then we ought to issue all other content under CC BY 4.0 *or* CC BY SA 4.0, but we ought to note exceptions as follows,
- non-copyrightable work may be present eg factual data, measurements, the like
- non-original non-copyright work may be present eg old manuscript extracts, quotes of old newspaper articles, etc
- non-original copyright work may be present eg quotes of recent journal articles, of recent books, etc

furthermore, the copyright notice should be fixed, as it seems copyright date should be year of first publication, rather than year of creation, but vars distinct copyright notices may have been included in working files or data made public or otherwise circulated.[^*publication* does not seem to encompass limited circulation of work to select persons, rather seems to require making work public ie unlimited distribution to all and sundry, regardless of work curation status (it seems).] so the notice ought to be as follows,
- 'Copyright (c) 2022 AE Navidad' for version 1.4 dataset and working files up to 31 Dec 2022,[^not '(c) 2020' nor '(c) 2021' as no dataset nor working file was available to public at large, rather only available to limited set of persons]
- 'Copyright (c) 2023 AE Navidad' for version 1.5 dataset and working files up to 31 Dec 2023,[^assuming version 1.5 dataset completed and made available to public in 2023]

for filling in s 4 below (osf registration supplement), we first refer to supplementary files in the 16 aug 2022 registration. they are meant to have 'standards and work outline' for version 1.5 of data, including 'likely only [...] data cleaning, checking, and standardising for output to human-readable and machine-readable formats'.
- `process-0.md` and `standards.md` are meant to include standards
- `standards.md` includes standards considered for adoption, but does not *actually* state which standards were or were not adopted,
- `process-0.md` includes standards adopted, and gives a birds eye view of work process, but no actual work details,
- `output.md` includes structure and content of output, but in a more freeform text,
- `algorithmic.md` includes more detailed work process.

## osf registration summary

### What is contained in this registration?
This registration contains three components (`version 1.5`, `pre-git work`, `post-git work`) and one supplementary file (`osf-reg.md`).[^And this summary itself and associated metadata, of course.]

#### The components
`version 1.5` is an empty component which is set to house version 1.5 of the upcoming data series ie datasets. 

`pre-git work` is a non-empty component which contains a current copy of the git repository [pre-git-hist](https://github.com/aenavidad/pre-git-hist), and so contains working files created or modified prior to the adoption of git, including version 1.4 of data. 

`post-git work` is a non-empty component which contains a current copy of the git repository [historical-series-re-Belize](https://github.com/aenavidad/historical-series-re-Belize), and so contains working files created or modified after the adoption of git, including version 1.4 of data.

#### The supplementary file
`osf-reg.md` is a non-empty supplementary file which which details the expected structure and contents of version 1.5, standards for it, and work process to obtain it.

### How does this registration differ from prior ones?
xx

### Does this project contain documents for a preregistration?
No.[^Preregistration is not possible as data have already been collected.]

### AsPredicted questions
#### Have any data been collected for this study already?
xx

#### What's the main question being asked or hypothesis being tested in this study?
xx

#### Describe the key dependent variable(s) specifying how they will be measured.
xx

#### How many and which conditions will participants be assigned to?
xx

#### Specify exactly which analyses you will conduct to examine the main question/hypothesis.
xx

#### Describe exactly how outliers will be defined and handled, and your precise rule(s) for excluding observations.
xx

#### How many observations will be collected or what will determine sample size? No need to justify decision, but be precise about exactly how the number will be determined.
xx

#### Anything else you would like to pre-register?  (e.g., secondary analyses, variables collected for exploratory purposes, unusual analyses planned?)
xx

## osf registration supplement
routed to [[work/oct-23/osf-reg.md]] on 11 oct 2023 18.11 bmp.

