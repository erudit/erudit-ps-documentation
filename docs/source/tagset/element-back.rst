.. _element-back:

<back>
======

+-----------------------------+------------------+
| Appears in                  | Frequency        |
+=============================+==================+
| :ref:`element-article`      | Zero or one time |
+-----------------------------+------------------+

This is the final part of the :term:`document` which is made up of:

+--------------------------+
| Elements                 |
+==========================+
| :ref:`element-ack`       |
+--------------------------+
| :ref:`element-app-group` |
+--------------------------+
| :ref:`element-bio`       |
+--------------------------+
| :ref:`element-fn-group`  |
+--------------------------+
| :ref:`element-glossary`  |
+--------------------------+
| :ref:`element-ref-list`  |
+--------------------------+
| :ref:`notes`             |
+--------------------------+

.. note::

  In the context of :term:`Érudit PS` it is not recommended to use the element :ref:`sec` inside the element ``<back>``

Example:

.. code-block:: xml

   ...
   <back>
      ...
      <ref-list>
        <ref id="R1">
          <element-citation publication-type="journal">
            <styled-content specific-use="display">
              Arrighi, L. et Boudreau, A. (2013). La construction discursive de l'identité francophone en Acadie ou «comment être francophone à partir des marges?». Minorités linguistiques et société/Linguistic Minorities and Society. 2. 8-92.
            </styled-content>
            <pub-id pub-id-type="doi">
              https://doi.org/10.7202/1016689ar
            </pub-id>           
          </element-citation>
        </ref>
      ...
      </ref-list>
      ...
   </back>
   ...

.. {"reviewed_on": "20180530", "by": "fabio.batalha@erudit.org"}
