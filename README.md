# Notes on Citation Styles (.csl)

## Citation Style Files

Sources of style files include:
- https://github.com/citation-style-language/styles
 - Download .csl files as raw (as explained here: - http://stackoverflow.com/questions/19949540/error-running-filter-pandoc-citeproc-when-specifying-csl-style?rq=1)
- https://www.zotero.org/styles

## Journal Abbreviations

Sources of journal abbreviations:
- https://github.com/citation-style-language/abbreviations/tree/master/ncbi
- https://github.com/dhruvbansal/bibtex_abbreviations

To include journal abbreviations in a .bib file, create strings containing the journal abbreviations following the instructions here: http://latex-community.org/forum/viewtopic.php?f=5&t=690

1. In your .bib file, replace the journal title with a string

        @article{louthan2013climatic,
        	Author = {Louthan, Allison M and Doak, Daniel F and Goheen, Jacob R and Palmer, Todd M and Pringle, Robert M},
        	Journal = JEcol,
        	Number = {4},
        	Pages = {1074--1083},
        	Publisher = {Wiley Online Library},
        	Title = {Climatic stress mediates the impacts of herbivory on plant population structure and components of individual fitness},
        	Volume = {101},
        	Year = {2013}}

2. Create a "short titles" .bib file with information linking the journal title string to its abbreviation

        @string{JEcol="J. Ecol."}

3. Create a "long titles" .bib file with information linking the journal title string to its full title

        @string{JEcol="Journal of Ecology"}


4. Note: To get this to work with R markdown, I pasted the strings to the beginning of my .bib file rather than include as a second file.


