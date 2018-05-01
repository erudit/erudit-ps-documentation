.. _element-pub-id:

<pub-id>
========


Mandatory attributes:

  1. ``@pub-id-type``

+----------------------------------+--------------------+
| Appears in                       | Frenquency         |
+==================================+====================+
| :ref:`element-element-citation`  | Zero or more times |
+----------------------------------+--------------------+

Specifies the identifier of a publication in a bibliographic reference. The attribute ``@pub-id-type`` is mandatory and states the type of identifier, authority or organization responsible for the identifier’s assignment.

Some examples of ``@pub-id-type`` are:

+--------+---------------------------------------+
| Value  | Description                           |
+========+=======================================+
| doi    | DOI number registered in Crossref     |
+--------+---------------------------------------+
| erudit | Article ID in Érudit                  |
+--------+---------------------------------------+
| pmid   | :term:`PubMed` ID                     |
+--------+---------------------------------------+
| pcmid  | :term:`PMC` ID                        |
+--------+---------------------------------------+
| pii    | Publisher identifier                  |
+--------+---------------------------------------+
| other  | Any other identifier                  |
+--------+---------------------------------------+

.. note::

    Even it is not mandatory, Érudit PS expects the presence of ``@pub-id-type=doi`` when the article has one DOI number.

Example:

.. code-block:: xml

    ...
    <element-citation publication-type="journal">
      <styled-content specific-use="display">
        Blommaert, J. (1999). Language Ideological Debates. Berlin : Mouton de Gruyter.
      </styled-content>
      <pub-id pub-id-type="doi">
        https://doi.org/10.1515/9783110808049
      </pub-id>           
    </element-citation>
    ...


.. {"reviewed_on": "20180501", "by": "fabio.batalha@erudit.org"}
