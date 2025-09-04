.. sectionauthor:: Aleksandr Myrov, Yuliya Grigorenko <grigorenko.j@gmail.com>

Как открыть карту или проект ArcMap в ArcGIS Pro
===================================================================

* `Закажите данные <https://data.nextgis.com/ru/catalog/subdivisions/?country=RU>`_ на интересующую Вас территорию в формате Shape (ArcMap) или Geodatabase (ArcMap).

.. note:: Вы можете заказать данные в формате ESRI Geodatabase (**ArcGIS Pro**). Тогда к данным будет приложен проект в формате APRX, который будет проще открыть.

* Скачайте и установите ArcGIS Pro, откройте его и создайте необходимую директорию для Ваших данных.

.. figure:: _static/arcgis_create_folder_en.png
   :name: arcgis_create_folder_pic
   :align: center
   :width: 24cm

* Дождитесь получения результата, `скачайте <https://data.nextgis.com/ru/orders/actual/>`_ и **распакуйте** архив с заранее заказанными данными и поместите их в подготовленную директорию.

Готовый проект включает все слои с настроенными стилями. 

* В панели «Catalog» нажмите «Project» → «Folders» → «MyProject», далее откройте папку со скачанными данными, внутри которой находится файл формата .MXD.

.. figure:: _static/arcgis_browse_folder_ru.png
   :name: arcgis_browse_folder_pic
   :align: center
   :width: 24cm

* Нажмите правой кнопкой мыши на файл формата .MXD и выберите «Import And Open».

.. figure:: _static/arcgis_import_ru.png
   :name: arcgis_import_pic
   :align: center
   :width: 24cm

Спустя некоторое время проект будет импортирован в ArcGIS Pro и данные будут готовы к работе.

.. figure:: _static/arcgis_result_ru.png
   :name: arcgis_result_pic
   :align: center
   :width: 24cm
