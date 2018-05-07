.. _elemento-app:

<app>
=====

Mandatory attributes:

  1. ``@id`` (See :ref:`id-attribution-tips`)

+-----------------+--------------------+
| Appears in      | Frenquency         |
+=================+====================+
| ``<app-group>`` | Zero or more times |
+-----------------+--------------------+

Used to indicate an appendix to the document. The element :ref:`label` or :ref:`title` could be present to describe the title of the appendix. The element :ref:`app-group` must always be used to group the ``<app>`` element even if there is only one occurrence of it.

.. note::

  According to JATS rules, one of :ref:`label` or :ref:`title` should be available in ``<app>``

Examples:

  * :ref:`element-app-example-1`
  * :ref:`element-app-example-2`
  * :ref:`element-app-example-3`
  * :ref:`element-app-example-4`
  * :ref:`element-app-example-5`
  * :ref:`element-app-example-6`


.. _element-app-example-1:

Example of an appendix with text
--------------------------------

.. code-block:: xml

    ...
    <app-group>
          <app id="app01">
              <label>Appendix</label>
              <p>Vivamus fermentum elit et pellentesque iaculis. Curabitur egestas rhoncus purus quis iaculis. Sed laoreet id leo eu tristique. Etiam hendrerit nibh in tincidunt mattis. Sed et volutpat nulla, eget semper tellus. Nullam imperdiet fringilla diam, nec mollis elit sagittis a. Nam euismod sagittis posuere.</p>
          </app>
    </app-group>
    ...

.. _element-app-example-2:

Example of an appendix with an image (photograph, figure, table, painting, equation, etc)
-----------------------------------------------------------------------------------------

.. code-block:: xml

    ...
    <app-group>
        <app id="app01">
              <label>Appendix 1</label>
              <title>Picture of a square</title>
              <graphic xlink:href="square.tif"/>
        </app>
    </app-group>
    ...


.. _element-app-example-3:

Example of an appendix with an external link
--------------------------------------------

.. code-block:: xml

    ...
    <app-group>
        <app id="app01">
            <label>Appendix 1</label>
            <p>For more information, see <ext-link ext-link-type="uri" xlink:href="http://www.erudit.org">click here</ext-link>.</p>
        </app>
    </app-group>
    ...


.. _element-app-example-4:

Example of an appendix with a table
-----------------------------------

.. code-block:: xml

    ...
    <app-group>
      <app id="app01">
      <label>Appendix</label>
            <table-wrap>
              <label>Table 1</label>
              <caption>
                  <title>Table Title</title>
              </caption>
              <table frame="hsides" rules="all">
                  <colgroup width="XX%">
                      <col/>
                      <col/>
                      <col/>
                  </colgroup>
                  <thead>
                      <tr>
                           <th style="background-color:#e5e5e5">xxxxx</th>
                           <th style="background-color:#e5e5e5">xxxxx</th>
                           <th style="background-color:#e5e5e5">xxxxxx</th>
                      </tr>
                  </thead>
                  <tbody>
                      <tr>
                           <td align="center">xxxxx</td>
                           <td align="center">xxxx</td>
                           <td align="center">xxxx</td>
                      </tr>
                  </tbody>
              </table>
            </table-wrap>
      </app>
    </app-group>
    ...


.. _element-app-example-5:

Example of an appendix with mixed content (figure and table)
------------------------------------------------------------

.. code-block:: xml

    ...
    <app-group>
        <app id="app01">
            <label>Appendix 1</label>
            <title>Picture of a square</title>
            <graphic xlink:href="square.tif"/>
        </app>
        <app id="app02">
            <label>Appendix 2</label>
            <table-wrap>
                <label>Supplementary Table S1</label>
                <caption>
                    <title>Table Title</title>
                </caption>
                <table frame="hsides" rules="all">
                    <colgroup width="XX%">
                        <col/>
                        <col/>
                        <col/>
                    </colgroup>
                    <thead>
                        <tr>
                            <th style="background-color:#e5e5e5">xxxxx</th>
                            <th style="background-color:#e5e5e5">xxxxx</th>
                            <th style="background-color:#e5e5e5">xxxxxx</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td align="center">xxxxx</td>
                            <td align="center">xxxx</td>
                            <td align="center">xxxx</td>
                        </tr>
                    </tbody>
                </table>
            </table-wrap>
        </app>
    </app-group>
    ...

.. _element-app-example-6:

Example of an appendix with a video
-----------------------------------

.. code-block:: xml

    ...
    <app-group>
          <app id="app01">
              <label>Appendix 1</label>
              <supplementary-material id="suppl01">
              <media xlink:href="video.avi" mimetype="video" mime-subtype="avi"/>
              </supplementary-material>
          </app>
    </app-group>
    ...


.. {"reviewed_on": "20180504", "by": "fabio.batalha@erudit.org"}