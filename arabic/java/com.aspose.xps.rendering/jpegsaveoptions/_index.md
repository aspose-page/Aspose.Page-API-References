---
title: "JpegSaveOptions"
second_title: "مرجع Aspose.Page لـ Java API"
description: "فئة لخيارات حفظ XPS كـ JPEG."
type: docs
weight: 12
url: /ar/java/com.aspose.xps.rendering/jpegsaveoptions/
---
**Inheritance:**
java.lang.Object, [com.aspose.page.SaveOptions](../../com.aspose.page/saveoptions), [com.aspose.xps.rendering.ImageSaveOptions](../../com.aspose.xps.rendering/imagesaveoptions)
```
public class JpegSaveOptions extends ImageSaveOptions
```

فئة لخيارات حفظ XPS كـ JPEG.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [JpegSaveOptions()](#JpegSaveOptions--) | ينشئ مثلاً جديداً من الخيارات. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAdditionalFontsFolders()](#getAdditionalFontsFolders--) | يعيد مجلدات الخطوط الإضافية التي يجب على المحول العثور على الخطوط فيها للمستند المدخل. |
| [getBatchSize()](#getBatchSize--) | يعيد حجم جزء من الصفحات للانتقال من عقدة إلى عقدة أخرى. |
| [getBeforePageSavingEventHandlers()](#getBeforePageSavingEventHandlers--) | يعيد مجموعة معالجات الأحداث التي تقوم بتعديلات على صفحة XPS قبل حفظها مباشرةً. |
| [getClass()](#getClass--) |  |
| [getConvertFontsToTTF()](#getConvertFontsToTTF--) | يحصل على العلامة التي تُظهر ما إذا كان من الضروري حفظ الخطوط غير TrueType إلى TTF. |
| [getExceptions()](#getExceptions--) | يعيد قائمة بالأخطاء غير الحرجة. |
| [getImageSize()](#getImageSize--) | يحصل على حجم الصور الناتجة بالبكسل. |
| [getInterpolationMode()](#getInterpolationMode--) | يحصل على وضع الاستيفاء. |
| [getJpegQualityLevel()](#getJpegQualityLevel--) | يعيد القيمة التي تحدد مستوى الضغط لصورة. |
| [getPageNumbers()](#getPageNumbers--) | يحصل على مصفوفة أعداد الصفحات التي سيتم عرضها. |
| [getResolution()](#getResolution--) | يحصل على دقة الصورة. |
| [getSize()](#getSize--) | يحصل على حجم الصفحة أو الصورة. |
| [getSmoothingMode()](#getSmoothingMode--) | يحصل على وضع التنعيم. |
| [getTextRenderingHint()](#getTextRenderingHint--) | يحصل على تلميح عرض النص. |
| [hashCode()](#hashCode--) |  |
| [isDebug()](#isDebug--) | يحصل على العلامة التي تسمح بإخراج التحذيرات والرسائل أثناء التحويل. |
| [isSupressErrors()](#isSupressErrors--) | يعيد قيمة تشير إلى ما إذا كانت الأخطاء ستُقمع أثناء التحويل. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAdditionalFontsFolders(String[] fontsFolders)](#setAdditionalFontsFolders-java.lang.String---) | يحدد مجلدات الخطوط الإضافية التي يجب على المحول العثور على الخطوط فيها للمستند المدخل. |
| [setBatchSize(int value)](#setBatchSize-int-) | يضبط حجم جزء من الصفحات للانتقال من عقدة إلى عقدة أخرى. |
| [setConvertFontsToTTF(boolean value)](#setConvertFontsToTTF-boolean-) | يحدد ما إذا كان سيتم حفظ الخطوط غير TrueType إلى TTF. |
| [setDebug(boolean debug)](#setDebug-boolean-) | يحدد العلامة التي تسمح بإخراج التحذيرات والرسائل أثناء التحويل. |
| [setImageSize(Dimension value)](#setImageSize-java.awt.Dimension-) | يضبط حجم صور الإخراج بالبكسل. |
| [setInterpolationMode(InterpolationMode value)](#setInterpolationMode-com.aspose.xps.rendering.InterpolationMode-) | يضبط وضع الاستيفاء. |
| [setJpegQualityLevel(int value)](#setJpegQualityLevel-int-) | يضبط القيمة التي تحدد مستوى الضغط للصورة. |
| [setPageNumbers(int[] value)](#setPageNumbers-int---) | يضبط مصفوفة أعداد الصفحات التي سيتم عرضها. |
| [setResolution(float value)](#setResolution-float-) | يضبط دقة الصورة. |
| [setSize(Dimension size)](#setSize-java.awt.Dimension-) | يحدد حجم الصفحة أو الصورة. |
| [setSmoothingMode(SmoothingMode value)](#setSmoothingMode-com.aspose.xps.rendering.SmoothingMode-) | يضبط وضع التنعيم. |
| [setSupressErrors(boolean supressErrors)](#setSupressErrors-boolean-) | يحدد العلم الذي يشير إلى ما إذا كان سيتم قمع الأخطاء أثناء التحويل. |
| [setTextRenderingHint(TextRenderingHint value)](#setTextRenderingHint-com.aspose.xps.rendering.TextRenderingHint-) | يضبط تلميح عرض النص. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### JpegSaveOptions() {#JpegSaveOptions--}
```
public JpegSaveOptions()
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
java.util.List<com.aspose.xps.features.EventBasedModifications.BeforePageSavingEventHandler>
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
### getExceptions() {#getExceptions--}
```
public List<Exception> getExceptions()
```


يعيد قائمة بالأخطاء غير الحرجة.

**Returns:**
java.util.List<java.lang.Exception> - قائمة الاستثناءات
### getImageSize() {#getImageSize--}
```
public Dimension getImageSize()
```


يحصل على حجم الصور الناتجة بالبكسل.

**Returns:**
java.awt.Dimension - حجم صور الإخراج بالبكسل.
### getInterpolationMode() {#getInterpolationMode--}
```
public InterpolationMode getInterpolationMode()
```


يحصل على وضع الاستيفاء.

**Returns:**
[InterpolationMode](../../com.aspose.xps.rendering/interpolationmode) - The interpolation mode.
### getJpegQualityLevel() {#getJpegQualityLevel--}
```
public int getJpegQualityLevel()
```


يعيد القيمة التي تحدد مستوى الضغط للصورة. القيم المتاحة من 0 إلى 100. كلما كان الرقم المحدد أقل، زاد الضغط وبالتالي انخفضت جودة الصورة. القيمة 0 تؤدي إلى أدنى جودة للصورة، بينما القيمة 100 تؤدي إلى أعلى جودة.

**Returns:**
int - القيمة التي تحدد مستوى الضغط للصورة.
### getPageNumbers() {#getPageNumbers--}
```
public int[] getPageNumbers()
```


يحصل على مصفوفة أعداد الصفحات التي سيتم عرضها.

**Returns:**
int[] - أعداد الصفحات.
### getResolution() {#getResolution--}
```
public float getResolution()
```


يحصل على دقة الصورة.

**Returns:**
float - دقة الصورة.
### getSize() {#getSize--}
```
public Dimension getSize()
```


يحصل على حجم الصفحة أو الصورة.

**Returns:**
java.awt.Dimension - حجم الصفحة أو الصورة.
### getSmoothingMode() {#getSmoothingMode--}
```
public SmoothingMode getSmoothingMode()
```


يحصل على وضع التنعيم.

**Returns:**
[SmoothingMode](../../com.aspose.xps.rendering/smoothingmode) - The smoothing mode.
### getTextRenderingHint() {#getTextRenderingHint--}
```
public TextRenderingHint getTextRenderingHint()
```


يحصل على تلميح عرض النص.

**Returns:**
[TextRenderingHint](../../com.aspose.xps.rendering/textrenderinghint) - The text rendering hint.
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

### setImageSize(Dimension value) {#setImageSize-java.awt.Dimension-}
```
public void setImageSize(Dimension value)
```


يضبط حجم صور الإخراج بالبكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.awt.Dimension | حجم الصور الناتجة بالبكسل. |

### setInterpolationMode(InterpolationMode value) {#setInterpolationMode-com.aspose.xps.rendering.InterpolationMode-}
```
public void setInterpolationMode(InterpolationMode value)
```


يضبط وضع الاستيفاء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [InterpolationMode](../../com.aspose.xps.rendering/interpolationmode) | وضع الاستيفاء. |

### setJpegQualityLevel(int value) {#setJpegQualityLevel-int-}
```
public void setJpegQualityLevel(int value)
```


يضبط القيمة التي تحدد مستوى الضغط للصورة. القيم المتاحة من 0 إلى 100. كلما كان الرقم المحدد أقل، زاد الضغط وبالتالي انخفضت جودة الصورة. القيمة 0 تؤدي إلى أدنى جودة للصورة، بينما القيمة 100 تؤدي إلى أعلى جودة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | القيمة التي تحدد مستوى الضغط للصورة. |

### setPageNumbers(int[] value) {#setPageNumbers-int---}
```
public void setPageNumbers(int[] value)
```


يضبط مصفوفة أعداد الصفحات التي سيتم عرضها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int[] | عدد الصفحات. |

### setResolution(float value) {#setResolution-float-}
```
public void setResolution(float value)
```


يضبط دقة الصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float | دقة الصورة. |

### setSize(Dimension size) {#setSize-java.awt.Dimension-}
```
public void setSize(Dimension size)
```


يحدد حجم الصفحة أو الصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الحجم | java.awt.Dimension | حجم الصفحة أو الصورة. |

### setSmoothingMode(SmoothingMode value) {#setSmoothingMode-com.aspose.xps.rendering.SmoothingMode-}
```
public void setSmoothingMode(SmoothingMode value)
```


يضبط وضع التنعيم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [SmoothingMode](../../com.aspose.xps.rendering/smoothingmode) | وضع التنعيم. |

### setSupressErrors(boolean supressErrors) {#setSupressErrors-boolean-}
```
public void setSupressErrors(boolean supressErrors)
```


يحدد العلم الذي يشير إلى ما إذا كان سيتم قمع الأخطاء أثناء التحويل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| supressErrors | boolean | قيمة منطقية. |

### setTextRenderingHint(TextRenderingHint value) {#setTextRenderingHint-com.aspose.xps.rendering.TextRenderingHint-}
```
public void setTextRenderingHint(TextRenderingHint value)
```


يضبط تلميح عرض النص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [TextRenderingHint](../../com.aspose.xps.rendering/textrenderinghint) | تلميح عرض النص. |

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

