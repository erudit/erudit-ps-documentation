.. _element-abstract:

<abstract>
==========

Mandatory attributes:

  1. ``xml:lang``

+------------------------------+--------------------+
| Appears in                   | Frequency          |
+==============================+====================+
| :ref:`element-article-meta`  | Zero or more times |
+------------------------------+--------------------+

Element that identifies the abstract of an article. It must contain the attribute ``@xml:lang`` and one of the elements :ref:`element-p` or :ref:`element-sec`.

The abstracts could be presented in two different formats (structured and simple).

Examples:

    * :ref:`element-abstract-example-1`
    * :ref:`element-abstract-example-2`

.. _element-abstract-example-1:

Example of structured ``<trans-abstract>``:
-------------------------------------------

The **Structured format** has groups of text arranged in sections identified with a title (For example: Introduction, Objectives, Methodology and Results).

Example:

  .. code-block:: xml

      ...
      <article-meta>
          ...
          <abstract xml:lang="pt">
            <title>Resumo</title>
            <sec>
              <title>Objetivo</title>
              <p>Verificar a sensibilidade e especificidade das curvas de fluxo-volume na detecção de obstrução da via aérea central (OVAC), e se os critérios qualitativos e quantitativos da curva se relacionam com a localização, o tipo e o grau de obstrução.</p>
            </sec>
            <sec>
              <title>Métodos</title>
              <p>Durante quatro meses foram selecionados, consecutivamente, indivíduos com indicação para broncoscopia. Todos efetuaram avaliação clínica, preenchimento de escala de dispneia, curva de fluxo-volume e broncoscopia num intervalo de uma semana. Quatro revisores classificaram a morfologia da curva sem conhecimento dos dados quantitativos, clínicos e broncoscopicos. Um quinto revisor averiguou os critérios morfológicos e quantitativos.</p>
            </sec>
          </abstract>
          ...
      </article-meta>
      ...


.. _element-transabstract-example-2:

Example fo simple ``<trans-abstract>``:
---------------------------------------

The **simple** format presents a brief summary of the main points of the article without division into sections.

Example:

  .. code-block:: xml

      ...
      <article-meta>
          ...
          <abstract xml:lang="pt">
            <title>Resumo</title>
              <p>Verificar a sensibilidade e especificidade das curvas de fluxo-volume na detecção de obstrução da via aérea central (OVAC), e se os critérios qualitativos e quantitativos da curva se relacionam com a localização, o tipo e o grau de obstrução. Métodos: Durante quatro meses foram selecionados, consecutivamente, indivíduos com indicação para broncoscopia. Todos efetuaram avaliação clínica, preenchimento de escala de dispneia, curva de fluxo-volume e broncoscopia num intervalo de uma semana. Quatro revisores classificaram a morfologia da curva sem conhecimento dos dados quantitativos, clínicos e broncoscopicos. Um quinto revisor averiguou os critérios morfológicos e quantitativos.</p>
          </abstract>
          ...
      </article-meta>
      ...

.. {"reviewed_on": "20180509", "by": "fabio.batalha@erudit.org"}