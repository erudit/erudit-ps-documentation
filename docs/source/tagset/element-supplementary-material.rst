.. _element-supplementary-material:

<supplementary-material>
========================

Mandatory attributes:

  1. ``@id`` (ver :ref:`id-attribution-tips`)
  2. ``@xlink:href``
  3. ``@mimetype``
  4. ``@mime-subtype``

+-------------------------------+--------------------+
| Appears in                    | Frequency          |
+===============================+====================+
| ``app-group``                 | Zero or more times |
+-------------------------------+--------------------+
| :ref:`element-article-meta`   | Zero or more times |
+-------------------------------+--------------------+
| :ref:`element-body`           | Zero or more times |
+-------------------------------+--------------------+
| :ref:`element-boxed-text`     | Zero or more times |
+-------------------------------+--------------------+
| :ref:`element-disp-quote`     | Zero or more times |
+-------------------------------+--------------------+
| ``license-p``                 | Zero or more times |
+-------------------------------+--------------------+
| :ref:`element-p`              | Zero or more times |
+-------------------------------+--------------------+
| :ref:`element-ref-list`       | Zero or more times |
+-------------------------------+--------------------+
| :ref:`element-sec`            | Zero or more times |
+-------------------------------+--------------------+

Supplementary material is used to include information to an article, as example: multimedia objects, tables, figures, raw data, spreadsheets, etc.

* ``@id``: Used as unique identifier in the document.
* ``@mimetype``: Specifies the type of media, ex: "vídeo", "aplicação" etc.
* ``@mime-subtype``: Specifies the format of the media, ex: "mp4", "pdf" etc).
* ``@xlink:href``: Link for the file.

.. note:: 

 * At :ref:`elemento-front`, this element must be inserted after the paging information or before the element :ref:`elemento-history`.
 * At http://www.iana.org/assignments/media-types/media-types.xhtml, there is detailed information about the values for the attributes ``@mimetype`` e ``@mime-subtype``.

Examples:

 * :ref:`element-supplementary-material-example-1`
 * :ref:`element-supplementary-material-example-2`
 * :ref:`element-supplementary-material-example-3`
 * :ref:`element-supplementary-material-example-4`

.. _elemento-supplementary-material-exemplo-1:

Example of ``<supplementary-material>`` in ``<front>``
------------------------------------------------------

.. code-block:: xml

    ...
    <front>
        ...
        <article-meta>
            ...
            <fpage>237</fpage>
            <lpage>259</lpage>
            <supplementary-material id="suppl01" mimetype="application" mime-subtype="pdf" xlink:href="1234-5678-rctb-45-05-0110-suppl01.pdf"/>
            ...
        </article-meta>
        ...
    </front>
    ...



.. _element-supplementary-material-example-2:

Example of ``<supplementary-material>`` wrapping an object in ``<body>``
------------------------------------------------------------------------

.. code-block:: xml
    
    ...
    <body>
        ...
        <p>
            <supplementary-material id="suppl02" mimetype="image" mime-subtype="tiff" xlink:href="11234-5678-rctb-45-05-0110-suppl01.tif">
                <label>Fig 1.</label>
                <caption>
                    <title>Supplementary material A</title>
                </caption>
            </supplementary-material>
        </p>
        ...
    </body>
    ...

.. _element-supplementary-material-example-3:

Example of ``<supplementary-material>`` in ``<p>`` inside ``<body>``
---------------------------------------------------------------------

.. code-block:: xml
    
    ...
    <body>
        ...
        <p>
            <supplementary-material id="suppl03" mimetype="application" mime-subtype="pdf" xlink:href="1234-5678-rctb-45-05-0110-suppl01.pdf"/>
        </p>
      ...
    </body>
    ...

.. _elemento-supplementary-material-exemplo-4:

Example of ``<supplementary-material>`` in ``<back>``
-----------------------------------------------------

.. code-block:: xml
    
    ...
    <back>
        <app-group>
            <app id="app01">
                <label>S-1</label>
                <supplementary-material id="suppl04" mimetype="image" mime-subtype="tiff" xlink:href="11234-5678-rctb-45-05-0110-suppl01.tif">
                    <label>Fig 1.</label>
                    <caption>
                        <title>Supplementary material A</title>
                    </caption>
                </supplementary-material>
            </app>
            <app id="app02">
                <label>S-2</label>
                <supplementary-material id="suppl05" mimetype="image" mime-subtype="tiff" xlink:href="11234-5678-rctb-45-05-0110-suppl02.tif"/>
            </app>
        </app-group>
        ...
    </back>
    ...

.. {"reviewed_on": "20180622", "by": "fabio.batalha@erudit.org"}