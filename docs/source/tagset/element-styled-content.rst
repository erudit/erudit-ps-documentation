.. _element-styled-content:

<styled-content>
================


Mandatory attributes:

  1. ``@specific-use``

+----------------------------------+--------------------+
| Appears in                       | Frenquency         |
+==================================+====================+
| :ref:`element-element-citation`  | Once               |
+----------------------------------+--------------------+

Have the original representation of the bibliographic reference, as it was given by the publisher. In this current version of :ref:`Érudit PS` it is mainly used for display purpose. The attribute ``@specific-use`` is mandatory and it's value must be **display**.

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
