Special Charset Encoding
========================

The :term:`Érudit PS` requires that the :term:`XML` documents must be encoded as :term:`UTF-8`, and they must have it's enconding explicity identified at the :term:`XML Declaration`.

   ``<?xml version="1.0" encoding="utf-8"?>``


The special characters, must be writen as is in the document or using it's hexadecimal numeric reference. As example, the character sigma uperscript should be represented by ``Σ`` or ``&#x03A3;``.

.. note:: *Érudit PS* recomend the use of the original characters besides the haxadecimal notation.

It is not allowed the use of any private character reference of the ASCII definition. They are the :term:`Unicode` within the iterval of ``xE000 – xF8FF``.

:term:`XML` entities are also accepted and must be used to represent the desired character:

+-----------+----------+
| Character | Entity   |
+===========+==========+
| "         | &quot;   |
+-----------+----------+
| '         | &apos;   |
+-----------+----------+
| &         | &amp;    |
+-----------+----------+
| <         | &lt;     |
+-----------+----------+
| >         | &gt;     |
+-----------+----------+

For more information see `Unicode table <http://unicode-table.com/en/>`_.

.. {"reviewed_on": "20180422", "by": "fabio.batalha@erudit.org"}
