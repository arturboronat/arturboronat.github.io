# Artur home page and portfolio

This is a resume template built with [Jekyll](https://jekyllrb.com/) that is ready for use with [GitHub Pages](https://pages.github.com/). There are sections for employment history, education, publications and presentations. It also includes [Reveal.js](https://revealjs.com/#/) allowing you to create and host presentations directly from your GitHub Pages User page.

## Configuration

* Original: https://github.com/toddstoffer/jekyll-academic-resume
* [Jekyll ORCID](https://github.com/mfenner/jekyll-orcid)

## Publishing page

To test web site: `bundle exec jekyll serve`, then access [http://0.0.0.0:4000/](http://0.0.0.0:4000/)

To publish web site; `../publish.sh "COMMIT MESSAGE"`

## Creating content

### Posts: articles and news

1. Create a draft md document in `_drafts` without date (name can contain letters and '-') and test the web page with `bundle exec jekyll serve --drafts`.
2. To publish the draft, move the file to `_posts` and add the prefix `YYYY-MM-DD-` and test with `bundle exec jekyll serve`.

### Bibliography

Add BibTeX entries to `./_bibliography/boronat.bib` with appropriate tags:
* add publications in `./assets/docs/` using the naming convention `YYYY-boronat-conference.pdf`
* add field `webdownload={YYYY-boronat-conference.pdf}` to BibTeX entry
* add DOI in field `webdoi`

To customize the way publications are rendered:
* In publications: modify CSS using `ol.bibliography`
* In research_themes: modify `./_layouts/bib.html`

## Modifying layout

* Use [boostrap 3.3.7](https://getbootstrap.com/docs/3.3/components/)
* [Shopify Liquid](https://shopify.github.io/liquid/) is the templating language using in html documents, which fetch data from the YAML files

## Other

### Creating Presentations
This Jekyll theme includes [Reveal.js](https://revealjs.com/#/) which is a lightweight framework that enables you to create slide decks using HTML and Markdown, and to host and present those slide decks from your website. To create a new presentation using Reveal.js make a copy of the example-presentation.md file in the \_presentations and begin editing it following the instructions found in the [Reveal.js repository](https://github.com/hakimel/reveal.js/).
