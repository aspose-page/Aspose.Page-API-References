---
title: XpsGlyphs
second_title: Aspose.Page per riferimento all'API .NET
description: Caratteristiche dellelemento Glyphs che incapsulano la classe. Questo elemento rappresenta una sequenza di testo formattato uniformemente da un singolo font. Fornisce le informazioni necessarie per un rendering accurato e supporta la ricerca e le funzioni di selezione nella visualizzazione dei consumatori.
type: docs
weight: 3030
url: /it/net/aspose.page.xps.xpsmodel/xpsglyphs/
---
## XpsGlyphs class

Caratteristiche dell'elemento Glyphs che incapsulano la classe. Questo elemento rappresenta una sequenza di testo formattato uniformemente da un singolo font. Fornisce le informazioni necessarie per un rendering accurato e supporta la ricerca e le funzioni di selezione nella visualizzazione dei consumatori.

```csharp
public sealed class XpsGlyphs : XpsContentElement
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BidiLevel](../../aspose.page.xps.xpsmodel/xpsglyphs/bidilevel) { get; set; } | Restituisce/imposta il valore che specifica il livello di annidamento bidirezionale dell'algoritmo Unicode. I valori pari implicano il layout da sinistra a destra, i valori dispari implicano il layout da destra a sinistra. Il layout da destra a sinistra posiziona l'origine della corsa sul lato destro del primo glifo, con larghezze di avanzamento positive (che rappresentano gli avanzamenti a sinistra) posizionando i successivi glifi a sinistra del glifo precedente. |
| [Clip](../../aspose.page.xps.xpsmodel/xpscontentelement/clip) { get; set; } | Restituisce/imposta l'istanza della geometria del percorso che limita la regione di rendering dell'elemento. |
| [Count](../../aspose.page.xps.xpsmodel/xpselement/count) { get; } | Restituisce il numero di elementi figlio. |
| [Fill](../../aspose.page.xps.xpsmodel/xpsglyphs/fill) { get; set; } | Restituisce/imposta il pennello utilizzato per riempire la forma dei glifi renderizzati. |
| [Font](../../aspose.page.xps.xpsmodel/xpsglyphs/font) { get; } | Restituisce la risorsa del font per il font TrueType utilizzato per comporre il testo degli elementi. |
| [FontRenderingEmSize](../../aspose.page.xps.xpsmodel/xpsglyphs/fontrenderingemsize) { get; set; } | Restituisce/imposta la dimensione del carattere in unità di superficie del disegno, espressa come float in unità dello spazio di coordinate effettivo. |
| [HyperlinkTarget](../../aspose.page.xps.xpsmodel/xpshyperlinkelement/hyperlinktarget) { get; set; } | Restituisce/imposta l'oggetto di destinazione del collegamento ipertestuale. |
| [IsSideways](../../aspose.page.xps.xpsmodel/xpsglyphs/issideways) { get; set; } | Restituisce/imposta il valore che indica che un glifo è girato su un lato, con l'origine definita come il centro superiore del glifo non ruotato. |
| [Item](../../aspose.page.xps.xpsmodel/xpselement/item) { get; } | Fornisce l'accesso ai figli dell'elemento in base all'indice*i* . |
| [Opacity](../../aspose.page.xps.xpsmodel/xpscontentelement/opacity) { get; set; } | Restituisce/imposta il valore che definisce la trasparenza uniforme dell'elemento. |
| [OpacityMask](../../aspose.page.xps.xpsmodel/xpscontentelement/opacitymask) { get; set; } | Restituisce/imposta il pennello specificando una maschera di valori alfa che viene applicata all'elemento allo stesso modo dell'attributo Opacità, ma consentendo valori alfa diversi per aree diverse dell'elemento. |
| [OriginX](../../aspose.page.xps.xpsmodel/xpsglyphs/originx) { get; set; } | Restituisce/imposta la coordinata x del primo glifo nella corsa, in unità dello spazio di coordinate effettivo. |
| [OriginY](../../aspose.page.xps.xpsmodel/xpsglyphs/originy) { get; set; } | Restituisce/imposta la coordinata y del primo glifo nella corsa, in unità dello spazio di coordinate effettivo. |
| [RenderTransform](../../aspose.page.xps.xpsmodel/xpscontentelement/rendertransform) { get; set; } | Restituisce/imposta la matrice di trasformazione affine stabilendo un nuovo frame di coordinate per tutti gli attributi dell'elemento e per tutti gli elementi figlio (se presenti). |
| [StyleSimulations](../../aspose.page.xps.xpsmodel/xpsglyphs/stylesimulations) { get; set; } | Restituisce/imposta il valore specificando una simulazione di stile. |
| [UnicodeString](../../aspose.page.xps.xpsmodel/xpsglyphs/unicodestring) { get; set; } | Restituisce/imposta la stringa di testo resa dall'elemento Glyphs. Il testo è specificato come punti di codice Unicode. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Clone](../../aspose.page.xps.xpsmodel/xpsglyphs/clone)() | Clona questi glifi. |
| [GetEnumerator](../../aspose.page.xps.xpsmodel/xpselement/getenumerator)() | Implementazione diIEnumerable interfaccia. |

### Guarda anche

* class [XpsContentElement](../xpscontentelement)
* spazio dei nomi [Aspose.Page.XPS.XpsModel](../../aspose.page.xps.xpsmodel)
* assemblea [Aspose.Page](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Page.dll -->