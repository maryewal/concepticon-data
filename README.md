# concepticon-data

## Structure of current data

- **conceptlists/** folder contains conceptlists with links to OMEGAWIKI and concepticon.tsv (all in column "OMEGAWIKI"), the lists are named after the first person who proposed them, the year of the reference publication in which we extracted them, and the number of concepts. All these three parts of information are separated by a dash. Furthermore, in cases where two lists would have an identical name, we add alphabetical letters to the lists to distinguish them. Files need to have the columns "GLOSS" (some still have "ENGLISH" instead, but this needs to be changed) and "OMEGAWIKI", additionally, most (if not all files) have a "NUMBER" field indicating the number in the reference, which is also important for ordering the entries as given in the original source. Additional columns are more or less free to the user, but we tried to be consistent.
- **references/references.bib** the bibtex file showing links to all concept lists (bibtex-key identical to the name of the conceptlist file, without file-ending. File further contains links to the references  in which the conceptlists were published (references stored in the "crossref" field). 
- **sources/** contains pdf-files of each conceptlist (only the list-parts, not the full publications for copyright reasons), naming is the same as for the conceptlists, but with the ending ".pdf" instead of ".tsv".
- **concepticon.tsv** basically also a conceptlist, but we use it as the basic reference which contains glosses, links to WOLD (if they are given), links to OMEGAWIKI, and some additional information.