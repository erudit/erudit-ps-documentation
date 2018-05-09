.. _element-kwd:

<kwd>
=====

+---------------------------+-------------------+
| Appears in                | Frequency         |
+===========================+===================+
| :ref:`element-kwd-group`  | One or more times |
+---------------------------+-------------------+

Mandatory element in :ref:`element-kwd-group` which identifies each keyword individually.


Example:

.. code-block:: xml

    ...
    <article-meta>
        ...
        <kwd-group xml:lang="fr">
            <title>Mots-clés</title>
            <kwd>francophonie minoritaire canadienne</kwd>
            <kwd>qualité de la langue</kwd>
            <kwd>jeunesse</kwd>
            <kwd>nationalisme linguistique</kwd>
            <kwd>idéologie linguistique</kwd>
        </kwd-group>
        <kwd-group xml:lang="en">
            <title>Keywords</title>
            <kwd>Canadian Francophone minority</kwd>
            <kwd>language quality</kwd>
            <kwd>youth</kwd>
            <kwd>linguistic nationalism</kwd>
            <kwd>language ideology</kwd>
        </kwd-group>
        ...
    </article-meta>
    ...

.. {"reviewed_on": "20180509", "by": "fabio.batalha@erudit.org"}
