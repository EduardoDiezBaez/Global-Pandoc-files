# Global Pandoc configuration files

After years of trying to perfect the conversion of academic Markdown files to Word (for people who swear by it), I think I've stumbled on the holy grail, thanks to Duke's [Kieran Healy](http://kieranhealy.org/blog/archives/2014/01/23/plain-text/). This repository is a non-forked fork of [this](https://github.com/kjhealy/pandoc-templates), but with the added ability to convert Markdown files into perfeclty styled Word documents, in addition to TeX, HTML, and PDF. 

Pandoc allows you to create custom output templates for most file formats, but unfortunately not for `.docx` files. Following Kieran's lead, this repository includes `odt.template` and `reference.odt`, which places and styles custom metadata (like author information) into an `.odt` file. This can then be converted to `.docx`, either manually (by opening LibreOffice) or with the command line:

	/Applications/LibreOffice.app/Contents/MacOS/soffice.bin --invisible --convert-to docx filename.odt

If I understood Makefile syntax better, I'd add a set of rules to convert from `.odt` to `.docx`, but I don't have time to figure that out now.

But HOLY GRAIL! Markdown to Word, HTML, and PDF with one command. Beautiful.

