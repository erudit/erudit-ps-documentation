.. _element-issn:

<issn>
======

Mandatory attributes:

  1. ``@pub-type='ppub'`` ou ``@pub-type='epub'``

+----------------------------------+-------------------+
| Appears in                       | Frequency         |
+==================================+===================+
| :ref:`element-journal-meta`      | One or more times |
+----------------------------------+-------------------+
| :ref:`element-element-citation`  | One or more times |
+----------------------------------+-------------------+



:term:`ISSN` is an :term:`ISO 3297:2007` numeric code which uniquely identifies a serial publication. Normally, each type of media used by a journal has its own specific ISSN.

This information can also be found in :ref:`element-back` within :ref:`element-element-citation` in the references, but no attribute is used in this case.

The allowed values for  ``@pub-type`` are:

+-------+-----------------------------+
| Value | Description                 |
+=======+=============================+
| ppub  | ISSN of the print version   |
+-------+-----------------------------+
| epub  | ISSN of the digital version |
+-------+-----------------------------+

If available, both ISSN’s should be identified.

Exemplos:

 * :ref:`element-issn-example-1`
 * :ref:`element-issn-example-2`


.. _element-issn-example-1:

Example of ISSN in ``<journal-meta>``:
--------------------------------------

.. code-block:: xml

    ...
    <journal-meta>
        ...
        <issn pub-type="epub">1712-2139</issn>
        <issn pub-type="ppub">0316-6368</issn>
        ...
    </journal-meta>
    ...


.. _element-issn-example-2:

Example of ISSN in ``<element-citation>``:
------------------------------------------

.. code-block:: xml

  ...
    <element-citation publication-type="journal">
       ...
      <source>Revue de l'Université de Moncton</source>
      <volume>44</volume>
      <issue>2</issue>
      <year>2013</year>
      <issn>1712-2139</issn>
    </element-citation>
  ...


.. {"reviewed_on": "20180427", "by": "fabio.batalha@erudit.org"}
