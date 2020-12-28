.. _data_pg:

Как загрузить данные в PostgreSQL/PostGIS
=========================================

* `Закажите данные <https://data.nextgis.com/ru/>`_ на интересующую Вас территорию в формате SQL (PostgreSQL/PostGIS).
* Дождитесь получения результата, скачайте, распакуйте архив с данными.
* Выберите нужный слой.

Для импорта данных в базу данных используйте psql.

.. code-block:: bash

   psql -f boundary-polygon.sql -h host -U user database

где, boundary-polygon.sql - выбранный слой, host - адрес сервера с базой (или localhost), user - имя пользователя, database - название базы данных.

.. warning::

   Не пытайтесь использовать pgAdmin. Он не умеет работать с геометриями объектов в формате WKB.
