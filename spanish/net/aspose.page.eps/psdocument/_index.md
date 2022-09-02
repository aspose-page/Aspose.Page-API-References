---
title: PsDocument
second_title: Referencia de la API de Aspose.Page para .NET
description: Esta clase encapsula documentos PS/EPS.
type: docs
weight: 100
url: /es/net/aspose.page.eps/psdocument/
---
## PsDocument class

Esta clase encapsula documentos PS/EPS.

```csharp
public sealed class PsDocument : Document
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PsDocument](psdocument)(Stream) | Inicializa[`PsDocument`](../psdocument) con un flujo de archivo PS/EPS. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [NumberOfPages](../../aspose.page.eps/psdocument/numberofpages) { get; } | Devuelve el número de páginas del documento PDF resultante. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetXmpMetadata](../../aspose.page.eps/psdocument/getxmpmetadata)() | Lee el archivo PS/EPS y extrae XmpMetdata si ya existe o agrega uno nuevo si no existe. |
| [Merge](../../aspose.page.eps/psdocument/merge)(string[], Device, SaveOptions) | Fusiona archivos PS/EPS en un dispositivo. |
| [Save](../../aspose.page.eps/psdocument/save#save_1)(Stream) | Guardados dados[`PsDocument`](../psdocument) como archivo EPS. Este método se usa solo después de actualizar los metadatos XMP. Guarda el archivo EPS inicial con los metadatos existentes actualizados o uno nuevo creado al llamar al método GetMetadata. En el último caso, se agrega todo el código PostScript y los comentarios EPS necesarios. |
| override [Save](../../aspose.page.eps/psdocument/save#save)(Device, SaveOptions) | Guarda el archivo PS/EPS en un dispositivo. |
| static [SaveImageAsEps](../../aspose.page.eps/psdocument/saveimageaseps#saveimageaseps)(Bitmap, Stream, PsSaveOptions) | Guarda el objeto de mapa de bits en el flujo de salida EPS. |
| static [SaveImageAsEps](../../aspose.page.eps/psdocument/saveimageaseps#saveimageaseps_1)(Bitmap, string, PsSaveOptions) | Guarda el objeto de mapa de bits en un archivo EPS. |
| static [SaveImageAsEps](../../aspose.page.eps/psdocument/saveimageaseps#saveimageaseps_2)(Stream, Stream, PsSaveOptions) | Guarda la imagen PNG/JPEG/TIFF/BMP/GIF/EMF del flujo de entrada al flujo de salida EPS. |
| static [SaveImageAsEps](../../aspose.page.eps/psdocument/saveimageaseps#saveimageaseps_3)(string, string, PsSaveOptions) | Guarda la imagen PNG/JPEG/TIFF/BMP/GIF/EMF de un archivo a un archivo EPS. |

### Ver también

* class [Document](../../aspose.page/document)
* espacio de nombres [Aspose.Page.EPS](../../aspose.page.eps)
* asamblea [Aspose.Page](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Page.dll -->