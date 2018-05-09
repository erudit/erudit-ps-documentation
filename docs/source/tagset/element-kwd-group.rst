.. _element-kwd-group:

<kwd-group>
===========

Mandatory attribute:

  1. ``@xml:lang``

+------------------------------+--------------------+
| Appears in                   | Frequency          |
+==============================+====================+
| :ref:`element-article-meta`  | Zero or more times |
+------------------------------+--------------------+
| :ref:`element-front-stub`    | Zero or more times |
+------------------------------+--------------------+

Identifies the group of article keywords by language. It must contain the attribute ``@xml:lang``. ``<kwd-group>``, it must have a title identifying the group by
means of the <title> element, and it must have at least one element :ref:`kwd` inside ``<kwd-group>``.

.. note::

    To simplify the usage, the elements ``<nested-kwd>`` and ``<compound-kwd>`` are not allowed inside ``<kwd-group>``.

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
        ...
    </article-meta>
    ...



.. {"reviewed_on": "20180509", "by": "fabio.batalha@erudit.org"}
