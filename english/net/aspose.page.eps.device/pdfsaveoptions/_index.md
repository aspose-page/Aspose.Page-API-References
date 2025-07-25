---
title: Class PdfSaveOptions
second_title: Aspose.Page for .NET API Reference
description: Aspose.Page.EPS.Device.PdfSaveOptions class. This class contains input and output streams and other options necessary for managing conversion process
type: docs
weight: 90
url: /net/aspose.page.eps.device/pdfsaveoptions/
---
## PdfSaveOptions class

This class contains input and output streams and other options necessary for managing conversion process.

```csharp
public class PdfSaveOptions : SaveOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/#constructor)() | Initializes a new instance of the `PdfSaveOptions` class with default values for flags !:SuppressErrors (true) and !:Debug (false). |
| [PdfSaveOptions](pdfsaveoptions/#constructor_2)(bool) | Initializes a new instance of the `PdfSaveOptions` class with default values for flag !:Debug (false). |
| [PdfSaveOptions](pdfsaveoptions/#constructor_1)(Size) | Initializes a new instance of the `PdfSaveOptions` with with specified size of the page. |
| [PdfSaveOptions](pdfsaveoptions/#constructor_3)(bool, Size) | Initializes a new instance of the `PdfSaveOptions` class with default values for flag !:Debug (false) and with specified size of the page. |

## Properties

| Name | Description |
| --- | --- |
| [AdditionalFontsFolders](../../aspose.page/saveoptions/additionalfontsfolders/) { get; set; } | Specifies additional folders where converter should find fonts for input document. Default folder are standard fonts folder where OS finds fonts for internal needs. |
| virtual [ConvertFontsToTTF](../../aspose.page/saveoptions/convertfontstottf/) { get; set; } | Specifies whether to save non-TrueType fonts to TTF. It significantly decreases the volume of the resulting document in PS to PDF conversion and increases the speed of conversion of PS files with a large quantity of text in non-TrueType fonts to any output format. However there is small vertical shift of text when converting PostSctipt file to image. |
| virtual [Debug](../../aspose.page/saveoptions/debug/) { get; set; } | Specifies whether debug information must be printed to standard output stream or not. |
| virtual [Exceptions](../../aspose.page/saveoptions/exceptions/) { get; } | Returns a list of suppressed conversion errors If !:SuppressErrors is true. |
| [JpegQualityLevel](../../aspose.page/saveoptions/jpegqualitylevel/) { get; set; } | The Quality category specifies the level of compression for an image. Available values are 0 to 100. The lower the number specified, the higher the compression and therefore the lower the quality of the image. 0 value results in lowest quality image, while 100 results in highest. |
| [Size](../../aspose.page/saveoptions/size/) { get; set; } | Gets/sets the size of the image. |
| virtual [SupressErrors](../../aspose.page/saveoptions/supresserrors/) { get; set; } | Specifies whether errors must be suppressed or not. If true suppressed errors are added to [`Exceptions`](../../aspose.page/saveoptions/exceptions/) list. If false the first error will terminate the program. |

### See Also

* class [SaveOptions](../../aspose.page/saveoptions/)
* namespace [Aspose.Page.EPS.Device](../../aspose.page.eps.device/)
* assembly [Aspose.Page](../../)


