.. _data_upload_tables_pg:

Как загрузить несколько одинаковых таблиц разных регионов в PostgreSQL/PostGIS
=============================================================================

.. important::
	Для загрузки потребуется предустановленная БД PostgreSQL с расширением `PostGIS <https://postgis.net/install/>`_.

* `Закажите данные <https://data.nextgis.com/ru/>`_ на несколько регионов в формате SQL (PostgreSQL/PostGIS).
* Дождитесь получения результата, скачайте, распакуйте архивы с данными.
* Откройте первый набор данных. Загрузите первый файл как указано `здесь <https://data.nextgis.com/ru/howto/pg/>`_, не меняя его структуру.

Например:

.. code-block:: bash

   psql -f aerialway-line.sql -h host -U user -d database

где aerialway-line.sql - выбранный слой, host - адрес сервера с базой (или localhost), user - имя пользователя, database - название базы данных.

* Возьмите второй набор данных. Откройте в редакторе тот же тип слоя, который был загружен из первого набора (например aerialway-line.sql)

Отредактируйте его так, чтобы осталась только такая структура (удалить лишние строки):

.. code-block:: bash

   SET standard_conforming_strings = OFF;
   BEGIN;
   COPY "public"."boundary_polygon_lvl8 ...
   ...
   END;
   COMMIT;

Пример измененного файла:

.. code-block:: bash

   SET standard_conforming_strings = OFF;
   BEGIN;
   COPY "public"."aerialway_line" ("wkb_geometry", "aerialway", "name", "name_en", "name_ru", "osm_type", "osm_id") FROM STDIN;
   0105000020E61000000100000001020000000D0000007CABBF6F8D25344046802E75EB784B40A279A5D189253440DA0BBBDEEC784B40BF547DF8432534401AB3DB1D08794B40E129E44A3D2534404EA6C0B80A794B4064986E6D3C2534405A0CC3EC0A794B40597A23A93B25344095C84FF40A794B40A65F22DE3A253440CB51DBE10A794B402A2AD1483A2534403C69E1B20A794B40EE3F321D3A2534404240BE840A794B407D282C4C3A253440BF61A2410A794B403FA2AE5A3E253440196B24AE08794B40D9C6E93587253440A5CAE660EC784B403CDC0E0D8B253440888961E2EA784B40	gondola	Канатная дорога	\N	\N	way	71513012\.
   END;
   COMMIT;

* Загрузите отредактированный(е) файл(ы) аналогично пункту 3 в БД

.. code-block:: bash

   psql -f aerialway-line.sql -h host -U user -d database

