.. role:: raw-html-m2r(raw)
   :format: html


`Оглавление </docs/ru/index.md>`_
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Предыдущая страница: `Условия отображения <visibility.md>`_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Условия активности
==================

Описание
--------

**Условия активности** - задают условия активности, то есть доступности  поля для редактирования в представлении.
Синтаксис условий такой же, как в `условиях отображения <visibility.md>`_.

Пример в JSON:
^^^^^^^^^^^^^^

.. code-block::

   {
             "caption": "Основание для условия активности",
             "type": 1,
             "property": "enablement_condition_base",
             "size": 2,
             "maskName": null,
             "mask": null,
             "mode": null,
             "fields": [],
             "hierarchyAttributes": null,
             "columns": [],
             "actions": null,
             "commands": [],
             "orderNumber": 20,
             "required": false,
             "visibility": null,
             "enablement": null,
             "obligation": null,
             "readonly": false,
             "selectionPaginated": true,
             "validators": null,
             "hint": null,
             "historyDisplayMode": 0,
             "tags": null
           },
   {
             "caption": "Поле активно, если основание заполнено",
             "type": 1,
             "property": "enablement_condition_use",
             "size": 2,
             "maskName": null,
             "mask": null,
             "mode": null,
             "fields": [],
             "hierarchyAttributes": null,
             "columns": [],
             "actions": null,
             "commands": [],
             "orderNumber": 30,
             "required": false,
             "visibility": null,
             "enablement": ".enablement_condition_base !\u003d \u0027\u0027",
             "obligation": null,
             "readonly": false,
             "selectionPaginated": true,
             "validators": null,
             "hint": null,
             "historyDisplayMode": 0,
             "tags": null
           },
           {
             "caption": "Поле активно, если в основании \u00271\u0027",
             "type": 1,
             "property": "enablement_condition_1",
             "size": 2,
             "maskName": null,
             "mask": null,
             "mode": null,
             "fields": [],
             "hierarchyAttributes": null,
             "columns": [],
             "actions": null,
             "commands": [],
             "orderNumber": 40,
             "required": false,
             "visibility": null,
             "enablement": ".enablement_condition_base \u003d\u003d \u00271\u0027",
             "obligation": null,
             "readonly": false,
             "selectionPaginated": true,
             "validators": null,
             "hint": null,
             "historyDisplayMode": 0,
             "tags": null
           }

Следующая страница: `Условия обязательности <obligation.md>`_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

----

`Licence </LICENSE>`_ &ensp;  `Contact us <https://iondv.com/portal/contacts>`_ &ensp;  `English </docs/en/2_system_description/metadata_structure/meta_view/enablement.md>`_   &ensp;
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


.. raw:: html

   <div><img src="https://mc.iondv.com/watch/local/docs/framework" style="position:absolute; left:-9999px;" height=1 width=1 alt="iondv metrics"></div>


----

Copyright (c) 2018 **LLC "ION DV"**.\ :raw-html-m2r:`<br>`
All rights reserved. 
