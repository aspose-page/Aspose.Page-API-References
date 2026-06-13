---
title: "PdfSaveOptions"
second_title: "مرجع Aspose.Page لـ Java API"
description: "فئة لخيارات حفظ XPS كـ PDF."
type: docs
weight: 14
url: /ar/java/com.aspose.xps.rendering/pdfsaveoptions/
---
**Inheritance:**
java.lang.Object, [com.aspose.page.SaveOptions](../../com.aspose.page/saveoptions)

**All Implemented Interfaces:**
[com.aspose.page.IMultiPageSaveOptions](../../com.aspose.page/imultipagesaveoptions), [com.aspose.xps.rendering.IXpsTextConversionOptions](../../com.aspose.xps.rendering/ixpstextconversionoptions), [com.aspose.xps.rendering.IPipelineOptions](../../com.aspose.xps.rendering/ipipelineoptions), [com.aspose.xps.rendering.IEventBasedModificationOptions](../../com.aspose.xps.rendering/ieventbasedmodificationoptions)
```
public class PdfSaveOptions extends SaveOptions implements IMultiPageSaveOptions, IXpsTextConversionOptions, IPipelineOptions, IEventBasedModificationOptions
```

فئة لخيارات حفظ XPS كـ PDF.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | ينشئ مثلاً جديداً من الخيارات. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAdditionalFontsFolders()](#getAdditionalFontsFolders--) | يعيد مجلدات الخطوط الإضافية التي يجب على المحول العثور على الخطوط فيها للمستند المدخل. |
| [getBatchSize()](#getBatchSize--) | يعيد حجم جزء من الصفحات للانتقال من عقدة إلى عقدة أخرى. |
| [getBeforePageSavingEventHandlers()](#getBeforePageSavingEventHandlers--) | يعيد مجموعة معالجات الأحداث التي تقوم بتعديلات على صفحة XPS قبل حفظها مباشرةً. |
| [getClass()](#getClass--) |  |
| [getConvertFontsToTTF()](#getConvertFontsToTTF--) | يحصل على العلامة التي تُظهر ما إذا كان من الضروري حفظ الخطوط غير TrueType إلى TTF. |
| [getEncryptionDetails()](#getEncryptionDetails--) | يعيد تفاصيل التشفير. |
| [getExceptions()](#getExceptions--) | يعيد قائمة بالأخطاء غير الحرجة. |
| [getImageCompression()](#getImageCompression--) | يعيد نوع الضغط الذي سيُستخدم لجميع الصور في المستند. |
| [getJpegQualityLevel()](#getJpegQualityLevel--) | يعيد القيمة التي تحدد مستوى الضغط لصورة. |
| [getOutlineTreeExpansionLevel()](#getOutlineTreeExpansionLevel--) | يحصل على المستوى الذي يجب توسيع مخطط المستند إليه عند فتح ملف PDF في عارض. 1 - تُظهر عناصر المخطط المستوى الأول فقط، 2 - تُظهر عناصر المخطط المستوى الأول والثاني فقط، وهكذا. |
| [getOutlineTreeHeight()](#getOutlineTreeHeight--) | يحصل على ارتفاع شجرة مخطط المستند التي سيتم حفظها. 0 - لن يتم تحويل شجرة المخطط، 1 - سيتم تحويل عناصر المخطط المستوى الأول فقط، وهكذا. |
| [getPageNumbers()](#getPageNumbers--) | يحصل على مصفوفة أعداد الصفحات التي سيتم عرضها. |
| [getSize()](#getSize--) | يحصل على حجم الصفحة أو الصورة. |
| [getTextCompression()](#getTextCompression--) | يعيد نوع الضغط الذي سيُستخدم لجميع تدفقات المحتوى باستثناء الصور. |
| [hashCode()](#hashCode--) |  |
| [isDebug()](#isDebug--) | يحصل على العلامة التي تسمح بإخراج التحذيرات والرسائل أثناء التحويل. |
| [isSupressErrors()](#isSupressErrors--) | يعيد قيمة تشير إلى ما إذا كانت الأخطاء ستُقمع أثناء التحويل. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [preserveText()](#preserveText--) | في XPS، قد تحتوي بعض عناصر النص على مراجع لأشكال رموز بديلة لا تتطابق مع أي رمز حرف في الخط. |
| [preserveText(boolean value)](#preserveText-boolean-) | في XPS، قد تحتوي بعض عناصر النص على مراجع لأشكال رموز بديلة لا تتطابق مع أي رمز حرف في الخط. |
| [setAdditionalFontsFolders(String[] fontsFolders)](#setAdditionalFontsFolders-java.lang.String---) | يحدد مجلدات الخطوط الإضافية التي يجب على المحول العثور على الخطوط فيها للمستند المدخل. |
| [setBatchSize(int value)](#setBatchSize-int-) | يضبط حجم جزء من الصفحات للانتقال من عقدة إلى عقدة أخرى. |
| [setConvertFontsToTTF(boolean value)](#setConvertFontsToTTF-boolean-) | يحدد ما إذا كان سيتم حفظ الخطوط غير TrueType إلى TTF. |
| [setDebug(boolean debug)](#setDebug-boolean-) | يحدد العلامة التي تسمح بإخراج التحذيرات والرسائل أثناء التحويل. |
| [setEncryptionDetails(PdfEncryptionDetails value)](#setEncryptionDetails-com.aspose.xps.rendering.PdfEncryptionDetails-) | يضبط تفاصيل التشفير. |
| [setImageCompression(PdfImageCompression value)](#setImageCompression-com.aspose.xps.rendering.PdfImageCompression-) | يضبط نوع الضغط الذي سيُستخدم لجميع الصور في المستند. |
| [setJpegQualityLevel(int value)](#setJpegQualityLevel-int-) | يضبط القيمة التي تحدد مستوى الضغط للصورة. |
| [setOutlineTreeExpansionLevel(int value)](#setOutlineTreeExpansionLevel-int-) | يضبط المستوى الذي يجب توسيع مخطط المستند إليه عند فتح ملف PDF في عارض. 1 - تُظهر عناصر المخطط المستوى الأول فقط، 2 - تُظهر عناصر المخطط المستوى الأول والثاني فقط، وهكذا. |
| [setOutlineTreeHeight(int value)](#setOutlineTreeHeight-int-) | يضبط ارتفاع شجرة مخطط المستند التي سيتم حفظها. 0 - لن يتم تحويل شجرة المخطط، 1 - سيتم تحويل عناصر المخطط المستوى الأول فقط، وهكذا. |
| [setPageNumbers(int[] value)](#setPageNumbers-int---) | يضبط مصفوفة أعداد الصفحات التي سيتم عرضها. |
| [setSize(Dimension size)](#setSize-java.awt.Dimension-) | يحدد حجم الصفحة أو الصورة. |
| [setSupressErrors(boolean supressErrors)](#setSupressErrors-boolean-) | يحدد العلم الذي يشير إلى ما إذا كان سيتم قمع الأخطاء أثناء التحويل. |
| [setTextCompression(PdfTextCompression value)](#setTextCompression-com.aspose.xps.rendering.PdfTextCompression-) | يضبط نوع الضغط الذي سيُستخدم لجميع تدفقات المحتوى باستثناء الصور. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


ينشئ مثلاً جديداً من الخيارات.

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
### getAdditionalFontsFolders() {#getAdditionalFontsFolders--}
```
public String[] getAdditionalFontsFolders()
```


يرجع مجلدات الخطوط الإضافية التي يجب على المحول العثور على الخطوط فيها للمستند المدخل. المجلد الافتراضي هو مجلد الخطوط القياسي حيث يجد نظام التشغيل الخطوط للاستخدامات الداخلية.

**Returns:**
java.lang.String[] - مصفوفة من مجلدات الخطوط.
### getBatchSize() {#getBatchSize--}
```
public int getBatchSize()
```


يعيد حجم جزء من الصفحات للانتقال من عقدة إلى عقدة أخرى.

**Returns:**
int - حجم جزء من الصفحات للانتقال من عقدة إلى عقدة أخرى.
### getBeforePageSavingEventHandlers() {#getBeforePageSavingEventHandlers--}
```
public List<EventBasedModifications.BeforePageSavingEventHandler> getBeforePageSavingEventHandlers()
```


يعيد مجموعة معالجات الأحداث التي تقوم بتعديلات على صفحة XPS قبل حفظها مباشرةً.

**Returns:**
java.util.List<com.aspose.xps.features.EventBasedModifications.BeforePageSavingEventHandler> - مجموعة معالجات الأحداث التي تقوم بإجراء تعديلات على صفحة XPS قبل حفظها مباشرةً.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConvertFontsToTTF() {#getConvertFontsToTTF--}
```
public boolean getConvertFontsToTTF()
```


يحصل على العلامة التي تُظهر ما إذا كان من الضروري حفظ الخطوط غير TrueType إلى TTF.

**Returns:**
boolean - قيمة العلم.
### getEncryptionDetails() {#getEncryptionDetails--}
```
public PdfEncryptionDetails getEncryptionDetails()
```


يعيد تفاصيل التشفير. إذا لم يتم ضبطها، فلن يتم تنفيذ أي تشفير.

**Returns:**
[PdfEncryptionDetails](../../com.aspose.xps.rendering/pdfencryptiondetails) - The encryption details.
### getExceptions() {#getExceptions--}
```
public List<Exception> getExceptions()
```


يعيد قائمة بالأخطاء غير الحرجة.

**Returns:**
java.util.List<java.lang.Exception> - قائمة الاستثناءات
### getImageCompression() {#getImageCompression--}
```
public PdfImageCompression getImageCompression()
```


يعيد نوع الضغط الذي سيُستخدم لجميع الصور في المستند. القيمة الافتراضية هي PdfImageCompression.Auto .

**Returns:**
[PdfImageCompression](../../com.aspose.xps.rendering/pdfimagecompression) - The compression type.
### getJpegQualityLevel() {#getJpegQualityLevel--}
```
public int getJpegQualityLevel()
```


يعيد القيمة التي تحدد مستوى الضغط للصورة. القيم المتاحة من 0 إلى 100. كلما كان الرقم المحدد أقل، زاد الضغط وبالتالي انخفضت جودة الصورة. القيمة 0 تؤدي إلى أدنى جودة للصورة، بينما القيمة 100 تؤدي إلى أعلى جودة.

**Returns:**
int - القيمة التي تحدد مستوى الضغط للصورة.
### getOutlineTreeExpansionLevel() {#getOutlineTreeExpansionLevel--}
```
public int getOutlineTreeExpansionLevel()
```


يحصل على المستوى الذي يجب توسيع مخطط المستند إليه عند فتح ملف PDF في عارض. 1 - تُظهر عناصر المخطط المستوى الأول فقط، 2 - تُظهر عناصر المخطط المستوى الأول والثاني فقط، وهكذا.

**Returns:**
int - مستوى توسيع شجرة المخطط.
### getOutlineTreeHeight() {#getOutlineTreeHeight--}
```
public int getOutlineTreeHeight()
```


يحصل على ارتفاع شجرة مخطط المستند لحفظه. 0 - لن يتم تحويل شجرة المخطط، 1 - سيتم تحويل عناصر المستوى الأول فقط، وهكذا. القيمة الافتراضية هي 10.

**Returns:**
int - ارتفاع شجرة المخطط.
### getPageNumbers() {#getPageNumbers--}
```
public int[] getPageNumbers()
```


يحصل على مصفوفة أعداد الصفحات التي سيتم عرضها.

**Returns:**
int[] - أعداد الصفحات.
### getSize() {#getSize--}
```
public Dimension getSize()
```


يحصل على حجم الصفحة أو الصورة.

**Returns:**
java.awt.Dimension - حجم الصفحة أو الصورة.
### getTextCompression() {#getTextCompression--}
```
public PdfTextCompression getTextCompression()
```


يعيد نوع الضغط الذي سيُستخدم لجميع تدفقات المحتوى باستثناء الصور. القيمة الافتراضية هي PdfTextCompression.Flate .

**Returns:**
[PdfTextCompression](../../com.aspose.xps.rendering/pdftextcompression) - The compression type.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isDebug() {#isDebug--}
```
public boolean isDebug()
```


يحصل على العلامة التي تسمح بإخراج التحذيرات والرسائل أثناء التحويل.

**Returns:**
boolean - قيمة التصحيح.
### isSupressErrors() {#isSupressErrors--}
```
public boolean isSupressErrors()
```


يعيد قيمة تشير إلى ما إذا كانت الأخطاء ستُقمع أثناء التحويل.

**Returns:**
منطقي - قيمة منطقية
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### preserveText() {#preserveText--}
```
public boolean preserveText()
```


في XPS، قد تحتوي بعض عناصر النص على مراجع لأشكال رموز بديلة لا تتطابق مع أي رمز حرف في الخط. إذا تم تعيين هذه العلامة إلى true، يتم تحويل النص من هذه العناصر في XPS إلى أشكال رسومية. ثم يظهر النص نفسه شفافًا في الأعلى، مما يترك نص تلك العناصر قابلًا للتحديد. لكن الأثر الجانبي هو أن ملف الإخراج قد يصبح أكبر بكثير من الأصل. إذا تم تعيين العلامة إلى false، يتم استبدال الأحرف التي يجب عرضها كأشكال بديلة بأحرف أخرى تُطابق أشكال الرموز البديلة. وبالتالي يظل النص قابلًا للتحديد، لكنه سيتغير وربما يصبح غير قابل للقراءة.

**Returns:**
boolean - قيمة العلم.
### preserveText(boolean value) {#preserveText-boolean-}
```
public void preserveText(boolean value)
```


في XPS، قد تحتوي بعض عناصر النص على مراجع لأشكال رموز بديلة لا تتطابق مع أي رمز حرف في الخط. إذا تم تعيين هذه العلامة إلى true، يتم تحويل النص من هذه العناصر في XPS إلى أشكال رسومية. ثم يظهر النص نفسه شفافًا في الأعلى، مما يترك نص تلك العناصر قابلًا للتحديد. لكن الأثر الجانبي هو أن ملف الإخراج قد يصبح أكبر بكثير من الأصل. إذا تم تعيين العلامة إلى false، يتم استبدال الأحرف التي يجب عرضها كأشكال بديلة بأحرف أخرى تُطابق أشكال الرموز البديلة. وبالتالي يظل النص قابلًا للتحديد، لكنه سيتغير وربما يصبح غير قابل للقراءة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean | قيمة العلم. |

### setAdditionalFontsFolders(String[] fontsFolders) {#setAdditionalFontsFolders-java.lang.String---}
```
public void setAdditionalFontsFolders(String[] fontsFolders)
```


يحدد مجلدات الخطوط الإضافية التي يجب على المحول العثور على الخطوط فيها للمستند المدخل. المجلد الافتراضي هو مجلد الخطوط القياسي حيث يجد نظام التشغيل الخطوط للاستخدامات الداخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fontsFolders | java.lang.String[] | مصفوفة من مجلدات الخطوط. |

### setBatchSize(int value) {#setBatchSize-int-}
```
public void setBatchSize(int value)
```


يضبط حجم جزء من الصفحات للانتقال من عقدة إلى عقدة أخرى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | حجم جزء من الصفحات للانتقال من عقدة إلى أخرى. |

### setConvertFontsToTTF(boolean value) {#setConvertFontsToTTF-boolean-}
```
public void setConvertFontsToTTF(boolean value)
```


يحدد ما إذا كان سيتم حفظ الخطوط غير TrueType كـ TTF. هذا يقلل بشكل كبير من حجم المستند الناتج في تحويل PS إلى PDF ويزيد من سرعة تحويل ملفات PS التي تحتوي على كمية كبيرة من النص بخطوط غير TrueType إلى أي تنسيق إخراج. ومع ذلك، هناك إزاحة رأسية صغيرة للنص عند تحويل ملف PostScript إلى صورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean | قيمة العلم. |

### setDebug(boolean debug) {#setDebug-boolean-}
```
public void setDebug(boolean debug)
```


يحدد العلامة التي تسمح بإخراج التحذيرات والرسائل أثناء التحويل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| debug | boolean | قيمة منطقية. |

### setEncryptionDetails(PdfEncryptionDetails value) {#setEncryptionDetails-com.aspose.xps.rendering.PdfEncryptionDetails-}
```
public void setEncryptionDetails(PdfEncryptionDetails value)
```


يضبط تفاصيل التشفير. إذا لم يتم ضبطه، فلن يتم تنفيذ أي تشفير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [PdfEncryptionDetails](../../com.aspose.xps.rendering/pdfencryptiondetails) | تفاصيل التشفير. |

### setImageCompression(PdfImageCompression value) {#setImageCompression-com.aspose.xps.rendering.PdfImageCompression-}
```
public void setImageCompression(PdfImageCompression value)
```


يضبط نوع الضغط الذي سيُستخدم لجميع الصور في المستند. القيمة الافتراضية هي PdfImageCompression.Auto .

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [PdfImageCompression](../../com.aspose.xps.rendering/pdfimagecompression) | نوع الضغط. |

### setJpegQualityLevel(int value) {#setJpegQualityLevel-int-}
```
public void setJpegQualityLevel(int value)
```


يضبط القيمة التي تحدد مستوى الضغط للصورة. القيم المتاحة من 0 إلى 100. كلما كان الرقم المحدد أقل، زاد الضغط وبالتالي انخفضت جودة الصورة. القيمة 0 تؤدي إلى أدنى جودة للصورة، بينما القيمة 100 تؤدي إلى أعلى جودة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | القيمة التي تحدد مستوى الضغط للصورة. |

### setOutlineTreeExpansionLevel(int value) {#setOutlineTreeExpansionLevel-int-}
```
public void setOutlineTreeExpansionLevel(int value)
```


يضبط المستوى الذي يجب توسيع مخطط المستند إليه عند فتح ملف PDF في عارض. 1 - تُظهر عناصر المخطط المستوى الأول فقط، 2 - تُظهر عناصر المخطط المستوى الأول والثاني فقط، وهكذا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | مستوى توسيع شجرة المخطط. |

### setOutlineTreeHeight(int value) {#setOutlineTreeHeight-int-}
```
public void setOutlineTreeHeight(int value)
```


يضبط ارتفاع شجرة مخطط المستند التي سيتم حفظها. 0 - لن يتم تحويل شجرة المخطط، 1 - سيتم تحويل عناصر المخطط المستوى الأول فقط، وهكذا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | ارتفاع شجرة المخطط. |

### setPageNumbers(int[] value) {#setPageNumbers-int---}
```
public void setPageNumbers(int[] value)
```


يضبط مصفوفة أعداد الصفحات التي سيتم عرضها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int[] | عدد الصفحات. |

### setSize(Dimension size) {#setSize-java.awt.Dimension-}
```
public void setSize(Dimension size)
```


يحدد حجم الصفحة أو الصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الحجم | java.awt.Dimension | حجم الصفحة أو الصورة. |

### setSupressErrors(boolean supressErrors) {#setSupressErrors-boolean-}
```
public void setSupressErrors(boolean supressErrors)
```


يحدد العلم الذي يشير إلى ما إذا كان سيتم قمع الأخطاء أثناء التحويل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| supressErrors | boolean | قيمة منطقية. |

### setTextCompression(PdfTextCompression value) {#setTextCompression-com.aspose.xps.rendering.PdfTextCompression-}
```
public void setTextCompression(PdfTextCompression value)
```


يضبط نوع الضغط الذي سيُستخدم لجميع تدفقات المحتوى باستثناء الصور. القيمة الافتراضية هي PdfTextCompression.Flate .

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [PdfTextCompression](../../com.aspose.xps.rendering/pdftextcompression) | نوع الضغط. |

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

