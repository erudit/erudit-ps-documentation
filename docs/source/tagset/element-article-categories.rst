.. _element-article-categories:

<article-categories>
====================

+------------------------------+--------------------+
| Appears in                   | Frequency          |
+==============================+====================+
| :ref:`element-article-meta`  | Zero or more times |
+------------------------------+--------------------+

Identifies the classification of the article according to the section in which it appears in the journal table of contents of an issue.

Examples:

    * :ref:`element-article-categories-example-1`
    * :ref:`element-article-categories-example-2`
    * :ref:`element-article-categories-example-3`

..note::

  There are no restrictions to create sub categories, but it is a best practice to not exceed 3 levels while defining the categories of the article in an issue.

.. _element-article-categories-example-1:

One level categorie:
--------------------

.. code-block:: xml

  ...
  <article-meta>
    ...
    <article-categories>
      <subj-group>
        <subject>Original Article</subject>
      </subj-group>
    </article-categories>
    ...
  </article-meta>
  ...

.. _element-article-categories-example-2:

Two levels categorie:
---------------------

.. code-block:: xml

  ...
  <article-meta>
    ...
    <article-categories>
      <subj-group>
        <subject>Original Article</subject>
        <subj-group>
          <subject>Level 2</subject>
        </subj-group>
      </subj-group>
    </article-categories>
    ...
  </article-meta>
  ...


.. _element-article-categories-example-3:

Tree levels categorie:
----------------------

.. code-block:: xml

  ...
  <article-meta>
    ...
    <article-categories>
      <subj-group>
        <subject>Original Article</subject>
        <subj-group>
          <subject>Level 2</subject>
          <subj-group>
            <subject>Level 2</subject>
          </subj-group>
        </subj-group>
      </subj-group>
    </article-categories>
    ...
  </article-meta>
  ...

.. {"reviewed_on": "20180523", "by": "fabio.batalha@erudit.org"}
