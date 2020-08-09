This is a minimal example of how to use academic references in a webpage. To use:
* Copy the "bib" script (footer of main.html) to your page's footer.
* Copy the script tags (JQuery, Citation.js, JQuery Comments) in the header to your page's header.

**Workflow**: Say you want to add citations to the webpage while writing.
* Search your favourite website (Google Scholar, Semantic Scholar etc.) and get the BibTeX entry of the publication. Most researchers know maintaining a BibTeX file is usual practice if you are working with LaTeX.
* Create `<div id="references"/>` before the end of your body.
* Right after this empty `<div>` tag, create a multiline HTML comment and paste the BibTeX entry there. Let's say the name of the entry is `author1991`
* In the rest of the page, you can use `\cite{author1991}` just like in LaTeX and upon render the page should have APA formatted bib entries at the end and links to those entries (anchors) where you placed the `\cite{...}`.

**What else**:
* Default format is APA. Change in "bib" script accordingly. Consult with [citation-js documentation](https://citation.js.org/api/index.html).
* I still don't know how to get a DOI link from BibTex entry. If I had that the citations would point to the actual paper link, which would be cool to have.

**Libraries used**:
* [Citation JS](https://citation.js.org/api/index.html)
* JQuery
