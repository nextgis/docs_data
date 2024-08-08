.. _data_dem_3D_to_qgis:

Как загрузить данные рельефа в 3D окно QGIS
=============================================
 
* `Закажите данные <https://data.nextgis.com/ru/>`_ рельефа на интересующую Вас территорию в формате ESRI Shape (QGIS) и GeoTIFF с указанием шага изолиний.
* Дождитесь получения результата, скачайте, распакуйте архив с данными.
* Скачайте и установите `NextGIS QGIS <https://nextgis.ru/nextgis-qgis/>`_ или обычный `QGIS <https://qgis.org/>`_.
* Запустите QGIS.
* Перетащите из папки с распакованными данными файлы **hillshade.tif** (светотеневая отмывка), **dem.tif** (цифровая модель рельефа) и **contour_lines.shp** (изолинии рельефа) в интерфейс QGIS, расположите слои в правильном порядке, установите прозрачность на 50%

.. figure:: _static/elev_ngqgis_project_ru.png
   :name: elev_qgis_project
   :align: center
   :width: 24cm

* На верхней панели нажмите Вид ‣ 3D карты ‣ Новый 3D вид карты.

.. figure:: _static/3d_dem_newmap_ru.png
   :name: 3d_dem_newmap
   :align: center
   :width: 24cm

* Откройте настройки 3D карты.

.. figure:: _static/3d_dem_settings_open_ru.png
   :name: 3d_dem_settings_open_pic
   :align: center
   :width: 18cm

* В настройках 3D карты установите параметры для Рельефа - выберите ЦМР (растровый слой), укажите растровый слой **dem**, подберите остальные параметры в зависимости от ваших данных

.. figure:: _static/3d_dem_settings_ru.png
   :name: 3d_dem_settings
   :align: center
   :width: 18cm
   
* Нажмите OK. В окне появится модель данных рельефа в 3D.

.. figure:: _static/3d_dem_result_ru.png
   :name: 3d_dem_result
   :align: center
   :width: 18cm
