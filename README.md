### task-cordova-app

Приложение представляет собой набор мелких фич - фонарик, строительный уровень и линейка. Используются следующие плагины:

* `cordova-plugin-flashlight` - управление вспышкой;
* `cordova-plugin-screen-orientation` - управление ориентацией экрана;
* `cordova-plugin-device-motion` - отслеживание датчиков положения в пространстве (акселерометр);
* `cordova-plugin-screensize` - получение размеров экрана (в пикселях и дюймах).

#### Проблемы:
* При разработке использовался эмулятор Android версии 7.0, в котором по-умолчанию используется WebView с браузером Chrome 51+: с ним проблем не было. Однако, при тестировании на реальном девайсе с версией Android 4.4 и установленным браузером Chrome 58, VebView использовал старую версию Chrome, а именно 30. Соответственно, часть функциональности не работано (если конкретно: сломались флексы и верстка поехала). Решение нашел пока только одно - переверстать без флексов :)
