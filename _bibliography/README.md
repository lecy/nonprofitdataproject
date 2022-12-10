These files update the bibliography printed at the bottom of the pubs.md file via the includes function: 

```
{% include_relative _bibliography/bibliography.html %}
```
The R Markdown file **bibliography.rmd** generates the bibliography from the BibTex file called **references.bib**.

The output is specifically an **html_fragment** instead of **html_document** so that the output can be added directly to the pubs.md page through the includes function. 

In order to refresh the database you need to visit the scholar results page:

https://scholar.google.com/scholar?start=0&hl=en&as_sdt=20000005&sciodt=1,21&cites=1166513345463666613&scipsc=

And import all of the citations using Zotero and the Zotero Connect plugin: 

https://guides.library.illinoisstate.edu/zotero/adding/resultslist

Replace the **references.bib** file with the updated version and the re-run the **bibliography.rmd** file. 

Sync the updated **bibliography.html** to GitHub and the references will refresh. 
