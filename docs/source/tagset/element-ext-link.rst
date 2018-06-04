.. _element-ext-link:

<ext-link>
==========

Madatory attributes:

  1. ``@ext-link-type``
  2. ``@xlink:href``

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


Especifica referências a recursos disponíveis na internet. As únicas restrições quanto à sua utilização são:

* O *scheme* deve ser explícito, ou seja, deve começar com ``http://``, ``ftp://``,   ``urn:`` etc;
* Referências locais, por meio do *scheme* ``file://`` não são permitidas.

Os valores possíveis para o ``@ext-link-type`` são:

* uri
* clinical-trial


Example URL:

.. code-block:: xml

    ...
    <p>This is the website of Érudit: <ext-link ext-link-type="uri" xlink:href="http://www.erudit.org">www.erudit.org</ext-link></p>
    ...

.. {"reviewed_on": "20180603", "by": "fabio.batalha@erudit.org"}
