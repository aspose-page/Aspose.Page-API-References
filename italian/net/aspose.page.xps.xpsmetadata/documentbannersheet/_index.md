---
title: DocumentBannerSheet
second_title: Aspose.Page per riferimento all'API .NET
description: Descrive il foglio banner da stampare per un particolare documento. Il foglio banner dovrebbe essere emesso sul default PageMediaSize./pagemediasize e utilizzando limpostazione predefinitaPageMediaType./pagemediatype . Il foglio banner dovrebbe anche essere isolato dal resto del lavoro. Ciò significa che qualsiasi opzione di finitura o lavorazione come DocumentDuplex./documentduplex DocumentStaple./documentstaple  oDocumentBinding./documentbinding non deve includere il foglio banner. Il foglio banner può essere isolato o meno dal resto del lavoro. Ciò significa che qualsiasi opzione di finitura o elaborazione del lavoro può includere il foglio banner del documento. Il foglio banner deve essere il primo foglio del documento. https //docs.microsoft.com/enus/windows/win32/printdocs/documentbannersheet
type: docs
weight: 470
url: /it/net/aspose.page.xps.xpsmetadata/documentbannersheet/
---
## DocumentBannerSheet class

Descrive il foglio banner da stampare per un particolare documento. Il foglio banner dovrebbe essere emesso sul default [`PageMediaSize`](../pagemediasize) e utilizzando l'impostazione predefinita[`PageMediaType`](../pagemediatype) . Il foglio banner dovrebbe anche essere isolato dal resto del lavoro. Ciò significa che qualsiasi opzione di finitura o lavorazione (come [`DocumentDuplex`](../documentduplex) ,[`DocumentStaple`](../documentstaple) , o[`DocumentBinding`](../documentbinding)) non deve includere il foglio banner. Il foglio banner può essere isolato o meno dal resto del lavoro. Ciò significa che qualsiasi opzione di finitura o elaborazione del lavoro può includere il foglio banner del documento. Il foglio banner deve essere il primo foglio del documento. https ://docs.microsoft.com/en-us/windows/win32/printdocs/documentbannersheet

```csharp
public sealed class DocumentBannerSheet : Feature, IDocumentPrintTicketItem, IJobPrintTicketItem
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [DocumentBannerSheet](documentbannersheet)(params BannerSheetOption[]) | Crea una nuova istanza. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Name](../../aspose.page.xps.xpsmetadata/printticketelement/name) { get; } | Ottiene il nome dell'elemento. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.page.xps.xpsmetadata/feature/add)(params IFeatureItem[]) | Aggiunge un elenco di elementi alla fine dell'elenco di elementi di questa funzione. Ognuno deve essere a[`Feature`](../feature) , un[`Option`](../option) o a[`Property`](../property) istanza. |

## Altri membri

| Nome | Descrizione |
| --- | --- |
| class [BannerSheetOption](documentbannersheet.bannersheetoption) | Rappresenta le opzioni del[`DocumentBannerSheet`](../documentbannersheet) caratteristica. |

### Guarda anche

* class [Feature](../feature)
* interface [IDocumentPrintTicketItem](../idocumentprintticketitem)
* interface [IJobPrintTicketItem](../ijobprintticketitem)
* spazio dei nomi [Aspose.Page.XPS.XpsMetadata](../../aspose.page.xps.xpsmetadata)
* assemblea [Aspose.Page](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Page.dll -->