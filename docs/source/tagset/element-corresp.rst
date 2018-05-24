.. _element-corresp:

<corresp>
=========

+------------------------------+--------------------+
| Appears in                   | Frequency          |
+==============================+====================+
| :ref:`element-author-notes`  | Zero or more times |
+------------------------------+--------------------+

Element that contains the information about the correspondence of one or more of an article’s authors. It may or may not contain the element ``<label>``. The attribute ``@id`` is also optional. The email information can still be marked up with ``<email>``, if the information exists. 

The :ref:`id-attribution-tips` describes how to compose the ``@id`` attribute.

.. note::

  Do not use paragraph :ref:`element-p` inside this element.

Example:

.. code-block:: xml

  ...
  <author-notes>
    ...
    <corresp id="c01">Correspondence paragraph, email:<email>user@foo.com</email></corresp>
    ...
  </author-notes>
  ...

.. {"reviewed_on": "20180524", "by": "fabio.batalha@erudit.org"}
