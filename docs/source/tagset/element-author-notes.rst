.. _element-author-notes:

<author-notes>
==============

+------------------------------+--------------------+
| Appears in                   | Frequency          |
+==============================+====================+
| :ref:`element-article-meta`  | Zero or more times |
+------------------------------+--------------------+
| :ref:`element-front-stub`    | Zero or more times |
+------------------------------+--------------------+

Identifies notes related to the author such as correspondence, equal contribution, etc.

Exemplo:

.. code-block:: xml

    ...
    <article-meta>
        ...
        <author-notes>
            <corresp id="c01"><bold>Correspondence:</bold> Address for correspondence <email>user@foo.com</email></corresp>
            <fn fn-type="conflict">
                <p>Conflict of interest: none</p>
            </fn>
        </author-notes>
        ...
    </article-meta>
    ...


.. {"reviewed_on": "20180524", "by": "fabio.batalha@erudit.org"}
