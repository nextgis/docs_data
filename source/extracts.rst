NextGIS Data extracts
====================================================

.. _ngdata_structure:

How the files are organized
------------------------------

When you order data on `NextGIS Data <https://data.nextgis.com/en/>`_, you get a ZIP archive that need to be unpacked before use. The name of the archive includes the date of the extract, its format and the code of the region (or "custom" if you selected your own area).

The archive unpacks to a folder containing the following files and subfolders. 

All extracts include:

* Boundary of the selected area ``order_boundary.geojson``.

* Folder called ``data``. It contains data layers and styles as well the data boundary in the selected format.

* A text file that has information on copyright and licencing, ``readme.txt``.

Depending on the data type and format the extracts may also contain:

* Project file for QGIS `data.qgs``, ArcMap ``data.mxd``, ArcGIS Pro ``data.aprx``  or Mapinfо ``data.wor``. Double-click on it to open in the corresponding software. All layers are already added to the project and stylized. 

   * QGIS projects are included for all products, if you select **Geopackage, Shape or GeoJSON** format.
   * Projects for ArcMap and ArcGIS Pro are available for all projects if you select  **Geodatabase or Shape** format.
   * Project for MapInfo is available only for the Basemap if you select **Mapinfo TAB** format.

* Folder containg icons, ``svg``. Some styles use vector markers in SVG format. This folder need to be next to the project for the style to work.



.. _ngdata_attr_osm:

Attributes in OpenStreetMap extracts
-------------------------------------------

Usually GIS data is organized into layers, each with its specific geometry type and a set of attributes. OpenStreetMap project organizes data differently. It's one big database containing interlinked geometries. Each feature has tags in the form of key-value pairs. Contributors can invent new keys, but the standard ones are described on wiki.openstreetmap.org. In NextGIS Data extracts the features are split into layers with the most important attributes.

* `List of attributes with descriptions <https://docs.google.com/spreadsheets/d/e/2PACX-1vRIUla6YhWLBPCfKZ6ldWZ_xAO7lc-DtHcS6_MI4knV1RgWgkfm0MOKaQJXHQ1Cnxg8UDl0hXpt4Eqk/pubhtml>`_  

* For the details of OSM tags see `OpenStreetMap wiki <https://wiki.openstreetmap.org/wiki/Map_features>`_

.. _ngdata_attr_other:

Attributes of other products
-----------------------------------

* `Elevation <https://docs.google.com/spreadsheets/d/1PRSpeLWrFttCS7tz8rk--R7aoV_B8LuGbDuUbhLyWJg/pubhtml>`_
* `Buildings AI <https://docs.google.com/spreadsheets/d/e/2PACX-1vRgaXygAc2KXQp-nGK2t8KcBYqCb6cttxCO6UzUkIdSafVxQmxhUBrGIV3pLjCMi64Ys0_tAwa61ZAy/pubhtml>`_
* `Roads AI <https://docs.google.com/spreadsheets/d/e/2PACX-1vT6LtVjaJy8GAOwBGFGqjL5NX0meddQbwG0qtiZuqBPMmDsjLAxYWM4ARzFDegb2UG2vhlHaLefOP2s/pubhtml>`_
* `Overture <https://docs.google.com/spreadsheets/d/e/2PACX-1vS2K6m2aTT-CRLZJROrAcsnBAcDPEcWJkxdh9l1dbSxpkSQ3UzusYRixNfCL8v74tXB7DFYjxltRInP/pubhtml?gid=0&single=true>`_
* `Places <https://docs.google.com/spreadsheets/d/e/2PACX-1vTPDiDiyf4nrfY-8cER2qyzjolFPDeOo_a2qa1ZICCr8XtH5Ba4cfKb2NZd2UB9S3zbiSzOmWK6dNDw/pubhtml?gid=125713722&single=true>`_
* `Landcover <https://docs.google.com/spreadsheets/d/e/2PACX-1vR9Uf9DzxXdxHH6h0lUnFd27bRNN6bRnsVpuVRPRnFTmIEnELZVGTAFXdtAg68zpUshCC2l1bi7F2tg/pubhtml>`_
* `Heritage <https://docs.google.com/spreadsheets/d/e/2PACX-1vTC_wgWY28Y3QjgvJ-Q8Jmu6Doxxhpz-Hm_b3JwEjqcpk8bpQmRJq6ldwgZoHWbWxk-FC2Wi0nyjXnY/pubhtml>`_
* `Satellite <https://data.nextgis.com/en/region/custom/sat/?format=geotiff>`_ - three-band RGB raster, not other attributes 
* `Tiles <https://data.nextgis.com/en/region/custom/tiles/>`_ - no attributes
* `Printable map <https://data.nextgis.com/en/region/custom/printmap/>`_ - no attributes, the legend is included
