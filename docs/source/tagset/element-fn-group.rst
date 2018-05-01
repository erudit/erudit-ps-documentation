.. _element-fn-group:

<fn-group>
==========

+----------------------+--------------------+
| Appears at           | Frequency          |
+======================+====================+
| :ref:`element-back`  | Zero or more times |
+----------------------+--------------------+


``<fn-group>`` faz parte do elemento :ref:`elemento-back` e deve conter todo o grupo de notas de rodapé mencionadas no :term:`documento`, que estão relacionadas com o documento como um todo, não confundir com notas de rodapé relacionadas ao autor. Este elemento pode apresentar um único título identificado com ``<title>`` e uma ou mais notas :ref:`elemento-fn`.

``<fn-group>`` is part of the element :ref:`element-back` and must contain the entire group of footnotes mentioned in the :term:`document` which are related to the document as a whole. Do not confuse this with footnotes related to the author. This element could have a single title identified with ``<title>`` and must have one or more notes :ref:`element-fn`.

Example:

.. code-block:: xml

    ...
    <back>
        ...
        <fn-group>
            <title>Footnotes</title>
            <fn id="fn1">
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
    </back>
    ...


.. {"reviewed_on": "20180501", "by": "fabio.batalha@gmail.com"}
