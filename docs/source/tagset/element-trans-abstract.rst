.. _element-trans-abstract:

<trans-abstract>
================

Mandatory attributes:

  1. ``@xml:lang``

+------------------------------+--------------------+
| Appears in                   | Frequency          |
+==============================+====================+
| :ref:`element-article-meta`  | Zero or more times |
+------------------------------+--------------------+
| :ref:`element-front-stub`    | Zero or more times |
+------------------------------+--------------------+

Contains the article translated abstract, if it exists, and displays simple or structured formats in the same way as element :ref:`element-abstract`. It should be inserted immediately after :ref:`element-abstract` and must have the attribute @xml:lang.

In ``<trans-abstract>``, label information should be inserted in element ``<title>``.

Examples:

    * :ref:`element-transabstract-example-1`
    * :ref:`element-transabstract-example-2`

.. _element-transabstract-example-1:

Example of structured ``<trans-abstract>``:
-------------------------------------------

The **Structured format** has groups of text arranged in sections identified with a title (For example: Introduction, Objectives, Methodology and Results).

Example:

.. code-block:: xml

    ...
    <article-meta>
        ...
        <trans-abstract xml:lang="en">
            <title>Abstract</title>
            <sec>
                <title>Objective</title>
                <p>To analyze the association between socioeconomic situation, clinical characteristics referred and the family history of cardiovascular disease, with the Self-perceived health of young adults education and their implications for clinical characteristics observed.</p>
            </sec>
            <sec>
                <title>Method</title>
                <p>Analytical study conducted with 501 young adults who are students in countryside city in the Brazilian Northeast. We used binary logistic regression.</p>
            </sec>
        </trans-abstract>
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
        <trans-abstract xml:lang="en">
            <title>Abstract</title>
            <p>In this paper we discuss the tutoring model adopted by the Public Institutions of Higher Education that integrate the Open University of Brazil (Universidade Aberta do Brasil - UAB) program. The starting point is the research and the actions developed by the authors in the past decade that are directly related to distance education in Brazil. The focus is on the classroom tutors who are responsible for assisting students in the presential center where they have support and who are selected through publishe.. notes in the virtual notice board of the institutions that offer higher education courses in a distinct mode of classroom teaching.</p>
        </trans-abstract>
        ...
    </article-meta>
    ...


.. {"reviewed_on": "20180509", "by": "fabio.batalha@erudit.org"}