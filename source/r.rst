.. _data_r:

How to load data into R
===========================

* `Order data <https://data.nextgis.com/en/>`_ for your area of interest in ESRI Shape format.
* Wait for email with download link, download and unpack archive with data.
* Select the layer you need.
* Install and load the rgdal package for R.

If you are using Windows, then to import data into R with correct attribute names instead of:

.. code-block:: r

   Districts <- readOGR(dsn ='KO/data/boundary-polygon-lvl6.shp')

use

.. code-block:: r

   Districts <- readOGR(dsn ='KO/data/boundary-polygon-lvl6.shp', use_iconv = TRUE, encoding = "UTF-8")
