The translations for draw.io are generated from [this spreadsheet](https://docs.google.com/spreadsheets/d/1FoYdyEraEQuWofzbYCDPKN7EdKgS_2ZrsDrOA8scgwQ). If you'd like to make edits, email support@draw.io asking for write access.

The process for updating, which live under [/war/resources](https://github.com/jgraph/draw.io/tree/master/war/resources) is:

- In Google Sheets invoke File->Download As->.tsv (tab separated)
- Put the .tsv file in the resources directory and run the [properties generation code](https://github.com/jgraph/draw.io/blob/master/etc/build/PropGen.java), selecting that file as the source.
- Remember to delete the .tsv afterwards, that doesn't live in source control.