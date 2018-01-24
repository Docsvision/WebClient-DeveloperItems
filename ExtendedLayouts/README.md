# Примеры расширенных разметок Docsvision 5 Web-клиент

Подробности о каждом элементе управления расширенных разметок можно уточить в [документации](https://docsvision.github.io/WebClient-JsDocApi/globals.html)
 

## Как заменить встроенные расширенные разметки 

1. Скопировать файл с выбранной разметкой в каталог "Путь к установленному Web-клиент\ExtendedLayouts"
2. Перезапустить IIS

## Как подключить файл с собственной расширенной разметкой
1. В web.config Docsvision 5 Web-клиент в раздел "ExtendedLayouts" необходимо добавить элемент ```<ExtendedLayout LayoutPosition="Идентификатор расширенной разметки (любое стровокое значение)" FileName="Наименование файла расширенных разметок в каталоге ExtendedLayouts" />```.
2. В существующую расширенную разметку Docsvision 5 Web-клиент (Например, DV.MainMenuLayoutPosition.xml) добавить элемент управления [LayoutPageMainMenuItem](https://docsvision.github.io/WebClient-JsDocApi/classes/webclient.layoutpagemainmenuitem.html).
3. Следует заполнить два атрибута:
[header](https://docsvision.github.io/WebClient-JsDocApi/classes/webclient.layoutpagemainmenuitemparams.html#header) - наименование элемента меню, 
[position](https://docsvision.github.io/WebClient-JsDocApi/classes/webclient.layoutpagemainmenuitemparams.html#position) - идентификатор расширенной разметки.
4. Перезапустить IIS.