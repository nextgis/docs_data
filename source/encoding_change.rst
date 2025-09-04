.. _data_encoding_change:

How to change data encoding
===========================

* `Order data <https://data.nextgis.com/en/>`_ for your area of interest, e.g. in GeoJSON format.
* Go to the `orders <https://data.nextgis.com/en/orders/actual/>`_ page and download the archive when it's complete.
* **Unpack** the archive.
* Import target layer, which encoding you want to change, in `QGIS <https://qgis.org/en/site/forusers/download.html>`_. 
* Right-click on a target layer in Layers Panel, select option “Save as…”. Thus you’ll create a copy of the layer, but in desired encoding.

.. figure:: _static/cs_change_select_save_en.png
   :name: encoding_change1
   :align: center
   :width: 24cm

* In the pop-up window select format "ESRI Shapefile" and the desired encoding (in this example - windows-1251), and also specify a name and a path to a new file. Press “OK”.

.. figure:: _static/encoding_change_en.png
   :name: encoding_change2
   :align: center
   :width: 11cm

* A new layer with the desired encoding will be created. 

.. figure:: _static/encoding_change_result_en.png
   :name: encoding_change3
   :align: center
   :width: 20cm
