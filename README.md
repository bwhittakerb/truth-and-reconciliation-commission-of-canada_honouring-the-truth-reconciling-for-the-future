# Readme

## About this document

This project is an attempt to format and typeset *Honouring the Truth, Reconciling for the Future: Summary of the Final Report of the Truth and Reconciliation Commission of Canada* from the Truth and Reconciliation Commission's existing and freely available PDF download into a standard and semantics-based EPUB format.

## Why EPUB?

It is the belief of this author that the Truth and Reconciliation Commission of Canada's report should be as accessible as widely as possible to all Canadians in a variety of formats. With the popularity of e-readers and the affordances available via digital book formats (e.g. 'popover endnotes'), the author of this project feels that making a digital publication of the Commission report summary will provide significant utility and accessibility to all interested readers. A static PDF is simply not designed for a reflowable and accessible experience.

EPUB is a broadly supported public standard for e-reading software with built in support in software available on many operating systems and directly on many hardware e-readers such as Kobo and Nook. Furthermore, this format can be easily converted to other e-reader formats such as Amazon Kindle.

Finally, as a format intended for semantic markup rather than optimized for pre-press like a PDF, EPUB and other derived e-reader formats allow screen reading software and other accessibility devices to work more efficiently and with greater clarity for impaired users who wish to read the report.

## Current status of this project

This is now buildable as a Minimum Viable e-book™ It's still missing many formatting niceties and may contain errors but is available for download as a 'beta version' for proofreaders. Currently the Standard Ebooks build tool crashes when it tries to build a Kindle version so it's only epub and kobo-optimized epub versions for now.

### Todos

* Tweak styling generally.
* Ensure Convictions Table in Appendix 3 is readable on small screens.
* Add additional semantics for abbreviations, times, dates, etc.
* Create final cover image.
* Create final (un)copyright page.
* add alt-text to all images.
* Convert SVGs to not use transforms.
* Add metadata to book.

## Files and structure

This project includes the source PDF as well as its extracted images in their original formats and converted to greyscale EPUB-friendly JPEGs. It is not currently packaged in a way that can be immediately read by e-reading software but that will be made available when the level of progress makes sense to do so.

## Toolsets being used to build this project

* Standard Ebooks (https://standardebooks.org) provides a style guide that is an invaluable reference as well as python-based EPUB automation tools.
* ARIA's Accessibility checker ACE: (https://inclusivepublishing.org/toolbox/accessibility-checker/)
* I used Popplers, a PDF command line toolkit, to extract the images embedded in the source pdf and imagemagick to convert them to JPEG from JPEG2000 (for increased e-reader support). The original JPEG2000 files were in the RGB colourspace despite being black and white images so I have converted them to greyscale colourspace at significant size savings.
* Typora for the initial cut and paste of the PDF text to markdown while preserving styled text formatting.
* Sublime Text for generic text processing.
* Calibre for its ebook management and editing tools
* My personal hardware e-reader is a Kobo Clara HD and I use Apple Books for mobile/desktop reading.


## How can I help?

This is a complex document with complex constructions within and I am sure that I have missed or overlooked items. How you can help now is to download the latest 'beta' version of the epub and proofread it and report issues as they come up. :)
