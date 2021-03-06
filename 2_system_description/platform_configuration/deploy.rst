.. role:: raw-html-m2r(raw)
   :format: html

Конфигурационный файл - ``deploy.json``
===========================================
`Оглавление </docs/ru/index.md>`_
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Предыдущая страница: `Мета отчёта </docs/ru/2_system_description/metadata_structure/meta_report/meta_report.md>`_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Конфигурационный файл deploy.json** - это файл, в котором описывается структура параметров программной системы и её конкретная настройка.

Структура файла deploy.json:
----------------------------

.. list-table::
   :header-rows: 1

   * - Поле
     - Имя
     - Описание
   * - ``"namespace":``
     - **Название проекта**
     - Пространство имен проекта.
   * - ``"parametrised": true,``
     - **Параметризация**
     - Подключение параметризации. При установленном значении "true" есть возможность задавать параметры, в которые, при сборке приложения, передаются переменные, заданные в ini-файлах или переменных окружения проекта.
   * - ``"globals": {``
     - `\ **Глобальные настройки** <deploy_globals.md>`_
     - Глобальные параметры конфигурирования.
   * - ``"deployer": "built-in"``
     - **Сборки**
     - Параметр конфигурирования сборки, на данный момент единственный.
   * - ``"modules"``
     - `\ **Настройки модулей** <deploy_modules.md>`_
     - Массив объектов - описание модулей.


Пример файла `deploy.json <deploy_ex.md>`_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Следующая страница: `Зависимости в package.json <package.md>`_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

----

`Licence </LICENSE>`_ &ensp;  `Contact us <https://iondv.com/portal/contacts>`_ &ensp;  `English </docs/en/2_system_description/platform_configuration/deploy.md>`_   &ensp;
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


.. raw:: html

   <div><img src="https://mc.iondv.com/watch/local/docs/framework" style="position:absolute; left:-9999px;" height=1 width=1 alt="iondv metrics"></div>


----

Copyright (c) 2018 **LLC "ION DV"**.\ :raw-html-m2r:`<br>`
All rights reserved. 
