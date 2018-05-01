.. _element-back:

<back>
======

+-----------------------------+------------------+
| Appears in                  | Ocorre           |
+=============================+==================+
| :ref:`element-article`      | Zero ou one time |
+-----------------------------+------------------+


This is the final part of the :term:`document` which is made up of:


+--------------------------+
| Elements                 |
+==========================+
| :ref:`elemento-ref-list` |
+--------------------------+
| :ref:`elemento-fn-group` |
+--------------------------+
| :ref:`elemento-ack`      |
+--------------------------+
| ``app-group``            |
+--------------------------+
| ``app-group``            |
+--------------------------+
| ``app-group``            |
+--------------------------+
| :ref:`elemento-glossary` |
+--------------------------+


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
