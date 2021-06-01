# Readme

## About this document

This project is an attempt to format and typeset *Honouring the Truth, Reconciling for the Future: Summary of the Final Report of the Truth and Reconciliation Commission of Canada* from the Truth and Reconciliation Commission's existing and freely available PDF download into a standard and semantics-based EPUB format.

## Why EPUB?

It is the belief of this author that the Truth and Reconciliation Commission of Canada's report should be as accessible as widely as possible to all Canadians in a variety of formats. With the popularity of e-readers and the affordances available via digital book formats (e.g. 'popover endnotes'), the author of this project feels that making a digital publication of the Commission report summary will provide significant utility and accessibility to all interested readers. A static PDF is simply not designed for a reflowable and accessible experience.

EPUB is a broadly supported public standard for e-reading software with built in support in software available on many operating systems and directly on many hardware e-readers such as Kobo and Nook. Furthermore, this format can be easily converted to other e-reader formats such as Amazon Kindle.

Finally, as a format intended for semantic markup rather than optimized for pre-press like a PDF, EPUB and other derived e-reader formats allow screen reading software and other accessibility devices to work more efficiently and with greater clarity for impaired users who wish to read the report.

## Current status of this project

Currently this is an initial upload with only the very roughest cut and paste of the text of the PDF. The next steps will involve a massive cleanup of the text as well as adding appropriate file splits and semantic markups. I will be working mostly with the markdown files of the text in the 'sourcefiles' directory and converting to semantic HTML from this document as I go for the first phase of this project.

This project includes the source PDF as well as its extracted images in their original formats and converted to greyscale EPUB-friendly JPEGs. It is not currently packaged in a way that can be immediately read by e-reading software but that will be made available when the level of progress makes sense to do so.

## Toolsets being used to build this project

* Standard Ebooks (https://standardebooks.org) provides a style guide that is an invaluable reference as well as python-based EPUB automation tools.
* I used Popplers, a PDF command line toolkit, to extract the images embedded in the source pdf and imagemagick to convert them to JPEG from JPEG2000 (for increased e-reader support). The original JPEG2000 files were in the RGB colourspace despite being black and white images so I have converted them to greyscale colourspace at significant size savings.
* Typora for the initial cut and paste of the PDF text to markdown while preserving styled text formatting.
* Sublime Text for generic text processing.
* Calibre for its ebook management and editing tools
* My personal hardware e-reader is a Kobo Clara HD


## How can I help?

It is anticipated that the several thousand endnotes will require significant manual labour to code correctly and semantically for e-readers in which contributions to a shared google sheet in the future would be gratefully accepted. In addition, helpful proof reading from a variety of readers on a variety of devices or reading applications would be invaluable.
