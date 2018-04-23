.. _element-journal-id:

<journal-id>
============

Mandatory Atributes:

  1. ``@journal-id-type``

+------------------------------+-------------------+
| Contained at                 | Frequency         |
+==============================+===================+
| :ref:`element-journal-meta` | One or more time   |
+------------------------------+-------------------+



Contém o identificador único do periódico indexado em uma base de dados ou instituição publicadora. Minimamente, o acrônimo do periódico deve ser identificado por meio do valor ``publisher-id``.

É obrigatório ter ao menos uma ocorrência de ``<journal-id>`` com o valor ``publisher-id`` no atributo ``@journal-id-type``. Nesta ocorrência deve ser identificado o acrônimo do periódico.

The allowed values for ``@journal-id-type`` are:

+---------------+-----------------------------------------+
| Value         | Description                             |
+===============+=========================================+
| publisher-id  | Journal id at Érudit database           |
+---------------+-----------------------------------------+

Example:

.. code-block:: xml

    ...
    <journal-meta>
        ...
        <journal-id journal-id-type="publisher-id">mioc</journal-id>
        <journal-id journal-id-type="nlm-ta">Mem Inst Oswaldo Cruz</journal-id>
        ...
    </journal-meta>
    ...


.. {"reviewed_on": "20180422", "by": "fabio.batalha@erudit.org"}