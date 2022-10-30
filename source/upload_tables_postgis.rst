.. _data_upload_tables_pg:

How to load multiple tables of different regions in PostgreSQL/PostGIS
========================================================================

.. important::
	To run, you need an installed PostgreSQL database with the `PostGIS <https://postgis.net/install/>`_.

* `Order data <https://data.nextgis.com/en/>`_ for multiple regions in SQL (PostgreSQL/PostGIS) format.
* Wait for an email with the download link. Download and unpack the data.
* Open the first dataset. Load target layer as stated `here <https://data.nextgis.com/en/howto/pg/>`_ without changing the structure.

For example:

.. code-block:: bash

   psql -f aerialway-line.sql -h host -U user -d database

where aerialway-line.sql - target layer, host - address of the server with database (or localhost), user - user name, database - name of the database.

* Go to the second dataset. Open in the editor (Notepad) same type of layer, which was loaded from the first set (например aerialway-line.sql)

Modify it so that only this structure remains (remove extra lines):

.. code-block:: bash

   SET standard_conforming_strings = OFF;
   BEGIN;
   COPY "public"."boundary_polygon_lvl8 ...
   ...
   END;
   COMMIT;

Modified file example:

.. code-block:: bash

   SET standard_conforming_strings = OFF;
   BEGIN;
   COPY "public"."aerialway_line" ("wkb_geometry", "aerialway", "name", "name_en", "name_ru", "osm_type", "osm_id") FROM STDIN;
   0105000020E61000000100000001020000000D0000007CABBF6F8D25344046802E75EB784B40A279A5D189253440DA0BBBDEEC784B40BF547DF8432534401AB3DB1D08794B40E129E44A3D2534404EA6C0B80A794B4064986E6D3C2534405A0CC3EC0A794B40597A23A93B25344095C84FF40A794B40A65F22DE3A253440CB51DBE10A794B402A2AD1483A2534403C69E1B20A794B40EE3F321D3A2534404240BE840A794B407D282C4C3A253440BF61A2410A794B403FA2AE5A3E253440196B24AE08794B40D9C6E93587253440A5CAE660EC784B403CDC0E0D8B253440888961E2EA784B40	gondola	Канатная дорога	\N	\N	way	71513012\.
   END;
   COMMIT;

* Load the edited file(s) in the same way as in step 3 to the database

.. code-block:: bash

   psql -f aerialway-line.sql -h host -U user -d database

