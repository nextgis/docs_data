.. _data_tableau:

Как добавить слой в Tableau
===========================

* `Закажите данные <https://data.nextgis.com/ru/>`_ на интересующую Вас территорию, например, в формате GeoJSON.
* Дождитесь получения результата, скачайте, распакуйте архив с данными.
* В программе Tableau нажмите на иконку **New Data Source**, выберите **Spatial file** и откройте нужный слой с пространственными данными.

.. figure:: _static/tableau1.png
   :name: tableau1
   :align: center
   :width: 16cm
   
* Когда вы подгружаете файл геоданных, Tableau создает поле **Geometry**, описывающее тип геометрии ваших пространственных данных - *Point* для точечных данных, *Linestring or Multilinestring* для линий, *Polygon or Multipolygon* для полигонов. Это поле используется для создания карты с вашими пространственными данными.
После загрузки данных в виде таблицы и генерации поля с геометрией, откройте новую рабочую область кнопкой слева внизу.


.. figure:: _static/tableau2.png
   :name: tableau2
   :align: center
   :width: 16cm
   
* В панели **Data** дважды кликнете на поле **Geometry**. Ваша карта загружена.

.. figure:: _static/tableau3.png
   :name: tableau3
   :align: center
   :width: 16cm
