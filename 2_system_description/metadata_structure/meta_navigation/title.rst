.. role:: raw-html-m2r(raw)
   :format: html


`Оглавление </docs/ru/index.md>`_
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Назад: `Мета узлов навигации <navigation_nodes.md>`_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Заголовок страницы - ``"title"``
====================================

Поле **"title"** необходимо для того, чтобы задать отличный от поля ``"caption"`` заголовок страницы в меню навигации. 

Описание
--------

Для формирования заголовка страницы в первую очередь используется значение поля ``"title"`` соответствующего узла навигации. Если поле ``"title"`` не задано - пустая строка, то для формирования заголовка страницы используется поле ``"caption"`` меты узла навигации.\ :raw-html-m2r:`<br>`
Для формирования заголовка страницы на страницах списка выбора (при открытии списка класса справочника из форм) используется ``"caption"`` общей части меты класса.  

JSON
----

.. code-block::

   {
     "code": "administrations.municipals",
     "orderNumber": 0,
     "type": 1,
     "title": "Администрации муниципальных районов", \\ отличается от наименования узла навигации поля `"caption"`
     "caption": "Муниципальные районы",
     "classname": "Organisation",
     "container": null,
     "collection": null,
     "url": null,
     "hint": "Список администраций муниципальных районов",
     "conditions": [],
     "sorting": [],
   }

----

`Licence </LICENSE>`_ &ensp;  `Contact us <https://iondv.com/portal/contacts>`_ &ensp;  `English </docs/en/2_system_description/metadata_structure/meta_navigation/title.md>`_   &ensp;
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


.. raw:: html

   <div><img src="https://mc.iondv.com/watch/local/docs/framework" style="position:absolute; left:-9999px;" height=1 width=1 alt="iondv metrics"></div>


----

Copyright (c) 2018 **LLC "ION DV"**.\ :raw-html-m2r:`<br>`
All rights reserved. 
