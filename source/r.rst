.. _data_r:

How to load data in R
=====================

* `Order data <https://data.nextgis.com/en/>`_ for your area of interest in ESRI Shape format.
* Wait for an email with download link, download and unpack archive with data.
* Identify a layer you need.
* Install and load the rgdal package for R.

If you are on Windows and attributes are garbled instead of:

.. code-block:: r

   Districts <- readOGR(dsn ='KO/data/boundary-polygon-lvl6.shp')

use

.. code-block:: r

   Districts <- readOGR(dsn ='KO/data/boundary-polygon-lvl6.shp', use_iconv = TRUE, encoding = "UTF-8")
