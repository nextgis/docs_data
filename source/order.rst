Как заказать данные
====================

.. _data_area:

Выбрать территорию
----------------------

Есть несколько способов выбрать область, на которую вы хотите заказать данные.

1. Нужный регион вы можете найти в `каталоге <https://data.nextgis.com/ru/catalog/subdivisions/?country=RU>`_. Выберите регион, чтобы увидеть его границы и цену выгрузки. 

2. В `строке поиска <https://data.nextgis.com/ru/>`_ на главной странице или на странице выбора области `справа на карте <https://data.nextgis.com/ru/region/custom/base>`_ введите нужное название и выберите подходящий регион из предлагаемого списка.

3. Также можно `нарисовать свою область <https://data.nextgis.com/ru/region/custom/base/>`_ полигоном на карте или загрузить границу из файла.

.. figure:: _static/data_area_select_ru.png
   :name: 
   :align: center
   :width: 20cm

* |button_area_rect| - выделить область прямоугольником;
* |button_area_draw| - нарисовать произвольный полигон;
* |button_data_upload| - загрузить файл границы;
* |button_clear_area| - снять выделение;
* |button_area_fullscreen| - отрыть карту на весь экран для точного выделения области.

.. |button_data_upload| image:: _static/button_data_upload.png
   :width: 6mm
.. |button_area_draw| image:: _static/button_area_draw.png
   :width: 6mm
.. |button_area_rect| image:: _static/button_area_rect.png
   :width: 6mm
.. |button_area_fullscreen| image:: _static/button_area_fullscreen.png
   :width: 6mm
.. |button_clear_area| image:: _static/button_clear_area.png
   :width: 6mm

.. _data_type:

Выбрать тип данных
-------------------

.. figure:: _static/data_type_select_ru.png
   :name: 
   :align: center
   :width: 20cm


Можно заказать следующие данные:

* `Базовая карта OpenStreetMap <https://data.nextgis.com/ru/region/custom/base/>`_
* `Базовая карта Ouverture <https://data.nextgis.com/ru/region/custom/overture/>`_
* `Рельеф <https://data.nextgis.com/ru/region/custom/dem/>`_
* `Застройка AI <https://data.nextgis.com/ru/region/custom/msbld/>`_
* `Дороги AI <https://data.nextgis.com/ru/region/custom/msrd/>`_
* `Космосъёмка <https://data.nextgis.com/ru/region/custom/sat/>`_
* `Реформа ЖКХ <https://data.nextgis.com/ru/region/custom/gkh/>`_
* `Особо охраняемые природные территории <https://data.nextgis.com/ru/region/custom/oopt/>`_
* `Роснедра <https://data.nextgis.com/ru/region/custom/rnlic/>`_
* `Наследие <https://data.nextgis.com/ru/region/custom/heritage/>`_

На каждой странице доступны ссылки на структуру данных и примеры.

.. _data_format:

Выбрать формат
---------------

В выпадающем меню "Формат" выберите нужный. 

.. figure:: _static/data_format_select_ru.png
   :name: 
   :align: center
   :width: 20cm

Формат по умолчанию для векторных слоёв - GeoPackage (QGIS).

Вы можете просмотреть список форматов для каждого типа данных, а также скачать и протестировать `примеры <https://data.nextgis.com/ru/about/#formats>`_ во всех доступных форматах.

.. _data_layers:

Выбрать слои
--------------

Данные могут включать в себя один или несколько слоёв. Чтобы увидеть, что именно входит в каждый слой, ознакомьтесь со структурой данных.

Если навести курсор на слой, вы увидите пример скрина. Обратите внимание, что это просто иллюстрация, данные на конкретную территорию могут не содержать объектов в этом слое.

.. figure:: _static/data_osm_layer_ill_ru.png
   :name: 
   :align: center
   :width: 20cm


При заказе Базовой карты OSM и Рельефа можно выбрать, какие из слоёв вам нужны, и отключить остальные.

.. figure:: _static/data_dem_layers_select_ru.png
   :name: 
   :align: center
   :width: 20cm

Для Рельефа также можно выбрать шаг изолиний.



.. _data_order:

Оформление заказа
------------------

После того, как вы выбрали нужные данные, внизу страницы вы увидите детали и цену заказа. Нажмите **Заказать данные**.

Введите e-mail, на который хотите получить ссылку для скачивания данных. Если у вас есть NextGIS ID, введите тот e-mail, которые использовали при регистрации.

Проверьте ещё раз детали заказа. Особенно обратите внимание на выбор формата. При переходе между вкладками и других действиях страница могла обновиться, сбросив сделанный вами выбор.

.. figure:: _static/data_order_details_ru.png
   :name: 
   :align: center
   :width: 10cm

Ниже можно ввести промокод на скидку, если он у вас есть.

Убедившись, что данные заказа верные, нажмите **Оплатить заказ**.

Заказ можно сделать как от физического, так и от `юридического лица <https://data.nextgis.com/ru/faq/#pricebywire>`_.

`Подробнее об оплате и документах <https://data.nextgis.com/ru/region/custom/base/>`_.

Обратите внимание, что через русскоязычный интерфейс сайта предлагается оплата в рублях. Если вы хотите оплатить заказ картой, выпущенной в другой валюте, переключитесь на английский интерфейс.
