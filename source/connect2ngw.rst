.. _data_connect2ngw:

How to upload data to NextGIS Web with via NextGIS Connect
==========================================================

* `Order data <https://data.nextgis.com/en/>`_ for your area of interest in ESRI Shape format (QGIS).
* Wait for an email with the download link. Download and unpack the data.
* Download and install `QGIS <https://qgis.org/en/site/forusers/download.html>`_ or `NextGIS QGIS <https://nextgis.com/nextgis-qgis/>`_.
* Launch QGIS. To open a preset GIS project (which includes all layers with customized styles), click "Project" > "Open" and in pop-up window select the saved file "data.qgs".

.. figure:: _static/open_map1_en.png
   :name: open_map1
   :align: center
   :width: 26cm

* The project will be added to QGIS.

.. figure:: _static/open_map2_en.png
   :name: open_map2
   :align: center
   :width: 26cm
   
* To transfer GIS project from QGIS to NextGIS Web special plugin is needed. In Menu Toolbar select "Plugins" > "Manage and Install Plugins". In pop-up window type "NextGIS Connect" into Search field. Check the box next to the plugin to activate it.

.. figure:: _static/connect2ngw1_en.png
   :name: connect2ngw1
   :align: center
   :width: 20cm

* NextGIS Connect panel will appear. You can also call this panel via |connect2ngw2| button from the toolbar. 
.. |connect2ngw2| image:: _static/connect2ngw2.png

.. figure:: _static/connect2ngw3.png
   :name: connect2ngw3
   :align: center
   :width: 8cm
      
* Set connection to your Web GIS: press "Settings" button (gear icon), then in pop-up window press "New", in next pop-up window fill in all the fields with the details of your Web GIS and press "OK". You can notice, that in very first pop-up window the name of connection appeared; press "Close" to finish settings.

.. figure:: _static/connect2ngw4_en.png
   :name: connect2ngw4
   :align: center
   :width: 26cm
      
* In NextGIS Connect panel resources from your Web GIS are displayed now.

.. figure:: _static/connect2ngw5_en.png
   :name: connect2ngw5
   :align: center
   :width: 8cm
      
* Select Resource group which will host GIS project, press "Add to Web GIS" button and select "Import current project" from drop-down list.

.. figure:: _static/connect2ngw6_en.png
   :name: connect2ngw6
   :align: center
   :width: 8cm
      
* Web map with preset project will appear in your Web GIS

.. figure:: _static/connect2ngw7_en.png
   :name: connect2ngw7
   :align: center
   :width: 22cm
