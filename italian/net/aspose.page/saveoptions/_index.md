---
title: SaveOptions
second_title: Aspose.Page per riferimento all'API .NET
description: Questa classe contiene le opzioni necessarie per la gestione del processo di conversione.
type: docs
weight: 240
url: /it/net/aspose.page/saveoptions/
---
## SaveOptions class

Questa classe contiene le opzioni necessarie per la gestione del processo di conversione.

```csharp
public abstract class SaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SaveOptions](saveoptions#constructor)() | Inizializza una nuova istanza di[`SaveOptions`](../saveoptions) classe con valori predefiniti per i flag!:SuppressErrors (vero) e[`Debug`](./debug) (falso). |
| [SaveOptions](saveoptions#constructor_1)(bool) | Inizializza una nuova istanza di[`SaveOptions`](../saveoptions) classe con valore predefinito per flag[`Debug`](./debug) (falso). |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AdditionalFontsFolders](../../aspose.page/saveoptions/additionalfontsfolders) { get; set; } | Specifica le cartelle aggiuntive in cui il convertitore deve trovare i caratteri per il documento di input. La cartella predefinita è una cartella dei caratteri standard in cui il sistema operativo trova i caratteri per le esigenze interne. |
| virtual [Debug](../../aspose.page/saveoptions/debug) { get; set; } | Specifica se le informazioni di debug devono essere stampate o meno sul flusso di output standard. |
| virtual [Exceptions](../../aspose.page/saveoptions/exceptions) { get; } | Restituisce un elenco di errori di conversione soppressi If!:SuppressErrors è vero. |
| [JpegQualityLevel](../../aspose.page/saveoptions/jpegqualitylevel) { get; set; } | La categoria Qualità specifica il livello di compressione per un'immagine. I valori disponibili sono compresi tra 0 e 100. Più basso è il numero specificato, maggiore è la compressione e quindi minore è la qualità dell'immagine. Il valore 0 restituisce la qualità dell'immagine più bassa, mentre 100 restituisce la più alta. |
| virtual [SupressErrors](../../aspose.page/saveoptions/supresserrors) { get; set; } | Specifica se gli errori devono essere soppressi o meno. Se vengono aggiunti veri errori soppressi a[`Exceptions`](./exceptions) list. Se false il primo errore terminerà il programma. |

### Guarda anche

* spazio dei nomi [Aspose.Page](../../aspose.page)
* assemblea [Aspose.Page](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Page.dll -->