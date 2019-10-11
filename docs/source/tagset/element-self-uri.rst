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

    See :term:`NISO JATS Journal Archiving DTD` specifications to see all the elements the ``<self-uri>`` could be inserted.

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

.. {"reviewed_on": "2019-10-11", "by": "mathieu.pigeon@erudit.org"}
