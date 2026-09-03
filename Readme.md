# Tool libraries for CNC mills - use with tooldb-converter

Library definitions for different tool manufacturers. For the meta format information and usage see 
https://github.com/codeblame-git/tooldb-converter.

# Folder structure

Each manufacturer gets its own folder.
Generate both file formats per catalog. You can use the meta convert functions of the tooldb-converter to convert 
between json and csv or dump both during sw<->hsm conversion.

```
\<manufacturer>
    |-<name of library/catalog>.json
    |-<name of library/catalog>.csv # generate both variants of meta files (use --convert-meta)
    |-output/ # for artifacts, ignored by gitignore. Generated artifacts (hsmlib, csv) should be packaged in releases
```