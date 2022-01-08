.. _data_r:

Как загрузить данные в R
===========================

* `Закажите данные <https://data.nextgis.com/ru/>`_ на интересующую Вас территорию в формате ESRI Shape.
* Дождитесь получения результата, скачайте, распакуйте архив с данными.
* Выберите нужный слой.
* Установите и загрузите модуль rgdal для R.

Если вы работаете в Windows, то для импорта данных в R с корректными названиями атрибутов используйте:

.. code-block:: r

   Districts <- readOGR(dsn ='KO/data/boundary-polygon-lvl6.shp', use_iconv = TRUE, encoding = "UTF-8")

в других операционных системах достаточно:

.. code-block:: r

   Districts <- readOGR(dsn ='KO/data/boundary-polygon-lvl6.shp')
