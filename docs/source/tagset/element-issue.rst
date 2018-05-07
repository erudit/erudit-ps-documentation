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

Exemplo de número em um fascíulo:
---------------------------------

Refere-se ao fascículo: volume 56, número 4 (v56n4)


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



.. _elemento-issue-exemplo-2:

Exemplo 1:  suplemento de número:
---------------------------------

Refere-se ao fascículo: volume 10, número 4, suplemento (v10n4s0)


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



.. _elemento-issue-exemplo-3:

Exemplo 2: suplemento de número:
--------------------------------
Refere-se ao fascículo: volume 10, número 4, suplemento 2 (v10n4s2)


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



.. _elemento-issue-exemplo-4:

Exemplo 1: suplemento de volume:
--------------------------------

Refere-se ao fascículo: volume 54, suplemento (v54s0)

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


.. _elemento-issue-exemplo-5:

Exemplo 2: suplemento de volume:
--------------------------------

Refere-se ao fascículo: volume 54, suplemento 1 (v54s1)

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

.. _elemento-issue-exemplo-6:

Exemplo 1: número especial
---------------------------

Refere-se ao fascículo: volume 25, número especial (v25nspe)

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


.. _elemento-issue-exemplo-7:

Exemplo 2: número especial
---------------------------

Refere-se ao fascículo: volume 25, número especial 2 (v25nspe2)

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


.. _elemento-issue-exemplo-8:

Exemplo de número em <element-citation>:
----------------------------------------

Refere-se a um número em uma referência

.. code-block:: xml


    ...
    <ref id="B01">
        ...
        <source>SciELO Journal</source>
        <volume>16</volume>
        <issue>3</issue>
        ...
    </ref>
    ...


.. note:: Se o periódico publicar mais de um suplemento ou número especial por ano, recomenda-se publicar informando a numeração do suplemento ou número especial (exemplos 2). Se apenas publicar um ao ano, não informe numeração no suplemento ou número especial (exemplos 1).