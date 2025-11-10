# Writing documents

This document describes common challenges when writing documents and proposes different processes to write documents.

## The problems

If you have used Microsoft Word, LibreOffice Writer, or Google Docs to write a non-trivial document, then you likely have faced some of these problems.

### What you see is what you get (WYSIWYG) document editors hide document structure

Popular document editors show you how your document would look when printed.

WYSIWYG editors tend to hide details about your document structure that make understanding the document behavior difficult.

For example, WYSIWYG editors frequently provide two ways of applying style to text.
You can alter the font, size, and others directly; or you can apply a defined style (such as header level 2).
Applying defined styles has many advantages, such as:

* You can edit the style, and all the text using the same style gets the updated style automatically.
  When editing style directly, you must apply changes manually everywhere.

* The editor can infer semantics from defined styles, such as considering text with the header style a header and collecting headers automatically in a table of contents.
  When applying header styles directly, automatic tables of contents do not work.

Often, WYSIWYG editors do not make obvious how styles are applied nor guide users to apply styles in the best way.
(Many editors provide features to show your document structure, but these features are frequently not enabled by default nor intuitive.)

### WYSIWYG editors favor paged documents

Although WYSIWYG editors frequently support creating documents that are not paged, most were designed with paged documents in mind and default to them.

In my experience, most documents are never printed, and most frequently, your readers will read them using a display, such as a phone, tablet, laptop, or computer monitor.

Editors provide features around paged documents that can be confusing, especially when you do not print them:

* [Widow and orphan control][Widows and orphans], where the editor tries to avoid having paragraphs interrupted by a page break.
  A WYSIWYG editor can make content jump unpredictably, confusing the user.

[Widows and orphans]: https://en.wikipedia.org/wiki/Widows_and_orphans "Widows and orphans"

* Page breaks, either manual or automatic (for example, to make chapters of a document start on a new page).
  On two-faced pages, page breaks can also skip an empty page so that content starts on the front face of a page.
  Page breaks can confuse users, especially if the editor does not show the page break clearly.

However, the worst consequence of paged documents is that paged documents frequently are painful to read on most displays.
When the document page size is larger than the display, readers must either scroll continuously or zoom out to read the content.
Additionally, because text sizes are fixed, readers might need to zoom in to read text comfortably and therefore require even more scrolling.

### WYSIWYG editors use complex document storage formats with bad interoperability

Different editors have different formats.
Because WYSIWYG editors support many features, those formats are often complex and frequently pose compatibility issues.
Editing documents using different software can result in many annoyances, such as harmful unexpected formatting changes.
