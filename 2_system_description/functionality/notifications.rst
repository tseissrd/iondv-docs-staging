.. role:: raw-html-m2r(raw)
   :format: html

Уведомления
===========
`Оглавление </docs/ru/index.md>`_
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Назад: `Функциональность <functionality.md>`_
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Уведомления** - на форме отображются в виде красного колокольчика, при клике на котором отображается лента уведомлений (10 последних непрочитанных), при клике на уведомлении оно скрывается как прочитанное. Лента обновляется раз в 15 секунд. Если колокольчик отсутсвует это значит что уведомлений нет.

Настройка уведомлений
---------------------

Реализована отправка уведомлений на почту. Настраивается в проекте - **TODO**.

Реализовано API для отправки уведомлений программно. т.е. можно в обработчике события отправить уведомление.
В админке при отправке уведомлений в поле "Получатели" указывается список полных имен пользователей (user@local) разделенных пробелом.

Хранение уведомлений происходит в коллекциях: ion_notification, ion_notification_recievers.

----

`Licence </LICENSE>`_ &ensp;  `Contact us <https://iondv.com/portal/contacts>`_ &ensp;  `English </docs/en/2_system_description/functionality/printed_forms.md>`_   &ensp;
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


.. raw:: html

   <div><img src="https://mc.iondv.com/watch/local/docs/framework" style="position:absolute; left:-9999px;" height=1 width=1 alt="iondv metrics"></div>


----

Copyright (c) 2018 **LLC "ION DV"**.\ :raw-html-m2r:`<br>`
All rights reserved. 
