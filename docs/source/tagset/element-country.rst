.. _element-country:

<country>
=========

+-------------------------+-----------------+
| Appears in              | Frequency       |
+=========================+=================+
| :ref:`element-aff`      | Zero or once    |
+-------------------------+-----------------+
| :ref:`element-corresp`  | Zero or once    |
+-------------------------+-----------------+

Identifies the country in an address. It is not a mandatory element in affiliation.

The attribute @country is not mandatory, but when used it must be completed using the two letter uppercase country codes from the `ISO 3166 Standard <http://www.iso.org/iso/country_codes>`_.

Example:

.. code-block:: xml

   ...
   <aff id="aff01">
     ...
     <country country="CA">Canada</country>
      ...
   </aff>
   ...
