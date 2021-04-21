.. _data_pg:

How to load data into PostgreSQL/PostGIS
=========================================

* `Order data <https://data.nextgis.com/en/>`_ for your area of interest in SQL (PostgreSQL/PostGIS) format.
* Wait for email with download link, download and unpack archive with data.
* Select target layer.

Use psql to import data into database.

.. code-block:: bash

   psql -f boundary-polygon.sql -h host -U user database

where boundary-polygon.sql - target layer, host - address of the server with database (or localhost), user - user name, database - name of the database.

.. warning::

   Do not use pgAdmin.
