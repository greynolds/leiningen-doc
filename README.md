leiningen-doc
=============

DITA documentation for Leiningen

# Contributing

# Building

Use either ditac or DITA-OT (links below).

## ditac

The instructions at
http://www.xmlmind.com/ditac/_distrib/doc/manual/manual-4.html#quickStart
are pretty clear.  The command I use to generate PDF is:

    $ /path/to/ditac tmp/ugbook.ditac.pdf ugbook.ditamap

## DITA-OT

The documentation isn't great, so you'll need to put in a little work
to figure out how to make it go.  What works for me is:

    <DITA_HOME> $ ant -Dargs.input=/path/to/leiningen-doc/ugbook.ditamap -Dtranstype=pdf

Must be executed from the toolkit's root dir; haven't figured out how
to get around that yet.  This puts the output in <DITA_HOME>/out.  I
haven't been able to figure out how to specify a different output dir.
Change the transtype parm to change the format, e.g. -Dtranstype=xhtml.

# DITA Resources

[DITA 1.2 Spec](http://docs.oasis-open.org/dita/v1.2/spec/DITA1.2-spec.html)

[DITA XML.org](http://dita.xml.org/) - "the official community gathering place and information resource for the DITA OASIS Standard."

[DITA Open Toolkit](http://dita-ot.github.io/)

(cmd: ant -Dargs.input=$HOME/dev/leiningen-doc/userguide.ditamap -Dtranstype=pdf2)

[XMLMind DITA Converter](http://www.xmlmind.com/ditac/)

Whitepapers: 

 * [An XML Architecture for Technical Documentation: The Darwin Information Typing Architecture](http://www.writersua.com/articles/DITA/)
 * [Hacking the DITA Open Toolkit](http://www.scriptorium.com/whitepapers/hackingot/index.html) (HTML)  ([PDF version](http://www.scriptorium.com/whitepapers/hackingot/hackingot.pdf)
 * [Customizing PDF Output in the DITA Open Toolkit](http://www.scriptorium.com/whitepapers/ditaotpdf/DITA-PDF-tweaks.pdf) (PDF)

Markdown:

 * [Standard Markdown](http://daringfireball.net/projects/markdown/syntax) at Daring Fireball
 * [GitHub Flavored Markdown](https://help.github.com/articles/github-flavored-markdown)
 * [GitHub markdown cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

# License

This work is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 3.0 Unported License. To view a copy of this license, visit http://creativecommons.org/licenses/by-nc-sa/3.0/ or send a letter to Creative Commons, 171 Second Street, Suite 300, San Francisco, California, 94105, USA.

