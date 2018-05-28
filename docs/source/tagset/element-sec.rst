.. _element-sec:

<sec>
=====

+--------------------------------+--------------------+
| Appears in                     | Frequency          |
+================================+====================+
| :ref:`element-body`            | Zero or more times |
+--------------------------------+--------------------+
| :ref:`element-sec`             | Zero or more times |
+--------------------------------+--------------------+
| :ref:`element-abstract`        | Zero or more times |
+--------------------------------+--------------------+
| :ref:`element-trans-abstract`  | Zero or more times |
+--------------------------------+--------------------+
| :ref:`element-boxed-text`      | Zero or more times |
+--------------------------------+--------------------+

The body of an article usually consists of sections. Each one has a ``<label>`` element followed by one or more paragraphs (:ref:`element-p`).

First level sections headings which match the list of values below should have attribute ``@sec-type``. This attribute should not be inserted if the first-level section has a name different from those which appear in the table below.

.. note::

  The element ``<title>`` is not mandatory but it is recommended that all sections have an element ``<title>`` inside.

+------------------------+------------------------------------------------+
| Value                  | Description                                    |
+========================+================================================+
| cases                  | reports/case studies                           |
+------------------------+------------------------------------------------+
| conclusions            | conclusions/final considerations/final Remarks |
+------------------------+------------------------------------------------+
| discussion             | discussions                                    |
+------------------------+------------------------------------------------+
| intro                  | introduction/synopsis                          |
+------------------------+------------------------------------------------+
| materials              | materiais                                      |
+------------------------+------------------------------------------------+
| methods                | methodology/method                             |
+------------------------+------------------------------------------------+
| results                | results                                        |
+------------------------+------------------------------------------------+
| supplementary-material | supplementary-material                         |
+------------------------+------------------------------------------------+

Examples:

  * :ref:`element-sec-example-1`
  * :ref:`element-sec-example-2`
  * :ref:`element-sec-example-3`
  * :ref:`element-sec-example-4`

.. _element-sec-example-1:

Example a simple ``<sec>``:
---------------------------

.. code-block:: xml

  ...
  <body>
    ...
    <sec sec-type="intro">
      <label>1<label>
      <title>Introduction</title>
      <p>Central airway obstruction (CAO) is a pathological process that leads to airflow limitation at the level of the glottis, subglottis, trachea, and main bronchi. Correct diagnosis and treatment of CAO is an area of interest and concern for health professionals,given that this disease has the potential to cause significant morbidity and mortality.</p>
      ...
    </sec>
    ...
  </body>
  ...


.. _element-sec-example-2:

Example of ``<sec>`` with combined @sec-type:
---------------------------------------------

In the case of combined sections, in other words, when the section heading is made up of more than one of the items from the above table, the value of attribute ``@sec-type`` should correspond to each item, respectively, separated by a | (pipe).

.. code-block:: xml

  ...
  <body>
    ...
    <sec sec-type="materials|methods">
      <label>1<label>
      <title>Materials and Methods</title>
      <p>Between November of 2009 and April of 2010, we conducted a prospective, observational, cross-sectional study. The target population consisted of patients for whom bronchoscopy was clinically indicated. The patients were consecutively selected for the sample on the...</p>
      ...
    </sec>
    ...
  </body>
  ...

.. _element-sec-example-3:

Example of sub-section:
-----------------------

Sections may have one or more subsections. In such cases, each subsection should be marked with element ``<sec>`` within the top-level section.

.. code-block:: xml

  ...
  <body>
    ...
    <sec sec-type="methods">
      <label>1<label>
      <title>Methodology</title>
      <sec>
        <label>1.1<label>
        <title>Methodology in Science</title>
        <p>Each patient underwent a brief physical examination, and the degree of dyspnea was determined by the Medical Research Council (MRC) 5-point scale.</p>
        ...
      </sec>
    </sec>
    ...
  </body>
  ...

.. _element-sec-example-4:

Example of ``<sec>`` without @sec-type:
---------------------------------------

Sections with a non-standard name can be declared without the attribute ``@sec-type``.

.. code-block:: xml

  ...
  <body>
    ...
    <sec>
      <label>1<label>
      <title>Biologia Marinha</title>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi pharetra lacinia orci at adipiscing.</p>
      ...
    <sec>
    ...
  </body>
  ...

.. {"reviewed_on": "20180528", "by": "fabio.batalha@erudit.org"}