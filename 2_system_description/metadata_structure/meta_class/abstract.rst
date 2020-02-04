.. role:: raw-html-m2r(raw)
   :format: html


`Оглавление </docs/ru/index.md>`_
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Предыдущая страница: `Семантика <semantic.md>`_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Признак абстрактности класса
----------------------------

**Признак абстрактности класса** - требуется в случае, когда необходимо по ссылке атрибута на базовый класс отображать список выбора его наследников. При формировании списка выбора классов для создания обьекта абстрактные классы не включены. Выставите ``true`` в поле "abstract".

Пример
^^^^^^

.. code-block::

   {
      "name": "SomeClassName",
      "abstract": true
   }

Класс становится недоступным для инициализации на уровне UI.

Пример
^^^^^^

.. code-block::

   {
     "isStruct": false,
     "key": [
       "id"
     ],
     "semantic": "value|[|plannedValue|](|dateStart|-|dateEnd|)",
     "name": "indicatorValueBasic",
     "version": "",
     "caption": "Значения показателей на период",
     "ancestor": null,
     "container": null,
     "creationTracker": "",
     "changeTracker": "",
     "history": 0,
     "journaling": true,
     "abstract": true,
     "compositeIndexes": [
       {
         "properties": [
           "indicatorBasic",
           "dateStart",
           "dateEnd"
         ],
         "unique": true
       }
     ],
     "properties": [
   ...

Следующая страница: `Версионирование <metaversion.md>`_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

----

`Licence </LICENSE>`_ &ensp;  `Contact us <https://iondv.com/portal/contacts>`_ &ensp;  `English </docs/en/2_system_description/metadata_structure/meta_class/abstract.md>`_   &ensp;
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


.. raw:: html

   <div><img src="https://mc.iondv.com/watch/local/docs/framework" style="position:absolute; left:-9999px;" height=1 width=1 alt="iondv metrics"></div>


----

Copyright (c) 2018 **LLC "ION DV"**.\ :raw-html-m2r:`<br>`
All rights reserved. 
