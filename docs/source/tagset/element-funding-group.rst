.. _element-funding-group:

<funding-group>
===============

+------------------------------+--------------------+
| Appears in                   | Frequency          |
+==============================+====================+
| :ref:`element-article-meta`  | Zero or more times |
+------------------------------+--------------------+

Used to represent any reference made to a funding agency or a funding with an explicit contract number. The funding information can also appear in tags :ref:`element-fn` ou :ref:`element-ack`.

.. note:: 

  ``<funding-group>`` should be inserted before the element :ref:`element-counts` or after the :ref:`element-kwd-group`.

Example:

.. code-block:: xml

  ...
  <article-meta>
    ...
    <funding-group>
      <award-group>
        <funding-source>NSERC</funding-source>
        <award-id>12345</award-id>
      </award-group>
    </funding-group>
    ...
  </article-meta>
  ...

.. {"reviewed_on": "20180523", "by": "fabio.batalha@erudit.org"}
