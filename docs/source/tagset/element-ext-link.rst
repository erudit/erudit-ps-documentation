.. _element-ext-link:

<ext-link>
==========

Madatory attributes:

  1. ``@xlink:href``

+----------------------------------+--------------------+
| Appears in                       | Frequency          |
+==================================+====================+
| :ref:`elemento-comment`          | Zero or more times |
+----------------------------------+--------------------+
| :ref:`elemento-element-citation` | Zero or more times |
+----------------------------------+--------------------+
| :ref:`elemento-p`                | Zero or more times |
+----------------------------------+--------------------+
| :ref:`elemento-product`          | Zero or more times |
+----------------------------------+--------------------+

Specifies references to web resources on the Internet. The only restrictions on the use of this element are:

* The scheme must be explicit, in other words, it must begin with http://, ftp://, urn:, etc;
* Local references via the scheme file:// are not allowed.

Example URL:

.. code-block:: xml

    ...
    <p>This is the website of Érudit: <ext-link ext-link-type="uri" xlink:href="http://www.erudit.org">www.erudit.org</ext-link></p>
    ...

.. {"reviewed_on": "20180603", "by": "fabio.batalha@erudit.org"}
