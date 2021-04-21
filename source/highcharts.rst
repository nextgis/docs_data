.. _data_highcharts:

How to upload data to Highcharts Maps (highcharts.js)
===========================

* `Order data <https://data.nextgis.com/en/>`_ for your area of interest in GeoJSON format.
* Wait for email with download link, download and unpack archive with data.
* Select target layer.
* Чтобы подключить данные с NextGIS Data в Highcharts Maps, нужно их захостить (положить туда, где они будут доступны по гиперссылке) и указать в подключении:
* To upload layer to Highcharts Maps first you need to host it (store in a place, asseccible through hyperlink) and specify for connection:

.. code-block:: javascript

   Highcharts.getJSON('https://cdn.jsdelivr.net/gh/highcharts/highcharts@v7.0.0/samples/data/germany.geo.json', function (geojson)

* There are a lot of `examples of gata usage <https://www.highcharts.com/demo/maps/geojson>`_ in Highcharts Maps documentation, so its source code is available.

* The example of NextGIS Data usage is presented below, also `live example <https://jsfiddle.net/rendrom/nhv4mu5z/>`_ is available.

.. figure:: _static/highcharts.png
   :name: highcharts
   :align: center
   :width: 16cm

.. note::
   Highcharts Maps library handles well fast visualization of spatial data statistics. However such libraries as Mapbox GL JS, Openlayers and Leaflet are better for interactive mapping. Examples of data upload from json files to forementioned libraries can be found here: https://jsfiddle.net/rendrom/a1xf63bk/ and https://jsfiddle.net/rendrom/yg6xz9kj/. In these examples `NextGIS Frontend <https://github.com/nextgis/nextgis_frontend>`_ libraries are used.

.. hint::
   For faster and better performing of data rendering in the web, additional generalization, thinning and modification of initial data can be useful. The resulting file would be smaller in size, has less nodes in polygones and lines and without unnecessary attributes.
