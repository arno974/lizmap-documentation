Lizmap - Documentation
=======================

This repository contains the complete documentation of the Lizmap application.

Lizmap allows to publish online QGIS maps.

The documentation is localized into several language. The main language is
the english. 

Contributing to the english documentation
=========================================

Clone the repository and edit files into `sources/`.

The format is the ReStructured Text format. 

See below to build the documentation into HTML to see the result.


Contributing by translating the doc into other languages
=========================================================

We are using [Transifex](https://www.transifex.com/3liz-1/lizmap-documentation/)
to translate the documentation. So if you want to contribute to the translation,
create an account on the Transifex web site, and translate different strings.

We retrieve regurlarly translation and store them into the `i18n/` directory. 

We don't recommend to contribute on translations by doing Pull Request on
github, as it may be difficult to merge content coming from Transifex and your
changes.

Building the documentation
===========================

We are using the tool [Sphinx](http://sphinx-doc.org)  and its 
internationalization mechanism [sphinx-intl](http://sphinx-doc.org/intl.html) to 
generate the HTML content in all languages.

So install these tools. On Linux / MacOs, install Python, Pip and then:

```
sudo pip install -U sphinx
sudo pip install -U sphinx-intl
```

Then run `make gettext && make html`. It will build the docs in all available 
languages.

For core contributor
--------------------

See DEV.md to see instructions to push and pull translated files to/from Transifex.


