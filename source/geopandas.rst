.. _data_geopandas:

Как использовать данные в GeoPandas
===================================

* `Закажите данные <https://data.nextgis.com/ru/>`_ на интересующую Вас территорию в формате ESRI Shape.
* Дождитесь получения результата, скачайте, распакуйте архив с данными.
* Выберите нужный слой, например границы муниципалитетов (boundary-polygon-lvl6)
* Установите и загрузите модуль geopandas для Python.

Показать карту:

.. code-block:: python

   import geopandas
   boundaries = geopandas.read_file("/tmp/data/boundary-polygon-lvl6.shp")
   boundaries.plot(column="oktmo")

.. figure:: _static/geopandas_map.png
   :name: geopandas_map
   :align: center
   :width: 16cm


Посчитать и вывести площади районов:

.. code-block:: python

   boundaries["AREA"] = boundaries.to_crs("EPSG:32637").area / 10 ** 6
   boundaries[["NAME", "AREA"]]
   
.. figure:: _static/geopandas_table.png
   :name: geopandas_table
   :align: center
   :width: 16cm
