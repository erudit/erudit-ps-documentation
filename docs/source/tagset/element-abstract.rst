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

Element that identifies the abstract of an article. It must contain the attribute ``@xml:lang`` and one of the elements :ref:`element-p` or :ref:`element-sec`. It is allowed to specify the ``@abstract-type``. The list of allowed values for ``@abstract-type`` follows the `JATS Specification <https://jats.nlm.nih.gov/publishing/tag-library/1.2d1/attribute/abstract-type.html>`_.

List of allowed values for ``@abstract-type``:

+-------------------+-------------------------------------------------------------------+
| Érudit Article    |  Description                                                      |
+===================+===================================================================+
| ASCII             |  A “plain text” abstract, i.e., without special characters or     |
|                   |  equations, so the abstract can be sent in email or displayed on  |
|                   |  primitive browsersRefers to books. It can also represent only a  |
|                   |  part or chapter of                                               |
+-------------------+-------------------------------------------------------------------+
| executive-summary |  A non-technical summation of the major findings of the article   |
|                   |                                                                   |
+-------------------+-------------------------------------------------------------------+
| graphical         |  A pictorial representation such as a picture or a video          |
|                   |                                                                   |
+-------------------+-------------------------------------------------------------------+
| editor            |  An abstract written by an editor, not an author                  |
|                   |                                                                   |
+-------------------+-------------------------------------------------------------------+
| key-points        |  An abstract which lists the key points made by the article       |
|                   |                                                                   |
+-------------------+-------------------------------------------------------------------+
| objetives         |  An abstract used for Learning Objectives or article objectives   |
|                   |                                                                   |
+-------------------+-------------------------------------------------------------------+
| section           |  An abstract containing the titles of an article’s sections;      |
|                   |  following each title, that section is summarized.                |
|                   |                                                                   |
+-------------------+-------------------------------------------------------------------+
| stereochemical    |  An abstract containing only the details of a chemical compound,  |
|                   |  for example, one major publisher’s “stereochem” abstract         |
|                   |                                                                   |
+-------------------+-------------------------------------------------------------------+
| teaser            |  A short abstract specifically written to create interest in the  |
|                   |  reader                                                           |
|                   |                                                                   |
+-------------------+-------------------------------------------------------------------+
| web-summary       |  Short summary intended for distribution on a website             |
|                   |                                                                   |
+-------------------+-------------------------------------------------------------------+
| other             |  Refers to books. It can also represent only a part or chapter of |
|                   |  a book.                                                          |
+-------------------+-------------------------------------------------------------------+
| toc               |  A very short abstract, usually only a line or two long, that is  |
|                   |  displayed in a Table of Contents                                 |
|                   |                                                                   |
+-------------------+-------------------------------------------------------------------+
| short             |  An abbreviated form of the abstract, for example, for use inside |
|                   |  a generated Table of Contents, or to be returned in addition to  |
|                   |  the article title during a search                                |
|                   |                                                                   |
+-------------------+-------------------------------------------------------------------+
| summary           |  Summation of the article, typically used in conjunction with     |
|                   |  other types of abstracts                                         |
|                   |                                                                   |
+-------------------+-------------------------------------------------------------------+

.. note::

  The attribute ``@abstract-type`` is not mandatory. The absense of this attribute means the abstract will be intrepreted as a **summary**. See the :ref:`compatibility-reference` documentation for more information.

.. note::

  The abstracts could be presented in two different formats (structured and simple).

Examples:

  * :ref:`element-abstract-example-1`
  * :ref:`element-abstract-example-2`

.. _element-abstract-example-1:

Example of simple ``<abstract>``:
---------------------------------

The **simple** format presents a brief summary of the main points of the article without division into sections.

Example:

  .. code-block:: xml

    ...
    <article-meta>
      ...
      <abstract xml:lang="fr">
        <title>Résumé</title>
        <p>Cet article a pour objectif d’analyser un débat linguistique idéologique centré sur le rapport établi entre l’avenir de la francophonie canadienne, la qualité de la langue et le devoir de la jeunesse en la matière. L’idée que la jeunesse serait particulièrement responsable de la dégradation de la langue fait l’objet d’un discours ancien et sans cesse redéployé. Nous proposons une approche critique de son actualisation récente en Acadie, telle qu’elle s’est manifestée dans des publications médiatiques aux parentés argumentatives fortes, entre l’automne 2012 et le printemps 2013. Afin d’objectiver les prises de position, nous montrons qu’elles puisent légitimité et autorité dans les fondements idéologiques du nationalisme politique moderne, qui font de la langue le ciment de l’identité collective et de sa « bonne maîtrise » une compétence accessible sur base démocratique.</p>
      </abstract>
      ...
    </article-meta>
    ...

.. _element-abstract-example-2:

Example of structured ``<abstract>``:
-------------------------------------

The **Structured** format has groups of text arranged in sections identified with a title (For example: Introduction, Objectives, Methodology and Results).

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

.. {"reviewed_on": "20180530", "by": "fabio.batalha@erudit.org"}