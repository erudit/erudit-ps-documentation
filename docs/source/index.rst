.. Erudit Publishing Schema Documentation documentation master file, created by
   sphinx-quickstart on Fri Apr 20 11:03:27 2018.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to Érudit Publishing Schema Documentation
=================================================

Version 0.1 (Beta) - March 2018. 

.. toctree::
   :maxdepth: 1
   :caption: Contents:


Introductions
-------------

This guide describes how to use the Markup Style designed by *Érudit* for the submission of documents in :term:`XML` format.

The :term:`Érudit Publishing Schema` (:term:`Érudit PS`) is compounded by the following specifications:

* :term:`NISO JATS Journal Publishing DTD` (JATS version `1.1 <http://jats.nlm.nih.gov/publishing/1.1/>`);
* :term:`Érudit PS Style` containing specialized validations to address Érudit needs.

The users of this guide must have mastered :term:`XML` and :term:`DTD`.


Support Tools
-------------

Some tools are being maintained by *SciELO* and *Érudit* following :term:`open source` polices, to support the process of evaluation of documents in the *XML* format.


 `Packtools <https://github.com/scieloorg/packtools/>`_:
     A :term:`Python` Library with tools to evaluate documents in XMLs format against validations specified by a Packtooks Catalog Plugin.

 `Érudit Packtools Catalog <https://gitlab.erudit.org/erudit/production/erudit-ps-packtools-plugin>`_:
     A :term:`Packtools Catalog Plugin` developed to address the Érudit requirements in the validation of :term:`XML` documents. This plugin implements the validations specified by the :term:`Érudit PS`.

General Info
------------

.. toctree::
   :maxdepth: 2

   special_characters
   glossary

Elements List
-------------

This list represents only the :term:`XML` elements of the :term:`Érudit PS`. The complete list of :term:`XML` elements of the JATS :term:`tag set` is available at `JATS 1.1 <http://jats.nlm.nih.gov/publishing/1.1/>`_.

.. toctree::
   :maxdepth: 1

   tagset/xml-encoding
   tagset/xml-doctype
   tagset/id-attribution-tips
   tagset/compatibility-reference


.. toctree::
   :maxdepth: 1
   :glob:

   tagset/element-*


Indexes and tables
==================

* :ref:`genindex`
* :ref:`search`

.. toctree::
   :hidden:

   copyright

.. {"reviewed_on": "20180422", "by": "fabio.batalha@erudit.org"}
