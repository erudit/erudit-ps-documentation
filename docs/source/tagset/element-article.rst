.. _element-article:

<article>
=========

Mandatory  Attributes:

  1. ``@dtd-version``
  2. ``@article-type``
  3. ``@xml:lang``
  4. ``@xmlns:mml``
  5. ``@xmlns:xlink="http://www.w3.org/1999/xlink"``
  6. ``@specific-use="sps-1.8"``

.. note:: In the attribute ``@specific-use`` the value **eps-0.1** is only a reference to the version of the *Érudit PS*. this value should be one of the active versions.

+--------------+-------------+
| Appears in   | Frenquency  |
+==============+=============+
| ``/``        | Once        |
+--------------+-------------+



:ref:`element-article` is the root element  of the XML *XML* and should mandatory explicity the attributes of the :term:`DTD` version, the type of the document, the original language of the text, the :term:`namespace` declaration and the version of the :term:`Érudit PS` being used.

The attribute ``@xmlns:mml="http://www.w3.org/1998/Math/MathML"`` is optional and should be used only when a formula is defined using :term:`MathML`.

For the JATS ``@dtd-version`` it is necessary to define the version 1.1 of :term:`JATS` :term:`DTD`.

For the ``@article-type`` attribute the allowed values are:

+--------------------+----------------------------------------------------------+
| Value              | Description                                              |
+====================+==========================================================+
|                    | Commentary - A critique or explanatory article, written  |
| article-commentary | to discuss, support or debate a previous article or other| 
|                    | publication. It can be an article, letter, editorial,    |
|                    | etc. These publications can appear as a commentary,      |
|                    | editorial comment, point of view, etc.                   |
+--------------------+----------------------------------------------------------+
|                    | Review - Critical analysis of a book or other monographs.|
| book-review        |                                                          |
|                    |                                                          |
+--------------------+----------------------------------------------------------+
|                    | Brief communication - A brief report of research results.|
| brief-report       |                                                          |
|                    |                                                          |
+--------------------+----------------------------------------------------------+
|                    | Report, description or case study - Specific research    |
| case-report        | issue.                                                   |
|                    |                                                          |
+--------------------+----------------------------------------------------------+
|                    | Errata - Corrects errors in articles after they have been| 
| correction         | published online and/or in print.                        |
|                    |                                                          |
+--------------------+----------------------------------------------------------+
|                    | Editorial - A statement of the journal editor’s opinions,|
| editorial          | beliefs, and policies, usually on issues of interest to  |
|                    | the scientific community and society in general.         |
|                    |                                                          |
+--------------------+----------------------------------------------------------+
|                    | Press release - Comunicação breve de linguagem           |
| in-brief           | jornalística sobre um artigo ou tema.                    |
|                    |                                                          |
+--------------------+----------------------------------------------------------+
|                    | Letters - Written correspondence between persons or      |
| letter             | institutions, usually commenting on a published work.    |
+--------------------+----------------------------------------------------------+
|                    | Other type of document - It can be an addendum, annex,   |
| other              | discussion, article of concern, or introduction, amongst |
|                    | others.                                                  |
+--------------------+----------------------------------------------------------+
|                    | Retraction or rejection of a part of materials already   |
| partial-retraction | published.                                               |
|                    |                                                          |
+--------------------+----------------------------------------------------------+
|                    | Brief communication - Report updating research or other  |
| rapid-communication| news.                                                    |
|                    |                                                          |
+--------------------+----------------------------------------------------------+
|                    | Reply (a letter or commentary) - Generally done by the   |
| reply              | original author and contains additional comments to      |
|                    | others previously written.                               |
|                    |                                                          |
+--------------------+----------------------------------------------------------+
|                    | Original article - It covers research, clinical and      |
| research-article   | surgical experiments and/or other original works.        |
|                    |                                                          | 
+--------------------+----------------------------------------------------------+
|                    | Retraction (of a scientific article) - A vehicle for     |
| retraction         | correcting an academic work erroneously published, for   |
|                    | example, a work that was plagiarized.                    |
|                    |                                                          |
+--------------------+----------------------------------------------------------+
|                    | Reviews of the literature - Systematic reviews of the    |
| review-article     | literature on a particular subject.                      |
|                    |                                                          |
+--------------------+----------------------------------------------------------+


The text language in ``@xml:lang`` is described by the standard :term:`ISO 639-1` with a 2 digits code in lower case, for more information about the standard see `site <http://www.mathguide.de/info/tools/languagecode.html>`_.

The attribute ``@specific-use`` identifies the :term:`Érudit Publishing Schema` version.


Example `JATS versão 1.1 <http://jats.nlm.nih.gov/publishing/1.1/>`_:

.. code-block:: xml

     <article xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:mml="http://www.w3.org/1998/Math/MathML" dtd-version="1.1" specific-use="eps-0.1" article-type="research-article" xml:lang="pt">

           ...

    </article>

.. {"reviewed_on": "20180430", "by": "fabio.batalha@erudit.org"}