.. _data_pg:

How to load data into PostgreSQL/PostGIS
=========================================

.. important::
	To run, you need an installed PostgreSQL database with the `PostGIS extension <https://postgis.net/install/>`_.

* `Order data <https://data.nextgis.com/en/>`_ for your area of interest in SQL (PostgreSQL/PostGIS) format.
* Wait for email with download link, download and unpack archive with data.
* Select target layer.

Use psql to import data into database.

.. code-block:: bash

   psql -f boundary-polygon.sql -h host -U user database

where boundary-polygon.sql - target layer, host - address of the server with database (or localhost), user - user name, database - name of the database.

.. note::

   For Windows OS if the command results in an encoding problem message, run the following commands before re-running

.. code-block:: bash

   SET PGCLIENTENCODING=utf-8
   chcp 65001

.. warning::

   Do not use pgAdmin.
