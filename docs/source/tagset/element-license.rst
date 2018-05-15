.. _element-license:

<license>
=========

Mandatory attributes:

  1. ``@xml:lang``

+-----------------------------+-------------------+
| Appears in                  | Frequency         |
+=============================+===================+
| :ref:`element-permissions`  | One or more times |
+-----------------------------+-------------------+

Indicates the URL of the license text which governs the use of the article. Each type of license defines the rules governing the use, distribution, and adaptation of the work.

The value for ``@xml:lang`` should correspond to the language of the license text defined by the element ``<license-p>``. There must be a ``<license-p>`` for the original language of the article, or in English.

Example:

.. code-block:: xml

    ...
    <article-meta>
        ...
        <permissions>
            ...
            <license xlink:href="http://creativecommons.org/licenses/by/4.0/"
                     xml:lang="en">
                <license-p>This is an open-access article distributed under the terms of the Creative Commons Attribution License, which permits unrestricted use, distribution, and reproduction in any medium, provided the original work is properly cited.</license-p>
            </license>
            <license xlink:href="http://creativecommons.org/licenses/by/4.0/"
                     xml:lang="pt">
                <license-p>Este artigo está licenciado com uma Licença Creative Commons que permite uso irrestrito, distribuição, e reprodução em qualquer mídia, desde que a obra original seja citada adequadamente.</license-p>
            </license>
            <license xlink:href="http://creativecommons.org/licenses/by/4.0/"
                     xml:lang="es">
                <license-p>Este es un artículo de acceso abierto distribuido bajo los términos de la licencia Creative Commons Attribution License, que permite el uso ilimitado, distribución y reproducción en cualquier medio, siempre que el artículo original esté debidamente citado.</license-p>
            </license>
        </permissions>
        ...
    </article-meta>
    ...


.. {"reviewed_on": "20180515", "by": "fabio.batalha@erudit.org"}