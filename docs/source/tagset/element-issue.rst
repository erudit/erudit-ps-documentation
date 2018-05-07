.. _element-issue:

<issue>
=======

+----------------------------------+--------------------+
| Appears in                       | Frequency          |
+==================================+====================+
| :ref:`element-article-meta`      | Zero or more times |
+----------------------------------+--------------------+
| :ref:`element-element-citation`  | Zero or more times |
+----------------------------------+--------------------+

Identifies the issue (or supplement to it), either as part of a volume or as a special issue

Examples:

  * :ref:`element-issue-example-1`
  * :ref:`element-issue-example-2`
  * :ref:`element-issue-example-3`
  * :ref:`element-issue-example-4`
  * :ref:`element-issue-example-5`
  * :ref:`element-issue-example-6`
  * :ref:`element-issue-example-7`
  * :ref:`element-issue-example-8`



.. _element-issue-example-1:

Example of a issue number:
--------------------------

Refers to the issue: volume 56, número 4


.. code-block:: xml

    ...
    <front>
        ...
        <article-meta>
            ...
            <volume>56</volume>
            <issue>4</issue>
            ...
        </article-meta>
        ...
    </front>
    ...



.. _element-issue-example-2:

Example of supplement of number:
--------------------------------

Refers to: volume 10, número 4, supplement


.. code-block:: xml

    ...
    <front>
        ...
        <article-meta>
            ...
            <volume>10</volume>
            <issue>4 suppl</issue>
            ...
        </article-meta>
        ...
    </front>
    ...



.. _element-issue-example-3:

Example of supplent of number:
------------------------------

Refers to the issue: volume 10, número 4, supplement 2


.. code-block:: xml

    ...
    <front>
        ...
        <article-meta>
            ...
            <volume>10</volume>
            <issue>4 suppl 2</issue>
            ...
        </article-meta>
        ...
    </front>
    ...



.. _element-issue-example-4:

Example of supplement of volume:
--------------------------------

Refers to the issue: volume 54, supplement

.. code-block:: xml

    ...
    <front>
        ...
        <article-meta>
            ...
            <volume>54</volume>
            <issue>suppl</issue>
            ...
        </article-meta>
        ...
    </front>
    ...


.. _element-issue-example-5:

Example of supplement of volume:
--------------------------------

Refers to the issue: volume 54, supplement 1

.. code-block:: xml

    ...
    <front>
        ...
        <article-meta>
            ...
            <volume>54</volume>
            <issue>suppl 1</issue>
            ...
        </article-meta>
        ...
    </front>
    ...

.. _element-issue-example-6:

Example of special number
-------------------------

Refers to the issue: volume 25, número especial

.. code-block:: xml

    ...
    <front>
        ...
        <article-meta>
            ...
            <volume>25</volume>
            <issue>spe</issue>
            ...
        </article-meta>
        ...
    </front>
    ...


.. _element-issue-example-7:

Example of special number
-------------------------

Refers to the issue: volume 25, número especial 2

.. code-block:: xml

    ...
    <front>
        ...
        <article-meta>
            ...
            <volume>25</volume>
            <issue>spe2</issue>
            ...
        </article-meta>
        ...
    </front>
    ...


.. _element-issue-example-8:

Example of issue in :ter:`element-citation`:
---------------------------------------

Refere-se a um número em uma referência

.. code-block:: xml


    ...
    <ref id="B01">
        ...
        <source>Journal Title</source>
        <volume>16</volume>
        <issue>3</issue>
        ...
    </ref>
    ...