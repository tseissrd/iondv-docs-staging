.. role:: raw-html-m2r(raw)
   :format: html


`Оглавление </docs/ru/index.md>`_
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Назад: `Модуль регистра <registry.md>`_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Настройки DI
============

Подключение в глобальных настройках модуля регистра
---------------------------------------------------

Пример в deploy.json
^^^^^^^^^^^^^^^^^^^^

.. code-block:: json

   "modules": {
       "registry": {
         "globals": {
        "di": {

treegridController
------------------

Описание
^^^^^^^^

Предназначен для создания иерархичных списков объектов в атрибуте-коллекции класса или в навигации класса.\ :raw-html-m2r:`<br>`
Работает с использование компонента dhtmlxSuite_v51_pro (https://dhtmlx.com/docs/products/dhtmlxTreeGrid/).

Подключение в DI
^^^^^^^^^^^^^^^^

.. code-block:: json

   "treegridController": {
               "module": "applications/viewlib/lib/controllers/api/treegrid",
               "initMethod": "init",
               "initLevel": 0,
               "options": {
                 "module": "ion://module",
                 "logger": "ion://sysLog",
                 "securedDataRepo": "ion://securedDataRepo",
                 "metaRepo": "ion://metaRepo",
                 "auth": "ion://auth",
                 "config": { // основной конфиг
                   "*": { // выборка объектов возможна в каждой навигации
                     "eventBasic@project-management":{ // выборка объектов по указанному классу
                       "roots":[{ // поиск корней
                         "property": "name",
                         "operation": 1,
                         "value": [null],
                         "nestedConditions": []
                       }],
                       "childs":["basicObjs"] // поиск дочерних элементов
                     },

Виды шаблонов
^^^^^^^^^^^^^


* "template": "treegrid/collection"\ :raw-html-m2r:`<br>`
  Для атрибута-коллекции. Подключается в представлении формы объекта:   

.. code-block:: json

   "options": {
               "template": "treegrid/collection",
               "reorderable": true,
               "treegrid": {
                 "width": "auto,100,100,100,100,0",
                 "align": "left, center,center,center,center, left",
                 "sort": "str, date, date, date, date, int",
                 "enableAutoWidth": false,
                 "paging": {
                   "size": 20
                 }
               }
             }


* "template": "treegrid/list"\ :raw-html-m2r:`<br>`
  Для навигации класса. Подключение:   

.. code-block:: json

   "options": {
       "template": "treegrid/list"
     }


* Настройка ``skin``

https://docs.dhtmlx.com/grid__skins.html

.. code-block::

   "options" : {
   ...
     "treegrid" : {
       "skin": "material" // по умолчанию
       // "skin": "skyblue"
       // "skin": "terrace"
       // "skin": "web"
     }
   }

Дополнительные источники информации по treegridController
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


* 
  `Иерархическое представление для коллекций <https://git.iondv.ru/ION/platform/blob/v1.24/docs/ru/2_system_description/platform_configuration/deploy_modules.md#настройка-иерархического-представления-для-коллекций>`_.

  DHTMLX (dhtmlxSuite_v51_pro)


  * https://docs.dhtmlx.com/
  * https://dhtmlx.com/docs/products/dhtmlxTreeGrid/

  ----

`Licence </LICENSE>`_\ &ensp;  `Contact us <https://iondv.com/portal/contacts>`_ &ensp;  `English </docs/en/3_modules_description/registry_treegrid.md>`_ &ensp;
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


.. raw:: html

   <div><img src="https://mc.iondv.com/watch/local/docs/framework" style="position:absolute; left:-9999px;" height=1 width=1 alt="iondv metrics"></div>


----

Copyright (c) 2018 **LLC "ION DV".**\ :raw-html-m2r:`<br>`
All rights reserved. 
