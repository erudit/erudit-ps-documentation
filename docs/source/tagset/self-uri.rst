.. _element-self-uri:

<self-uri>
==========

Madatory attributes:

  1. ``@xlink:href``

+----------------------------------+--------------------+
| Appears commonly in              | Frequency          |
+==================================+====================+
| :ref:`element-article-meta`      | Zero or more times |
+----------------------------------+--------------------+

.. note::

    See `JATS Specifications <https://jats.nlm.nih.gov/publishing/tag-library/1.2d1/element/attrib.html>`_ to see all the elements the ``<self-uri>`` could be inserted.

Specifies references to web resources on the Internet. The only restrictions on the use of this element are:

* The scheme must be explicit, in other words, it must begin with http://, ftp://, urn:, etc;
* Local references via the scheme file:// are not allowed.

Example URL:

.. code-block:: xml

    ...
    <article>
        <front>
            ...
            <article-meta>
                ...
                <self-uri xlink:href="file.pdf">Link para PDF</self-uri>
                ...
            </article-meta>
        </front>
        ...
    </article>
    ...

.. {"reviewed_on": "20181029", "by": "fabio.batalha@erudit.org"}
