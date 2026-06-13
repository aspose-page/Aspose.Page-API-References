---
title: "PageMediaType.PageMediaTypeOption"
second_title: "مرجع Aspose.Page لـ Java API"
description: "يصف خيارات ميزة PageMediaType."
type: docs
weight: 13
url: /ar/java/com.aspose.xps.metadata/pagemediatype.pagemediatypeoption/
---
**Inheritance:**
java.lang.Object, [com.aspose.xps.metadata.PrintTicketElement](../../com.aspose.xps.metadata/printticketelement), [com.aspose.xps.metadata.CompositePrintTicketElement](../../com.aspose.xps.metadata/compositeprintticketelement), [com.aspose.xps.metadata.Option](../../com.aspose.xps.metadata/option)

**All Implemented Interfaces:**
[com.aspose.xps.metadata.PageMediaType.IPageMediaTypeItem](../../com.aspose.xps.metadata/ipagemediatypeitem)
```
public static final class PageMediaType.PageMediaTypeOption extends Option implements PageMediaType.IPageMediaTypeItem
```

يصف خيارات ميزة PageMediaType.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [PageMediaTypeOption(String optionName, PageMediaType.IPageMediaTypeOptionItem[] items)](#PageMediaTypeOption-java.lang.String-com.aspose.xps.metadata.PageMediaType.IPageMediaTypeOptionItem...-) | ينشئ نسخة جديدة. |
| [PageMediaTypeOption(PageMediaType.PageMediaTypeOption option)](#PageMediaTypeOption-com.aspose.xps.metadata.PageMediaType.PageMediaTypeOption-) | ينسخ هذا المثيل من الخيار. |
## الحقول

| حقل | الوصف |
| --- | --- |
| [Archival](#Archival) | يحدد وسائط بجودة أرشيفية. |
| [AutoSelect](#AutoSelect) | يحدد أن الوسائط سيتم اختيارها تلقائيًا. |
| [BackPrintFilm](#BackPrintFilm) | يحدد وسائط فيلم طباعة خلفية متخصصة. |
| [Bond](#Bond) | يحدد وسائط رابطة قياسية. |
| [CardStock](#CardStock) | يحدد وسائط ورق بطاقة قياسي. |
| [Continous](#Continous) | يحدد وسائط تغذية مستمرة. |
| [EnvelopePlain](#EnvelopePlain) | يحدد وسائط ظرف قياسي. |
| [EnvelopeWindow](#EnvelopeWindow) | يحدد وسائط ظرف بنفذة. |
| [Fabric](#Fabric) | يحدد وسائط قماشية. |
| [HighResolution](#HighResolution) | يحدد وسائط عالية الدقة متخصصة. |
| [Label](#Label) | يحدد وسائط ملصق. |
| [MultiLayerForm](#MultiLayerForm) | يحدد وسائط نماذج متعددة الأجزاء مرفقة. |
| [MultiPartForm](#MultiPartForm) | يحدد وسائط نماذج متعددة الأجزاء منفصلة. |
| [None](#None) | يحدد وسائط غير معروفة أو غير مدرجة. |
| [Photographic](#Photographic) | يحدد وسائط تصوير فوتوغرافي قياسية. |
| [PhotographicFilm](#PhotographicFilm) | يحدد وسائط تصوير فوتوغرافي فيلمية. |
| [PhotographicGlossy](#PhotographicGlossy) | يحدد وسائط تصوير فوتوغرافي لامعة. |
| [PhotographicHighGloss](#PhotographicHighGloss) | يحدد وسائط تصوير فوتوغرافي ذات لمعان عالي. |
| [PhotographicMatte](#PhotographicMatte) | يحدد وسائط تصوير فوتوغرافي غير لامعة. |
| [PhotographicSatin](#PhotographicSatin) | يحدد وسائط تصوير فوتوغرافي ساتان. |
| [PhotographicSemiGloss](#PhotographicSemiGloss) | يحدد وسائط تصوير فوتوغرافي شبه لامعة. |
| [Plain](#Plain) | يحدد وسائط ورق قياسية. |
| [Screen](#Screen) | يحدد الإخراج إلى عرض مخرجات بصيغة مستمرة. |
| [ScreenPaged](#ScreenPaged) | يحدد الإخراج إلى عرض مخرجات بصيغة صفحات. |
| [Stationary](#Stationary) | يحدد وسائط قرطاسية متخصصة. |
| [TShirtTransfer](#TShirtTransfer) | يحدد وسائط نقل القمصان المتخصصة. |
| [TabStockFull](#TabStockFull) | يحدد وسائط مخزون علامات التبويب التي لم تُقطع مسبقًا (علامات تبويب فردية). |
| [TabStockPreCut](#TabStockPreCut) | يحدد وسائط مخزون علامات التبويب التي تم قطعها مسبقًا (عدة علامات تبويب). |
| [Transparency](#Transparency) | يحدد وسائط الشفافية. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(IOptionItem[] items)](#add-com.aspose.xps.metadata.IOptionItem...-) | يضيف قائمة من العناصر إلى نهاية قائمة العناصر لهذا الخيار. |
| [add(PageMediaType.IPageMediaTypeOptionItem[] items)](#add-com.aspose.xps.metadata.PageMediaType.IPageMediaTypeOptionItem...-) | يضيف مصفوفة من كائنات  IPageMediaTypeOptionItem  إلى الخيار. |
| [clone()](#clone--) | ينسخ هذا المثيل من الخيار. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | يحصل على اسم العنصر. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setWeight(int weight)](#setWeight-int-) | يضبط قيمة خاصية  Weight  المُقيمة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PageMediaTypeOption(String optionName, PageMediaType.IPageMediaTypeOptionItem[] items) {#PageMediaTypeOption-java.lang.String-com.aspose.xps.metadata.PageMediaType.IPageMediaTypeOptionItem...-}
```
public PageMediaTypeOption(String optionName, PageMediaType.IPageMediaTypeOptionItem[] items)
```


ينشئ نسخة جديدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| optionName | java.lang.String | اسم خيار. |
| items | [IPageMediaTypeOptionItem\[\]](../../com.aspose.xps.metadata/ipagemediatypeoptionitem) | مصفوفة عشوائية من كائنات  IPageMediaTypeOptionItem . |

### PageMediaTypeOption(PageMediaType.PageMediaTypeOption option) {#PageMediaTypeOption-com.aspose.xps.metadata.PageMediaType.PageMediaTypeOption-}
```
public PageMediaTypeOption(PageMediaType.PageMediaTypeOption option)
```


ينسخ هذا المثيل من الخيار.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| option | [PageMediaTypeOption](../../com.aspose.xps.metadata/pagemediatypeoption) | كائن للاستنساخ. |

### Archival {#Archival}
```
public static PageMediaType.PageMediaTypeOption Archival
```


يحدد وسائط بجودة أرشيفية.

### AutoSelect {#AutoSelect}
```
public static PageMediaType.PageMediaTypeOption AutoSelect
```


يحدد أن الوسائط سيتم اختيارها تلقائيًا.

### BackPrintFilm {#BackPrintFilm}
```
public static PageMediaType.PageMediaTypeOption BackPrintFilm
```


يحدد وسائط فيلم طباعة خلفية متخصصة.

### Bond {#Bond}
```
public static PageMediaType.PageMediaTypeOption Bond
```


يحدد وسائط رابطة قياسية.

### CardStock {#CardStock}
```
public static PageMediaType.PageMediaTypeOption CardStock
```


يحدد وسائط ورق بطاقة قياسي.

### Continous {#Continous}
```
public static PageMediaType.PageMediaTypeOption Continous
```


يحدد وسائط تغذية مستمرة.

### EnvelopePlain {#EnvelopePlain}
```
public static PageMediaType.PageMediaTypeOption EnvelopePlain
```


يحدد وسائط ظرف قياسي.

### EnvelopeWindow {#EnvelopeWindow}
```
public static PageMediaType.PageMediaTypeOption EnvelopeWindow
```


يحدد وسائط ظرف بنفذة.

### Fabric {#Fabric}
```
public static PageMediaType.PageMediaTypeOption Fabric
```


يحدد وسائط قماشية.

### HighResolution {#HighResolution}
```
public static PageMediaType.PageMediaTypeOption HighResolution
```


يحدد وسائط عالية الدقة متخصصة.

### Label {#Label}
```
public static PageMediaType.PageMediaTypeOption Label
```


يحدد وسائط ملصق.

### MultiLayerForm {#MultiLayerForm}
```
public static PageMediaType.PageMediaTypeOption MultiLayerForm
```


يحدد وسائط نماذج متعددة الأجزاء مرفقة.

### MultiPartForm {#MultiPartForm}
```
public static PageMediaType.PageMediaTypeOption MultiPartForm
```


يحدد وسائط نماذج متعددة الأجزاء منفصلة.

### None {#None}
```
public static PageMediaType.PageMediaTypeOption None
```


يحدد وسائط غير معروفة أو غير مدرجة.

### Photographic {#Photographic}
```
public static PageMediaType.PageMediaTypeOption Photographic
```


يحدد وسائط تصوير فوتوغرافي قياسية.

### PhotographicFilm {#PhotographicFilm}
```
public static PageMediaType.PageMediaTypeOption PhotographicFilm
```


يحدد وسائط تصوير فوتوغرافي فيلمية.

### PhotographicGlossy {#PhotographicGlossy}
```
public static PageMediaType.PageMediaTypeOption PhotographicGlossy
```


يحدد وسائط تصوير فوتوغرافي لامعة.

### PhotographicHighGloss {#PhotographicHighGloss}
```
public static PageMediaType.PageMediaTypeOption PhotographicHighGloss
```


يحدد وسائط تصوير فوتوغرافي ذات لمعان عالي.

### PhotographicMatte {#PhotographicMatte}
```
public static PageMediaType.PageMediaTypeOption PhotographicMatte
```


يحدد وسائط تصوير فوتوغرافي غير لامعة.

### PhotographicSatin {#PhotographicSatin}
```
public static PageMediaType.PageMediaTypeOption PhotographicSatin
```


يحدد وسائط تصوير فوتوغرافي ساتان.

### PhotographicSemiGloss {#PhotographicSemiGloss}
```
public static PageMediaType.PageMediaTypeOption PhotographicSemiGloss
```


يحدد وسائط تصوير فوتوغرافي شبه لامعة.

### Plain {#Plain}
```
public static PageMediaType.PageMediaTypeOption Plain
```


يحدد وسائط ورق قياسية.

### Screen {#Screen}
```
public static PageMediaType.PageMediaTypeOption Screen
```


يحدد الإخراج إلى عرض مخرجات بصيغة مستمرة.

### ScreenPaged {#ScreenPaged}
```
public static PageMediaType.PageMediaTypeOption ScreenPaged
```


يحدد الإخراج إلى عرض مخرجات بصيغة صفحات.

### Stationary {#Stationary}
```
public static PageMediaType.PageMediaTypeOption Stationary
```


يحدد وسائط قرطاسية متخصصة.

### TShirtTransfer {#TShirtTransfer}
```
public static PageMediaType.PageMediaTypeOption TShirtTransfer
```


يحدد وسائط نقل القمصان المتخصصة.

### TabStockFull {#TabStockFull}
```
public static PageMediaType.PageMediaTypeOption TabStockFull
```


يحدد وسائط مخزون علامات التبويب التي لم تُقطع مسبقًا (علامات تبويب فردية).

### TabStockPreCut {#TabStockPreCut}
```
public static PageMediaType.PageMediaTypeOption TabStockPreCut
```


يحدد وسائط مخزون علامات التبويب التي تم قطعها مسبقًا (عدة علامات تبويب).

### Transparency {#Transparency}
```
public static PageMediaType.PageMediaTypeOption Transparency
```


يحدد وسائط الشفافية.

### add(IOptionItem[] items) {#add-com.aspose.xps.metadata.IOptionItem...-}
```
public void add(IOptionItem[] items)
```


يضيف قائمة من العناصر إلى نهاية قائمة العناصر لهذا الخيار. يجب أن يكون كل عنصر إما  ScoredProperty  أو  Property  مثيل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| items | [IOptionItem\[\]](../../com.aspose.xps.metadata/ioptionitem) | قائمة العناصر للإضافة. |

### add(PageMediaType.IPageMediaTypeOptionItem[] items) {#add-com.aspose.xps.metadata.PageMediaType.IPageMediaTypeOptionItem...-}
```
public PageMediaType.PageMediaTypeOption add(PageMediaType.IPageMediaTypeOptionItem[] items)
```


يضيف مصفوفة من كائنات  IPageMediaTypeOptionItem  إلى الخيار.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| items | [IPageMediaTypeOptionItem\[\]](../../com.aspose.xps.metadata/ipagemediatypeoptionitem) | مصفوفة عشوائية من كائنات  IPageMediaTypeOptionItem . |

**Returns:**
[PageMediaTypeOption](../../com.aspose.xps.metadata/pagemediatypeoption) - This options instance.
### clone() {#clone--}
```
public PageMediaType.PageMediaTypeOption clone()
```


ينسخ هذا الكائن الخيار. الاختصار إلى مُنشئ النسخ.

**Returns:**
[PageMediaTypeOption](../../com.aspose.xps.metadata/pagemediatypeoption) - The clone of this option instance.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getName() {#getName--}
```
public String getName()
```


يحصل على اسم العنصر.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setWeight(int weight) {#setWeight-int-}
```
public PageMediaType.PageMediaTypeOption setWeight(int weight)
```


يضبط قيمة خاصية  Weight  المُقيمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الوزن | int | قيمة خاصية  Weight  المُقيمة. |

**Returns:**
[PageMediaTypeOption](../../com.aspose.xps.metadata/pagemediatypeoption) - This option instance.
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

