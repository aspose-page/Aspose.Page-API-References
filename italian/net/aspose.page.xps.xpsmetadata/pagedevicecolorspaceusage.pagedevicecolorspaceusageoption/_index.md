---
title: PageDeviceColorSpaceUsage.PageDeviceColorSpaceUsageOption
second_title: Aspose.Page per riferimento all'API .NET
description: Descrive ilPageDeviceColorSpaceUsage./pagedevicecolorspaceusage opzioni delle funzioni.
type: docs
weight: 1880
url: /it/net/aspose.page.xps.xpsmetadata/pagedevicecolorspaceusage.pagedevicecolorspaceusageoption/
---
## PageDeviceColorSpaceUsage.PageDeviceColorSpaceUsageOption class

Descrive il[`PageDeviceColorSpaceUsage`](../pagedevicecolorspaceusage) opzioni delle funzioni.

```csharp
public sealed class PageDeviceColorSpaceUsageOption : Option
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Name](../../aspose.page.xps.xpsmetadata/printticketelement/name) { get; } | Ottiene il nome dell'elemento. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.page.xps.xpsmetadata/option/add)(params IOptionItem[]) | Aggiunge un elenco di elementi alla fine dell'elenco di elementi di questa opzione. Ognuno deve essere a[`ScoredProperty`](../scoredproperty) o[`Property`](../property) istanza. |

## Campi

| Nome | Descrizione |
| --- | --- |
| static [MatchToDefault](../../aspose.page.xps.xpsmetadata/pagedevicecolorspaceusageoption/matchtodefault) | Se il dispositivo determina che il profilo specificato da[`PageDeviceColorSpaceProfileURI`](../pagedevicecolorspaceprofileuri) parametro può essere utilizzato come profilo dello spazio colore del dispositivo, tutti gli elementi che utilizzano lo stesso profilo vengono trattati come già specificati nello spazio colore del dispositivo. Tutti gli altri elementi DEVONO utilizzare il profilo specificato per quell'elemento. Se il profilo non può essere utilizzato come profilo dello spazio colore del dispositivo, gli elementi che utilizzano il profilo DEVONO essere gestiti del colore come qualsiasi altro elemento che utilizza il profilo colore. |
| static [OverrideDeviceDefault](../../aspose.page.xps.xpsmetadata/pagedevicecolorspaceusageoption/overridedevicedefault) | Se il profilo specificato dal parametro PageDeviceColorSpaceProfileURI ha un numero di canali che corrispondono al numero di primari del dispositivo, DOVREBBE essere utilizzato al posto della gestione del colore interna dei dispositivi per tutti gli elementi. Gli elementi che utilizzano questo profilo si presume siano nel colore del dispositivo spazio e non verrà ulteriormente gestito il colore. |

### Guarda anche

* class [Option](../option)
* class [PageDeviceColorSpaceUsage](../pagedevicecolorspaceusage)
* spazio dei nomi [Aspose.Page.XPS.XpsMetadata](../../aspose.page.xps.xpsmetadata)
* assemblea [Aspose.Page](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Page.dll -->