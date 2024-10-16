# Динамические лобби-арты

## Спецификации

**Поддерживаемые форматы:** PNG, JPG, GIF, DMI\*

- При использовании DMI формата стоит учитывать, что в одном файле может храниться лишь одно изображение, стейт иконки требуется оставить пустым.

**Разрешение:** 480x480\*

- Возможно использование изображений и большего / меньшего разрешения, но они будут центрированы и обрезаны.

Стоит избегать использования изображений больше ~2000 пикселей в ширину или высоту может вызвать зависания и вылеты клиентов.

Файлы GIF желательно переводить в нативный формат DMI, со вторым Byond работает немного лучше.

## Использование

Изображения помещаются в папку по пути `/config/lobby_art/images`, имена файлов могут быть любыми, но желательно избегать кириллицы и иных не **ASCII** символов.

К каждому изображению **можно** приложить метаинформацию, в ней можно указать название рисунка, его автора и опционально социальную сеть.

Файл **json** с метаинформацией должен иметь то же название, что и описываемое избражение, ниже приведены поддерживаемые поля.

```json
{
  "title": "...",
  "author": "...",
  "socials": "..."
}
```
