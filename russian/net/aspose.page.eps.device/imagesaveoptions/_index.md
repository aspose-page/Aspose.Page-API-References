---
title: ImageSaveOptions
second_title: Справочник по Aspose.Page для .NET API
description: Этот класс содержит опции необходимые для управления процессом сохранения изображения.
type: docs
weight: 50
url: /ru/net/aspose.page.eps.device/imagesaveoptions/
---
## ImageSaveOptions class

Этот класс содержит опции, необходимые для управления процессом сохранения изображения.

```csharp
public class ImageSaveOptions : SaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions#constructor)() | Инициализирует новый экземпляр класса[`ImageSaveOptions`](../imagesaveoptions)со значениями по умолчанию для флагов!:SuppressErrors(true) и!:Debug(false). |
| [ImageSaveOptions](imagesaveoptions#constructor_1)(bool) | Инициализирует новый экземпляр[`ImageSaveOptions`](../imagesaveoptions)со значением по умолчанию для флага!:Debug(false). |

## Характеристики

| Имя | Описание |
| --- | --- |
| [AdditionalFontsFolders](../../aspose.page/saveoptions/additionalfontsfolders) { get; set; } | Указывает дополнительные папки, в которых конвертер должен найти шрифты для входного документа. Папка по умолчанию - стандартная папка шрифтов, в которой ОС находит шрифты для внутренних нужд. |
| virtual [Debug](../../aspose.page/saveoptions/debug) { get; set; } | Указывает, должна ли отладочная информация выводиться в стандартный поток вывода или нет. |
| virtual [Exceptions](../../aspose.page/saveoptions/exceptions) { get; } | Возвращает список подавленных ошибок преобразования. Если!:SuppressErrorsистинно. |
| [JpegQualityLevel](../../aspose.page/saveoptions/jpegqualitylevel) { get; set; } | Категория "Качество" указывает уровень сжатия изображения. Доступные значения:от 0 до 100. Чем меньше указанное число, тем выше степень сжатия и, следовательно, ниже качество изображения. Значение 0 приводит к самому низкому качеству изображения, а 100 — к самому высокому. |
| [Resolution](../../aspose.page.eps.device/imagesaveoptions/resolution) { get; set; } | Получает/устанавливает разрешение изображения. |
| virtual [SupressErrors](../../aspose.page/saveoptions/supresserrors) { get; set; } | Указывает, должны ли ошибки подавляться или нет. Если true, в список[`Exceptions`](../../aspose.page/saveoptions/exceptions)добавляются подавленные ошибки. Если false, первая ошибка завершит программу. |

### Смотрите также

* class [SaveOptions](../../aspose.page/saveoptions)
* пространство имен [Aspose.Page.EPS.Device](../../aspose.page.eps.device)
* сборка [Aspose.Page](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Page.dll -->