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

Contains the article translated abstract, if it exists, and displays simple or structured formats in the same way as element :ref:`element-abstract`. It should be inserted immediately after :ref:`element-abstract` and must have the attribute @xml:lang.

In ``<trans-abstract>``, label information should be inserted in element ``<title>``.

Examples:

    * :ref:`element-transabstract-example-1`
    * :ref:`element-transabstract-example-2`

.. _element-transabstract-example-1:

Example of structured ``<trans-abstract>``:
-------------------------------------------

The **Structured** format has groups of text arranged in sections identified with a title (For example: Introduction, Objectives, Methodology and Results).

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
        <p>This article analyses the language ideological debate surrounding the relationship between the future of the Canadian Francophonie, the quality of the language, and the duty of young people to preserve it. The idea that young people in particular are responsible for the deterioration of a language is part of an old and recurring discourse. We examine its resurgence between the fall of 2012 and the spring of 2013 in Acadie, as seen in media texts that share strong argumentative similarities. Through a critical approach, we show that the positions staked out in this debate draw their legitimacy and authority from the ideological foundations of modern political nationalism, which construe language as the central feature of identity and language proficiency as a skill that is accessible to all.</p>
      </trans-abstract>
      ...
    </article-meta>
    ...


.. {"reviewed_on": "20180509", "by": "fabio.batalha@erudit.org"}