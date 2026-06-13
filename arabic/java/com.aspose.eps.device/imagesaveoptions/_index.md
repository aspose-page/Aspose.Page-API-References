---
title: "ImageSaveOptions"
second_title: "مرجع Aspose.Page لـ Java API"
description: "تحتوي هذه الفئة على الخيارات اللازمة لإدارة عملية التحويل."
type: docs
weight: 10
url: /ar/java/com.aspose.eps.device/imagesaveoptions/
---
**Inheritance:**
java.lang.Object, [com.aspose.page.SaveOptions](../../com.aspose.page/saveoptions)
```
public class ImageSaveOptions extends SaveOptions
```

تحتوي هذه الفئة على الخيارات اللازمة لإدارة عملية التحويل.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [ImageSaveOptions()](#ImageSaveOptions--) | إنشاء نسخة جديدة من فئة  ImageSaveOptions  مع القيم الافتراضية للعلامات  suppressErrors  (true) و  debug  (false). |
| [ImageSaveOptions(ImageFormat imageFormat)](#ImageSaveOptions-com.aspose.page.ImageFormat-) | يُنشئ نسخة جديدة من  ImageSaveOptions  بالتنسيق المحدد للصورة. |
| [ImageSaveOptions(Dimension size)](#ImageSaveOptions-java.awt.Dimension-) | يُنشئ نسخة جديدة من  ImageSaveOptions  بالحجم المحدد للصورة. |
| [ImageSaveOptions(Dimension size, ImageFormat imageFormat)](#ImageSaveOptions-java.awt.Dimension-com.aspose.page.ImageFormat-) | يُنشئ نسخة جديدة من  ImageSaveOptions  بالحجم المحدد للصورة وتنسيق الصورة. |
| [ImageSaveOptions(ImageFormat imageFormat, boolean supressErrors)](#ImageSaveOptions-com.aspose.page.ImageFormat-boolean-) | يُنشئ نسخة جديدة من  ImageSaveOptions  بالتنسيق المحدد للصورة وعلامة suppressErrors. |
| [ImageSaveOptions(Dimension size, boolean supressErrors)](#ImageSaveOptions-java.awt.Dimension-boolean-) | يُنشئ نسخة جديدة من  ImageSaveOptions  بالحجم المحدد للصورة وعلامة suppressErrors. |
| [ImageSaveOptions(Dimension size, ImageFormat imageFormat, boolean supressErrors)](#ImageSaveOptions-java.awt.Dimension-com.aspose.page.ImageFormat-boolean-) | يُنشئ نسخة جديدة من  ImageSaveOptions  بالحجم المحدد للصورة، وتنسيق الصورة، وعلامة suppressErrors. |
| [ImageSaveOptions(boolean supressErrors)](#ImageSaveOptions-boolean-) | إنشاء نسخة جديدة من فئة  ImageSaveOptions  مع القيم الافتراضية للعلامة  debug  (false). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAdditionalFontsFolders()](#getAdditionalFontsFolders--) | يعيد مجلدات الخطوط الإضافية التي يجب على المحول العثور على الخطوط فيها للمستند المدخل. |
| [getClass()](#getClass--) |  |
| [getConvertFontsToTTF()](#getConvertFontsToTTF--) | يحصل على العلامة التي تُظهر ما إذا كان من الضروري حفظ الخطوط غير TrueType إلى TTF. |
| [getExceptions()](#getExceptions--) | يعيد قائمة بالأخطاء غير الحرجة. |
| [getImageFormat()](#getImageFormat--) | يحصل على تنسيق الصورة الناتجة. |
| [getJpegQualityLevel()](#getJpegQualityLevel--) | يعيد القيمة التي تحدد مستوى الضغط لصورة. |
| [getResolution()](#getResolution--) | يعيد دقة الصورة الناتجة. |
| [getSize()](#getSize--) | يحصل على حجم الصفحة أو الصورة. |
| [getSmoothingMode()](#getSmoothingMode--) | يحصل على وضع التنعيم. |
| [getTryJoinImageFragments()](#getTryJoinImageFragments--) | يشير إلى ما إذا كانت المكتبة ستحاول دمج أجزاء الصورة. |
| [hashCode()](#hashCode--) |  |
| [isDebug()](#isDebug--) | يحصل على العلامة التي تسمح بإخراج التحذيرات والرسائل أثناء التحويل. |
| [isSupressErrors()](#isSupressErrors--) | يعيد قيمة تشير إلى ما إذا كانت الأخطاء ستُقمع أثناء التحويل. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAdditionalFontsFolders(String[] fontsFolders)](#setAdditionalFontsFolders-java.lang.String---) | يحدد مجلدات الخطوط الإضافية التي يجب على المحول العثور على الخطوط فيها للمستند المدخل. |
| [setConvertFontsToTTF(boolean value)](#setConvertFontsToTTF-boolean-) | يحدد ما إذا كان سيتم حفظ الخطوط غير TrueType إلى TTF. |
| [setDebug(boolean debug)](#setDebug-boolean-) | يحدد العلامة التي تسمح بإخراج التحذيرات والرسائل أثناء التحويل. |
| [setImageFormat(ImageFormat imageFormat)](#setImageFormat-com.aspose.page.ImageFormat-) | يحدد تنسيق الصورة الناتجة. |
| [setJpegQualityLevel(int value)](#setJpegQualityLevel-int-) | يضبط القيمة التي تحدد مستوى الضغط للصورة. |
| [setResolution(float resolution)](#setResolution-float-) | يحدد دقة الصورة الناتجة. |
| [setSize(Dimension size)](#setSize-java.awt.Dimension-) | يحدد حجم الصفحة أو الصورة. |
| [setSmoothingMode(SmoothingMode smoothingMode)](#setSmoothingMode-com.aspose.eps.device.SmoothingMode-) | يضبط وضع التنعيم. |
| [setSupressErrors(boolean supressErrors)](#setSupressErrors-boolean-) | يحدد العلم الذي يشير إلى ما إذا كان سيتم قمع الأخطاء أثناء التحويل. |
| [setTryJoinImageFragments(boolean tryJoinImageFragments)](#setTryJoinImageFragments-boolean-) | يحدد ما إذا كان يجب على المكتبة محاولة ربط شظايا الصورة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ImageSaveOptions() {#ImageSaveOptions--}
```
public ImageSaveOptions()
```


إنشاء نسخة جديدة من فئة  ImageSaveOptions  مع القيم الافتراضية للعلامات  suppressErrors  (true) و  debug  (false).

### ImageSaveOptions(ImageFormat imageFormat) {#ImageSaveOptions-com.aspose.page.ImageFormat-}
```
public ImageSaveOptions(ImageFormat imageFormat)
```


يُنشئ نسخة جديدة من  ImageSaveOptions  بالتنسيق المحدد للصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| imageFormat | [ImageFormat](../../com.aspose.page/imageformat) | تنسيق الصورة. |

### ImageSaveOptions(Dimension size) {#ImageSaveOptions-java.awt.Dimension-}
```
public ImageSaveOptions(Dimension size)
```


يُنشئ نسخة جديدة من  ImageSaveOptions  بالحجم المحدد للصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الحجم | java.awt.Dimension | حجم الصورة. |

### ImageSaveOptions(Dimension size, ImageFormat imageFormat) {#ImageSaveOptions-java.awt.Dimension-com.aspose.page.ImageFormat-}
```
public ImageSaveOptions(Dimension size, ImageFormat imageFormat)
```


يُنشئ نسخة جديدة من  ImageSaveOptions  بالحجم المحدد للصورة وتنسيق الصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الحجم | java.awt.Dimension | حجم الصورة. |
| imageFormat | [ImageFormat](../../com.aspose.page/imageformat) | تنسيق الصورة. |

### ImageSaveOptions(ImageFormat imageFormat, boolean supressErrors) {#ImageSaveOptions-com.aspose.page.ImageFormat-boolean-}
```
public ImageSaveOptions(ImageFormat imageFormat, boolean supressErrors)
```


يُنشئ نسخة جديدة من  ImageSaveOptions  بالتنسيق المحدد للصورة وعلامة suppressErrors.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| imageFormat | [ImageFormat](../../com.aspose.page/imageformat) | تنسيق الصورة. |
| supressErrors | boolean | إذا كان صحيحًا، سيستمر التحويل على الرغم من الأخطاء غير الحرجة. |

### ImageSaveOptions(Dimension size, boolean supressErrors) {#ImageSaveOptions-java.awt.Dimension-boolean-}
```
public ImageSaveOptions(Dimension size, boolean supressErrors)
```


يُنشئ نسخة جديدة من  ImageSaveOptions  بالحجم المحدد للصورة وعلامة suppressErrors.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الحجم | java.awt.Dimension | حجم الصورة. |
| supressErrors | boolean | إذا كان صحيحًا، سيستمر التحويل على الرغم من الأخطاء غير الحرجة. |

### ImageSaveOptions(Dimension size, ImageFormat imageFormat, boolean supressErrors) {#ImageSaveOptions-java.awt.Dimension-com.aspose.page.ImageFormat-boolean-}
```
public ImageSaveOptions(Dimension size, ImageFormat imageFormat, boolean supressErrors)
```


يُنشئ نسخة جديدة من  ImageSaveOptions  بالحجم المحدد للصورة، وتنسيق الصورة، وعلامة suppressErrors.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الحجم | java.awt.Dimension | حجم الصورة. |
| imageFormat | [ImageFormat](../../com.aspose.page/imageformat) | تنسيق الصورة. |
| supressErrors | boolean | إذا كان صحيحًا، سيستمر التحويل على الرغم من الأخطاء غير الحرجة. |

### ImageSaveOptions(boolean supressErrors) {#ImageSaveOptions-boolean-}
```
public ImageSaveOptions(boolean supressErrors)
```


إنشاء نسخة جديدة من فئة  ImageSaveOptions  مع القيم الافتراضية للعلامة  debug  (false).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| supressErrors | boolean | إذا كان صحيحًا، سيستمر التحويل على الرغم من الأخطاء غير الحرجة. |

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
### getImageFormat() {#getImageFormat--}
```
public ImageFormat getImageFormat()
```


يحصل على تنسيق الصورة الناتجة.

**Returns:**
[ImageFormat](../../com.aspose.page/imageformat) - An output image format.
### getJpegQualityLevel() {#getJpegQualityLevel--}
```
public int getJpegQualityLevel()
```


يعيد القيمة التي تحدد مستوى الضغط للصورة. القيم المتاحة من 0 إلى 100. كلما كان الرقم المحدد أقل، زاد الضغط وبالتالي انخفضت جودة الصورة. القيمة 0 تؤدي إلى أدنى جودة للصورة، بينما القيمة 100 تؤدي إلى أعلى جودة.

**Returns:**
int - القيمة التي تحدد مستوى الضغط للصورة.
### getResolution() {#getResolution--}
```
public float getResolution()
```


يعيد دقة الصورة الناتجة.

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
[SmoothingMode](../../com.aspose.eps.device/smoothingmode) - the smoothingMode.
### getTryJoinImageFragments() {#getTryJoinImageFragments--}
```
public boolean getTryJoinImageFragments()
```


يشير إلى ما إذا كانت المكتبة ستحاول ربط شظايا الصورة. يُستخدم ذلك عندما يتم تقطيع الصورة في ملف PS/EPS المصدر إلى شظايا. في هذه الحالة، بدون هذه العلامة تُترك فجوات رقيقة بين الشظايا.

**Returns:**
boolean - قيمة العلامة.
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

### setImageFormat(ImageFormat imageFormat) {#setImageFormat-com.aspose.page.ImageFormat-}
```
public void setImageFormat(ImageFormat imageFormat)
```


يحدد تنسيق الصورة الناتجة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| imageFormat | [ImageFormat](../../com.aspose.page/imageformat) | تنسيق صورة إخراج. |

### setJpegQualityLevel(int value) {#setJpegQualityLevel-int-}
```
public void setJpegQualityLevel(int value)
```


يضبط القيمة التي تحدد مستوى الضغط للصورة. القيم المتاحة من 0 إلى 100. كلما كان الرقم المحدد أقل، زاد الضغط وبالتالي انخفضت جودة الصورة. القيمة 0 تؤدي إلى أدنى جودة للصورة، بينما القيمة 100 تؤدي إلى أعلى جودة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | القيمة التي تحدد مستوى الضغط للصورة. |

### setResolution(float resolution) {#setResolution-float-}
```
public void setResolution(float resolution)
```


يحدد دقة الصورة الناتجة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الدقة | float | دقة الصورة. |

### setSize(Dimension size) {#setSize-java.awt.Dimension-}
```
public void setSize(Dimension size)
```


يحدد حجم الصفحة أو الصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الحجم | java.awt.Dimension | حجم الصفحة أو الصورة. |

### setSmoothingMode(SmoothingMode smoothingMode) {#setSmoothingMode-com.aspose.eps.device.SmoothingMode-}
```
public void setSmoothingMode(SmoothingMode smoothingMode)
```


يضبط وضع التنعيم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| smoothingMode | [SmoothingMode](../../com.aspose.eps.device/smoothingmode) | وضع smoothingMode لتعيينه |

### setSupressErrors(boolean supressErrors) {#setSupressErrors-boolean-}
```
public void setSupressErrors(boolean supressErrors)
```


يحدد العلم الذي يشير إلى ما إذا كان سيتم قمع الأخطاء أثناء التحويل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| supressErrors | boolean | قيمة منطقية. |

### setTryJoinImageFragments(boolean tryJoinImageFragments) {#setTryJoinImageFragments-boolean-}
```
public void setTryJoinImageFragments(boolean tryJoinImageFragments)
```


يحدد ما إذا كانت المكتبة ستحاول ربط شظايا الصورة. يُستخدم ذلك عندما يتم تقطيع الصورة في ملف PS/EPS المصدر إلى شظايا. في هذه الحالة، بدون هذه العلامة تُترك فجوات رقيقة بين الشظايا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| tryJoinImageFragments | boolean | قيمة العلامة. |

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

