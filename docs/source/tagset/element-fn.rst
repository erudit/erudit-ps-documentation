.. _element-fn:

<fn>
====

Mandatory attribute:

  1. ``@id`` (see :ref:`id-attribution-suggestion`)

+-------------------------+--------------------+
| Appears at              | Frequency          |
+=========================+====================+
| :ref:`element-fn-group` | One or more times  |
+-------------------------+--------------------+

General notes usually referencing some information of the current :term:`document` and research.

The element ``<fn>`` may have the attribute ``fn-type``. It is not mandatory to use it, but used, it should follow as much as possible the :term:`NISO JATS Journal Archiving DTD` recomendation for ``@fn-type``.

Example:

.. code-block:: xml

  ...
  <fn-group>
    <title>Footnotes</title>
    <fn id="fn1" fn-type="supplementary-material">
      <label>1.</label>
      <p>Ce débat n’est pas, loin s’en faut, spécifiquement acadien, ni même propre aux milieux minoritaires. Pour un exemple de son actualisation en France, voir Bentolina (1996, 2000), et pour une approche critique de celui-ci en ce même lieu, voir Moïse (2007). Pour le Québec, on peut consulter Vincent (2008). </p>
    </fn>
    <fn id="fn2">
      <label>2.</label>
      <p>Nous référons aux divers contributeurs au débat étudié par leur statut (journaliste, professeur, étudiant, etc.). Non seulement ils se présentent ainsi dans leurs prises de parole, mais aussi, lors de débats, ils sont le plus fréquemment mentionnés, cités selon leur statut. La question de leur statut n’est pas négligeable pour comprendre leurs prises de parole, et nous consacrons d’ailleurs un développement à ce point (voir section 2.3). </p>
    </fn>
    ...
  </fn-group>
  ...


.. {"reviewed_on": "20191011", "by": "mathieu.pigeon@erudit.org"}
