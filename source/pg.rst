.. _data_pg:

Как загрузить данные в PostgreSQL/PostGIS
=========================================

* `Закажите данные <https://data.nextgis.com/ru/>`_ на интересующую Вас территорию в формате SQL (PostgreSQL/PostGIS).
* Дождитесь получения результата, скачайте, распакуйте архив с данными.
* Выберите нужный слой.

Для импорта данных в базу данных используйте psql.

.. code-block:: bash

   psql -f boundary-polygon.sql -h host -U user database

где boundary-polygon.sql - выбранный слой, host - адрес сервера с базой (или localhost), user - имя пользователя, database - название базы данных.

.. note::

   Если в результате импорта появится сообщения о проблеме с кодировкой, выполните следующие команды перед повторным запуском

.. code-block:: bash

   SET PGCLIENTENCODING=utf-8
   chcp 65001

.. warning::

   Не пытайтесь использовать pgAdmin.
