.. include:: partials/substitutions.rst

*************************
MGnify Genomes Catalogues
*************************

In the presentation we will cover:

- Recap of :ref:`mag:MAG Generation`
- Overview of MGnify MAG Catalogues
- Annotations available for catalogues and genomes
- Metadata available for catalogues and genomes
- Download files available for catalogues and genomes, via web, FTP, and the API
- Search mechanisms available against catalogues

MAG Catalogues hands-on exercises
#################################

These exercises will again use the `API <https://en.wikipedia.org/wiki/API>`_ ("Application programming interface"),
showing how your scripts (e.g. Python or R) can talk to the MGnify database.

This builds on the exercises you looked at in the :ref:`services:API` practical.

The practical will use a Jupyter Notebook.

Do you have MAGs?
-----------------

|info| For the last few exercises, you need some MAGs.
If you didn’t get as far as making your own MAGs in the :ref:`mag:MAG Generation` exercises,
you can copy some we made earlier with this command in a Terminal:

.. code-block:: bash

    cp -r /media/penelopeprime/Metagenomics-Nov21/Day4/day-4-example-mag-bins/* ~/mags

If you DID make your own, copy them to :code:`~/mags`.

.. include:: partials/jupyter.rst

Today's Notebook is "Day 4".
