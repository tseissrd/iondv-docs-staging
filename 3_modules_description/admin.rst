.. role:: raw-html-m2r(raw)
   :format: html

Модуль ionadmin
===============
`Оглавление </docs/ru/index.md>`_
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Назад: `Модули <modules.md>`_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Модуль администрирования (ionadmin)** – используется для назначения прав, управления задачами по расписанию и другими административными задачами.

Настройка модуля Ionadmin в файле config.json
---------------------------------------------

Настройка записи в БД интервалов
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Настройка в виде модального окна на списке медленных запросов.
В в файле config.json модуля ionadmin указывать источник:

.. code-block:: json

   "profiling": {
       "slowQuery": {
         "sources": [
             {
               "collection": "system.profile"
             }
         ]
       }
     }

Если свойство ``"sources"`` не задано или null, то будет браться из таблицы:

.. code-block:: json

   { 
     "profiling": {
       "slowQuery": {
         "sources": null
       }
     }
   }

Если задан пустой массив, то источников нет.

Настройка источников логов
~~~~~~~~~~~~~~~~~~~~~~~~~~

Источники логов (может быть несколько) указываются в конфиге модуля:

.. code-block:: json

   "profiling": {
       "slowQuery": {
         "sources": [
           {
             "collection": "system.profile"
           },
           {
             "file": "D:/Temp/slow-query.txt"
           }
         ]
       }
     }

Сделанные выборки хранятся в отдельной таблице и не зависят от текущего состояния источников логов. Их можно дополнить редактированием. Например, комментариями или пометками решена проблема или нет.

Настройка резервирования БД
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Настройка в *ionmodule/config*\ :

.. code-block:: json

   "backup": {
       "dir": "../ion-backups",
       "zlib": {
         "level": 1
       }
     }


* 
  ``dir`` содержит путь папки, в которой было запущено приложение ноды. По умолчанию *"../ion-backups"*

* 
  ``zlib.level`` - уровень сжатия, также влияет на скорость создания архива. По умолчанию - значение 3

* 
  К тому же необходимо что бы утилита ``export.js`` с заданными параметрами корректно отрабатывала сама по себе.

Руководство пользователя по безопасности
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Руководство пользователя по безопасности находится `здесь <admin_security.md>`_.

----

`Licence </LICENSE>`_\ &ensp;  `Contact us <https://iondv.com/portal/contacts>`_ &ensp;  `English </docs/en/3_modules_description/admin.md>`_ &ensp;
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


.. raw:: html

   <div><img src="https://mc.iondv.com/watch/local/docs/framework" style="position:absolute; left:-9999px;" height=1 width=1 alt="iondv metrics"></div>


----

Copyright (c) 2018 **LLC "ION DV".**\ :raw-html-m2r:`<br>`
All rights reserved. 
