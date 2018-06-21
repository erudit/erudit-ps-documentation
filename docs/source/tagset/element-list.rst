.. _element-list:

<list>
======

Mandatory attribute:

  1. ``@list-type``

+----------------------------+--------------------+
| Appears in                 | Frequency          |
+============================+====================+
| :ref:`element-body`        | Zero or more times |
+----------------------------+--------------------+
| :ref:`element-boxed-text`  | Zero or more times |
+----------------------------+--------------------+
| :ref:`element-disp-quote`  | Zero or more times |
+----------------------------+--------------------+
| ``<list-item>``            | Zero or more times |
+----------------------------+--------------------+
| :ref:`element-p`           | Zero or more times |
+----------------------------+--------------------+
| :ref:`element-sec`         | Zero or more times |
+----------------------------+--------------------+

Element used to identify one list that contains one or more itens. I could have an optional element ``<title>`` or a element :ref:`element-label`.

The attribute ``@list-type`` specifies the prefix to be used in the list. The allowed values are:

+----------------+-------------------------------------------------------------------+
| Value          | Description                                                       |
+================+===================================================================+
| order          | Ordered list which prefix is a number                             |
+----------------+-------------------------------------------------------------------+
| bullet         | Unordered list, which prefix is a bullet (circle)                 |
+----------------+-------------------------------------------------------------------+
| alpha          | Ordered list which prefix is a alpha character                    |
+----------------+-------------------------------------------------------------------+
| roman          | Ordered list which prefix is a roman number                       |
+----------------+-------------------------------------------------------------------+
| simple         | Unordered list without a prefix                                   |
+----------------+-------------------------------------------------------------------+


Examples:

  * :ref:`element-list-example-1`
  * :ref:`element-list-example-2`
  * :ref:`element-list-example-3`



.. _element-list-example-1:

Example of a ordered list:
--------------------------


Donec rhoncus

1. Nullam gravida tellus eget condimentum egestas.
2. Donec pulvinar odio ut enim lobortis, eu dignissim elit accumsan.
3. Vestibulum urna elit, auctor ac fringilla ac, sagittis in ex.

.. code-block:: xml

  ...
  <list list-type="order">
    <title>Donec rhoncus</title>
      <list-item>
        <p>Nullam gravida tellus eget condimentum egestas.</p>
      </list-item>
      <list-item>
        <p>Donec pulvinar odio ut enim lobortis, eu dignissim elit accumsan.</p>
      </list-item>
      <list-item>
        <p>Vestibulum urna elit, auctor ac fringilla ac, sagittis in ex.</p>
      </list-item>
  </list>
  ...


.. _element-list-example-2:

Example of an ordered list with sub-itens:
------------------------------------------


Vivamus cursus

1. Nullam gravida tellus eget condimentum egestas.
    1.1. Curabitur luctus lorem ac feugiat pretium.  
2. Donec pulvinar odio ut enim lobortis, eu dignissim elit accumsan.

.. code-block:: xml

  ...
  <list list-type="order">
    <title>Vivamus cursus</title>
      <list-item>
        <p>Nullam gravida tellus eget condimentum egestas.</p>
          <list list-type="order">
            <list-item>
              <p>Curabitur luctus lorem ac feugiat pretium.</p>
            </list-item>
          </list>
      </list-item>
      <list-item>
        <p>Donec pulvinar odio ut enim lobortis, eu dignissim elit accumsan.</p>
      </list-item>
  </list>
  ...

.. _element-list-example-3:


Example of an unordered list with bullets:
------------------------------------------

Nam commodo

* Morbi luctus elit enim.
* Nullam nunc leo.
* Proin id dui lorem.
* Nunc finibus risus.

.. code-block:: xml

  ...
  <list list-type="bullet">
    <title>Nam commodo</title>
      <list-item>
        <p>Morbi luctus elit enim.</p>
      </list-item>
      <list-item>
        <p>Nullam nunc leo.</p>
      </list-item>
      <list-item>
        <p>Proin id dui lorem.</p>
      </list-item>
      <list-item>
        <p>Nunc finibus risus.</p>
      </list-item>
  </list>
  ...

.. {"reviewed_on": "20180422", "by": "fabio.batalha@erudit.org"}