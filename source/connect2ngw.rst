.. _data_connect_to_ngw:

How to upload data to NextGIS Web with NextGIS Connect
======================================================

* `Order data <https://data.nextgis.com/en/>`_ for your area of interest in Geopackage format (QGIS).
* Go to the `orders <https://data.nextgis.com/en/orders/actual/>`_ page and download the archive when it's complete. 
* **Unpack** the archive.
* Download and install `QGIS <https://qgis.org/en/site/forusers/download.html>`_.
* Launch QGIS.
* Drag the project file "data_reseding.qgs" into QGIS window.

The project is loaded in QGIS.

.. figure:: _static/open_project_qgis_drag_en.png
   :name: open_map1
   :align: center
   :width: 20cm
   
* Install **NextGIS Connect** plugin (top menu Plugins - Manage and install plugins - enter *NextGIS Connect* in the search bar - Install). 

* NextGIS Connect panel will appear. You can also call this panel via |connect_logo| button from the toolbar. 

.. |connect_logo| image:: _static/connect_logo.png
   :width: 6mm

.. figure:: _static/ngc_no_connection_en.png
   :name: connect_panel
   :align: center
   :width: 8cm

* Add connection to your Web GIS.

.. admonition:: Don't have a Web GIS yet?

   `How to create your Web GIS in a few clicks <https://docs.nextgis.com/docs_ngcom/source/create_webgis.html>`_

1. Click on the gear icon to open Settings.

2. In the Connections section create a **new** connection (enter URL of your Web GIS and, if needed, login and password of your NextGIS ID). 

.. figure:: _static/quick_webmap_connect_en.png
   :name: create_connection
   :align: center
   :width: 20cm


3. Click **Save**, then **OK**, and close the Settings menu. In the NextGIS Connect panel you'll see appear the entire resource tree of your Web GIS.

 
.. figure:: _static/qgis_connect_panel_en_2.png
   :name: resources_on_panel
   :align: center
   :width: 8cm

4. Select the *resource group* where you want to upload your project, click **Add to Web GIS** |button_cloud_upload| in the plugin toolbar and select **Upload all**.

.. figure:: _static/import_project_en_2.png
   :name: import_project
   :align: center
   :width: 20cm

After a while a newly created Web Map opens in the default browser.

.. figure:: _static/webmap_proj_en_2.png
   :name:  webmap_proj
   :align: center
   :width: 20cm

.. |button_cloud_upload| image:: _static/button_cloud_upload.png
   :width: 7mm
   :alt: cloud with upward arrow
