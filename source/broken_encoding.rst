.. _data_broken_encoding:

What if text in attribute table is garbled…
===========================

.. figure:: _static/broken_encoding1.png
   :name: broken_encoding1
   :align: center
   :width: 16cm

* It is recommended to ensure that your GIS doesn’t ignore layer encoding information. For `NextGIS QGIS <https://nextgis.com/nextgis-qgis/>`_ it can be checked via “Settings” > “Options” > “Data Sources”. If the box with “Ignore shapefile encoding declaration” is checked, uncheck it.

.. figure:: _static/broken_encoding2.png
   :name: broken_encoding2
   :align: center
   :width: 16cm

* It can be also helpful to check, does encoding of “problematic” layer correspond to initial encoding. Possible initial encodings are listed `here <https://data.nextgis.com/en/about/#formats>`_ and depend on format of your ordered data. Encoding of the layer is shown in its “Properties” menu.

.. figure:: _static/broken_encoding3.png
   :name: broken_encoding3
   :align: center
   :width: 16cm

