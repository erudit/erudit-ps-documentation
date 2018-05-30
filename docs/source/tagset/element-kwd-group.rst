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

Identifies the group of article keywords by language. It must contain the attribute ``@xml:lang``. ``<kwd-group>``, and it must have at least one element :ref:`element-kwd` inside ``<kwd-group>``.

.. note::

    The element ``<title>`` is not mandatory, but as best practice, the :term:`Érudit PS` suggests it should be available.

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



.. {"reviewed_on": "20180530", "by": "fabio.batalha@erudit.org"}
