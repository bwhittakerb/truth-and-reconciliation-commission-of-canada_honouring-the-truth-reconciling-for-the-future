# Readme


## About this project

This project is a total conversion of the publication *Honouring the Truth, Reconciling for the Future: Summary of the Final Report of the Truth and Reconciliation Commission of Canada* from the Truth and Reconciliation Commission's existing and freely available PDF download into a standard and semantics-based EPUB format for electronic reading. It, and its source code and components is free to all.


## Why EPUB?

It is our belief that the Truth and Reconciliation Commission of Canada's report should be as **accessible as widely as possible to all Canadians in a variety of formats**. With the popularity of e-readers and the affordances available via digital book formats (e.g. 'popover endnotes'), the author of this project feels that making a digital publication of the Commission report summary will provide significant utility and accessibility to all interested readers. A static PDF is simply not designed for a reflowable and accessible experience.

EPUB is a broadly supported public standard for e-reading software with built in support in software available on many operating systems and directly on many hardware e-readers such as Kobo and Nook. Furthermore, this format can be easily converted to other e-reader formats such as Amazon Kindle.

Finally, as a format intended for semantic markup rather than optimized for pre-press like a PDF, EPUB and other derived e-reader formats allow screen reading software and other accessibility devices to work more efficiently and with greater clarity for impaired users who wish to read the report.


## Current status of this project

Version 1.0 has been released! This is a complete readable and formatted copy with accessability and other affordances. [The latest compiled formats are found here][latest release]. Please read below to get instructions on which version is right for you and how to download them to your preferred device.


## How to get this ebook

* [You can download the standard epub version here][epub download link] (works on most computer readers and Apple devices and many Android apps).

* [You can download the Kobo-optimized version here.][kobo download link]

* [You can download the Kindle version here.][kindle download link]

### How to install kepub.epub files on a Kobo:

(Instructions copied from standardebooks.org)

**Important:** Don’t use Calibre to transfer the kepub file! Calibre will apply its own conversion on top of our own conversion, making for strange results.

1. Using a USB cable, connect your Kobo to the computer you downloaded [the kepub file][kobo download link] to. Your Kobo will appear as a USB drive that you can browse using your computer’s file manager.
2. Navigate to the Kobo drive and drag and drop the kepub file in. *Don’t change the filename of the ebook! Kobo requires that the filename end in `.kepub.epub.`*
3. Eject the Kobo from your computer using your system’s “Safely remove drive” option. Your ebook should now be visible!

### How to install/read the .epub file on your iPhone/iPad

1. Tap on the [download link][epub download link] for the standard epub file.
2. On the download screen that appears, tap “open in Books”.

### Amazon Kindle eInk Devices (Paperwhite, Voyage, Oasis, etc. except DX)

Important: You can’t use “Send to Kindle” to transfer the azw3 file. This is a bug in Amazon’s software. You *must* transfer the azw3 file to Kindles with a USB cable.

1. Using a USB cable, connect your Kindle to the computer you downloaded [the azw3 file][kindle download link] to. Your Kindle will appear as a USB drive that you can browse.

2. Navigate to the documents folder on your Kindle, then drag and drop the azw3 file into the documents or ebooks folder.

3. If you don’t see a system folder when your Kindle is plugged in, you may have to tell your computer to show hidden system files. If you’re using Windows, you may also have to show protected operating system files. To do that, see [these instructions for Windows](https://www.howtogeek.com/howto/windows-vista/show-hidden-files-and-folders-in-windows-vista/) and [these instructions for Mac](https://www.lifewire.com/display-hidden-files-in-os-x-153332).

4. Eject the Kindle from your computer using your system’s “Safely remove drive” option. Your ebook should now be visible!

## How can I help?

The best way to help is to read the report. The second best way to help is to report any errors or oddities you experience. This is a sophisticated document with complex structure and formatting. There is almost certainly overlooked problems or issues. If you experience any, please open an issue on github or reach out to me directly on Twitter at @distinctivename. Otherwise, I'm very much open to contributors or forking to make the best possible digital version of this book.

### Todos for 2.0

* Tweak styling generally.
* Ensure Convictions Table in Appendix 3 is readable on small screens.
* Add additional semantics for abbreviations, times, dates, etc.
* Convert SVGs to not use transforms.
* Mark up Apology subheaders appropriately.
* Create hyperlinks from Calls to Action section to each Call's context in the mainmatter.
* ~~Tweak styling on Calls to Action.~~
* ~~Create final cover image.~~
* ~~Create final (un)copyright page.~~
* ~~Add alt-text to all images.~~
* ~~Add metadata to book.~~

### Files and structure

This project includes the source PDF as well as its extracted images in their original formats and converted to greyscale EPUB-friendly JPEGs.

* Files that will comprise the content of the epub file itself are located in `/src/`
* Files used to build graphics for the epub cover are located in `/images/`
* Files used to construct material for the ebook but not be part of the bundle (e.g. Original PDF document, Vector Files, Markdown conversions, etc) are located in `/sourcefiles/`
* Actual e-reader files will be compiled and listed in the 'releases' section.

### Toolsets being used to build this project

* [Standard Ebooks](https://standardebooks.org) provides a style guide that is an invaluable reference as well as python-based EPUB automation tools.
* ARIA's Accessibility checker [ACE](https://inclusivepublishing.org/toolbox/accessibility-checker/).
* [Poppler](https://poppler.freedesktop.org), a PDF command line toolkit, was used to extract the images embedded in the source PDF and imagemagick to convert them to JPEG from JPEG2000 (for increased e-reader support). The original JPEG2000 files were in the RGB colourspace—despite being black and white images—so I have converted them to greyscale colourspace at significant size savings.
* [Typora](https://typora.io) for the initial cut and paste of the PDF text to markdown while preserving styled text formatting.
* [Sublime Text](https://www.sublimetext.com) for generic text processing.
* [Calibre](https://calibre-ebook.com) for its ebook management and editing tools
* My personal hardware e-ink reader is a Kobo Clara HD and I use Apple Books for mobile/desktop reading.

[latest release]: https://github.com/bwhittakerb/truth-and-reconciliation-commission-of-canada_honouring-the-truth-reconciling-for-the-future/releases/tag/v0.97-releasecandidate
[epub download link]: https://github.com/bwhittakerb/truth-and-reconciliation-commission-of-canada_honouring-the-truth-reconciling-for-the-future/releases/download/v0.97-releasecandidate/TRC_honouring-the-truth-reconciling-for-the-future.epub
[kobo download link]: https://github.com/bwhittakerb/truth-and-reconciliation-commission-of-canada_honouring-the-truth-reconciling-for-the-future/releases/download/v0.97-releasecandidate/TRC_honouring-the-truth-reconciling-for-the-future_kobo.kepub.epub
[kindle download link]: https://github.com/bwhittakerb/truth-and-reconciliation-commission-of-canada_honouring-the-truth-reconciling-for-the-future/releases/download/v0.97-releasecandidate/TRC_honouring-the-truth-reconciling-for-the-future_kindle.azw3