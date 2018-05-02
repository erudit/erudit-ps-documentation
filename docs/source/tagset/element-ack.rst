.. _element-ack:

<ack>
=====

+----------------------+--------------------+
| Appears in           | Frequency          |
+======================+====================+
| :ref:`element-back`  | Zero or more times |
+----------------------+--------------------+


The Acknowledgements section.

In the case it has a title, (e.g. “Acknowledgments” ) identify it in ``<title>``. The element :ref:`element-p` is used to identify paragraphs of text.

.. note:: The element :ref:`element-sec` must not be used inside the ``ack`` element.

Example:

.. code-block:: xml

    ...
    <back>
        <ack>
            <title>Remerciement</title>
            <p>Texte de remerciement.</p>
        </ack>
    </back>
    ...

.. {"reviewed_on": "20180502", "by": "fabio.batalha@erudit.org"}
