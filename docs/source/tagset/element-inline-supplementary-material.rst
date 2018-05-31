.. _element-inline-supplementary-material:

<inline-supplementary-material>
===============================

Mandatory attributes:

  1. ``@xlink:href``
  2. ``@mimetype``
  3. ``@mime-subtype``

+------------------------------+--------------------+
| Appears in                   | Frequency          |
+==============================+====================+
| :ref:`element-article-meta`  | Zero or more times |
+------------------------------+--------------------+
| :ref:`element-p`             | Zero or more times |
+------------------------------+--------------------+
| :ref:`element-app`           | Zero or more times |
+------------------------------+--------------------+

The element ``<inline-supplementary-material>`` is used to include information in a paragraph of the document, supplying a link to multimedia files, tables or aditional figures, lists, raw data in spreadsheets, etc.

The mandatory attributes are:

* ``@mimetype:``: Specifies the type of media, such as “video” and “application”, among others.
* ``@mime-subtype``: Identifies the media format, as example, "mp4", "pdf" etc.
* ``@xlink:href``: Contains the complete name of the media file, for example file.pdf”, file.mp4”, “file.mp3” etc.

.. note:: 
 * See the address http://www.iana.org/assignments/media-types/media-types.xhtml for detailed information about the values for the attributes ``@mimetype`` and ``@mime-subtype``.

 Examples:

  * :ref:`element-inlinesm-exemplo-1`
  * :ref:`element-inlinesm-exemplo-2`

.. _element-inlinesm-example-1:

Example of <inline-supplementary-material> wrapping a text:
-----------------------------------------------------------

.. code-block:: xml

    <p>Text of supplementary material... <inline-supplementary-material xlink:href="0103-507X-rbti-26-02-0130-suppl1.pdf" mimetype="application" mime-subtype="pdf">Supplementary Material Suplementar</inline-supplementary-material></p>
    

.. _element-inlinesm-example-2:

Example of <inline-supplementary-material> without a text:
----------------------------------------------------------

.. code-block:: xml

    <p>Nunc faucibus orci ut bibendum mollis. Nunc rutrum ullamcorper neque sit amet venenatis. Praesent mattis <inline-supplementary-material xlink:href="0103-507X-rbti-26-02-0130-suppl1.pdf" mimetype="video" mime-subtype="avi"/> elit id augue tincidunt, sit amet ornare nibh laoreet. Morbi et odio a libero facilisis dapibus id vitae orci.</p>
