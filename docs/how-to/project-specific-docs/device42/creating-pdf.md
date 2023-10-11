# Create a PDF version of Device42 documentation site

* Start the docs project on localhost:3000
* Run the following command (note the PDF is 1500+ pages, so it takes up to 30 mins to generate, hence the protocolTimeout)
* Save something like [this document](https://docs.google.com/document/d/1P0FxClhfjb0GMnS4ccVOYKWfsCfxT7E9LqGGWwyjFt4/edit#heading=h.wo9ldjw9o7vy) as a PDF and add it as the first page, deleting the first page that is automatically generated

```
npx docs-to-pdf --initialDocURLs="http://localhost:3000/getstarted/" --contentSelector="article" --paginationSelector="a.pagination-nav__link.pagination-nav__link--next" --excludeSelectors=".margin-vert--xl a,[class^='tocCollapsible'],.breadcrumbs,.theme-edit-this-page" --coverImage="https://www.device42.com/wp-content/uploads/2021/07/d42-rgb-full.png" --coverTitle="Device42 Documentation" --protocolTimeout 18000000
```

Editing the file in Preview.app (e.g. to delete the first page and add the custom cover) increases the file size a lot.An alternative is to use pdftk (`brew install pdftk-java`).

Then create a version without the first page, and add the cover into a new doc called 'combined.pdf'.

```
pdftk docs-to-pdf.pdf cat 2-end output docs-excluding-first.pdf
pdftk A=cover.pdf B=docs-excluding-first.pdf cat A B output combined.pdf
```


