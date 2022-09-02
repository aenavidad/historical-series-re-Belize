# detour-at-1-54

## abstract

this file contains output from step 52 of [[ia-extractions]][^file written 23 aug 2022 1.56 in Boston MA]

## style

## log

1. start at 1.57
2. skim [RFC 6838](https://www.rfc-editor.org/rfc/rfc6838) for style advice,
3. note [RFC 5234](https://www.rfc-editor.org/rfc/rfc5234) specifies ABNF,
4. note [Terminal User Guide](https://support.apple.com/en-gb/guide/terminal/welcome/2.11/mac/11.6) for [macOS Terminal](https://en.wikipedia.org/wiki/Terminal_(macOS)),
5. skim wiki referenced in step 4,
    6. begin step 5 notes,
    7. [type](https://en.wikipedia.org/wiki/Software_categories#Categorization_approaches) = [terminal emulator](https://en.wikipedia.org/wiki/Terminal_emulator),
    8. default shell = [zsh](https://en.wikipedia.org/wiki/Z_shell)
    9. environment variables in use retrievable via `% env` command per relevant sec in [Guide](https://support.apple.com/en-gb/guide/terminal/apd382cc5fa-4f58-4449-b20a-41c53c006f8f/2.11/mac/11.0),
    10. either default or currently-in-use programme settings retrievable via `% defaults read` command ver [StackExchange](https://apple.stackexchange.com/questions/195244/concise-compact-list-of-all-defaults-currently-configured-and-their-values),
    11. Terminal's default shell ie zsh has options to log activity (assume this means input and output) and to configure vars options etc per [wiki](https://en.wikipedia.org/wiki/Comparison_of_command_shells),
    7. end step 5 notes,
6. skim Guide referenced in step 4 at 4.30,
    7. begin step 6 notes,
    8. zsh manual available in [Terminal](x-man-page://zsh),
    9. shell script primer in [relevant sec](https://support.apple.com/en-gb/guide/terminal/apd53500956-7c5b-496b-a362-2845f2aab4bc/2.11/mac/11.0) of Guide,
    10. shell scripts may be managed in Terminal with [launchd](https://support.apple.com/en-gb/guide/terminal/apdc6c1077b-5d5d-4d35-9c19-60f2397b2369/2.11/mac/11.0) via `% launchctl` command,
    11. may log Terminal session (or vars sessions?) via `% script` command,[^eg per [this haphazard blogpost](https://ostechnix.com/record-everything-terminal/)]
    8. end step 6 notes,
7. note [Script Editor User Guide](https://support.apple.com/en-gb/guide/script-editor/welcome/2.11/mac/11.6) for [Script Editor](https://en.wikipedia.org/wiki/AppleScript_Editor) ie the native editor for the AppleScript proprietary [scripting language](https://en.wikipedia.org/wiki/Scripting_language),
8. skim zsh files referenced in step 5 notes,
9. paused on 23 aug 2022 4.11,
10. continued on 24 aug 2022 15.00,
11. recovered files skimmed after step 9 pause but prior to step 10 continuation,
    12. begin step 11 list,
    13. re [pseudocode](https://en.wikipedia.org/wiki/Pseudocode),
    14. re [algorithms](https://www.khanacademy.org/computing/ap-computer-science-principles/algorithms-101/building-algorithms/a/expressing-an-algorithm),
    15. re [social procedures as algorithms](https://plato.stanford.edu/entries/social-procedures/),
    16. re [algorithms](https://en.wikipedia.org/wiki/Algorithm_characterizations),
    17. re [Turing machines](https://en.wikipedia.org/wiki/Turing_machine),
    18. re [Turing completeness](https://en.wikipedia.org/wiki/Turing_completeness),
    19. a [list of programming languages by characterisation](https://en.wikipedia.org/wiki/List_of_programming_languages_by_type)
    13. end step 11 list,
12. pause at 15.06,
13. continue at 15.26,
14. note W3C [Guide](https://www.w3.org/Guide/) for specification development,
    15. begin step 14 notes,
    16. use [CommonMark](https://commonmark.org) for markdown as per editing tool [Bikeshed](https://tabatkins.github.io/bikeshed/),
    17. vars practices per [QA Guide](https://www.w3.org/TR/qaframe-spec/) and [Manual of Style](https://www.w3.org/Guide/manual-of-style/) and [QA Primer](https://www.w3.org/QA/WG/qaframe-primer),
    18. use of [DTD](https://en.wikipedia.org/wiki/Document_type_definition),[^where, DTD defines the structure and the legal elements and attributes of an markup lang document]
    16. end step 14 notes,
15. null