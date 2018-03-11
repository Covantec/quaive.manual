# quaive.manual
An end user manual for quaive

## Building locally

* Clone the repository
* You can build the documentation with `make html`.
  This will auto-bootstrap a virtualenv and install sphinx, only the first time you run it.
* The output can then be found under _build/html.
* To force a full rebuild, do `make clean html`.

## Languages supported

You can Building locally for specific languages, like these following:

**Deutsch documentation**

* You can build the PO message catalogs with `make gettext`.
* You can build the Deutsch documentation with `make html_de`.
* The output can then be found under **_build/html/de**.

**Spanish documentation**

* You can build the PO message catalogs with `make gettext`.
* You can build the Spanish documentation with `make html_es`.
* The output can then be found under **_build/html/es**.

## Adding Languages

Adding new languages you can execute these following command:

First activate the virtualenv:

    $ source bin/activate

Update specified language's po files from pot:

    $ sphinx-intl update -p ./locale/ -l <LANG>

**note:** `<LANG>` is the language code to add.
