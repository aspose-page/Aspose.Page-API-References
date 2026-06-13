---
title: "PsConverter"
second_title: "مرجع Aspose.Page لـ Java API"
description: "يمثل ملحق PsConverter."
type: docs
weight: 10
url: /ar/java/com.aspose.eps.plugins/psconverter/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.page.plugins.IPlugin](../../com.aspose.page.plugins/iplugin)
```
public class PsConverter implements IPlugin
```

يمثل ملحق PsConverter.

يوضح المثال كيفية تحويل ملف PS/EPS إلى مستند PDF.

// إنشاء PsConverter PsConverter converter = new PsConverter(); // إنشاء كائن PsConverterToPdfOptions لتعيين نوع البيانات الناتجة كملف PsConverterToPdfOptions opt = new PsConverterToPdfOptions(); // إضافة مسار ملف الإدخال opt.addDataSource(new FileDataSource(inputPath)); // تعيين مسار ملف الإخراج opt.addSaveDataSource(new FileDataSource(outputPath)); // بدء عملية التحويل ResultContainer results = converter.process(opt);

يوضح المثال كيفية تحويل ملف PS/EPS إلى صورة مع إخراج إلى ملف.

// إنشاء PsConverter PsConverter converter = new PsConverter(); // إنشاء PsConverterToImageOptions مع تنسيق صورة هدف JPEG. تنسيق الصورة الافتراضي للصورة الناتجة هو PNG. // يمكننا أيضًا تعيين حجم الصورة الناتجة، ودقة، ووضع التنعيم ومستوى جودة JPEG لتنسيق الصورة الناتجة JPEG. PsConverterToImageOptions opt = new PsConverterToImageOptions(ImageFormat.Jpeg); // إضافة مسار ملف الإدخال opt.addDataSource(new FileDataSource(inputPath)); // إذا كان ملف PS الإدخال متعدد الصفحات، ستكون النتائج مجموعة من ملفات الصورة بالأسماء: [\"outputPath\" بدون امتداد][رقم الصفحة يبدأ من 0].[الامتداد من \"outputPath\"] opt.addSaveDataSource(new FileDataSource(outputPath)); // بدء عملية التحويل converter.process(opt);

يوضح المثال كيفية تحويل ملف PS/EPS إلى صورة مع إخراج على شكل مصفوفات بايت.

في مصدر بيانات إخراج مصفوفات البايت (byte [][] ) تحتوي مصفوفة بايت واحدة على صورة صفحة واحدة. وبالتالي، بالنسبة للمستندات ذات الصفحة الواحدة سيكون الناتج يحتوي على مصفوفة [1][], أما المستندات متعددة الصفحات فسيكون الناتج يحتوي على مصفوفة [عدد الصفحات في مستند PS الإدخال][]. // إنشاء PsConverter PsConverter converter = new PsConverter(); // إنشاء PsConverterToImageOptions مع تنسيق صورة هدف JPEG. تنسيق الصورة الافتراضي للصورة الناتجة هو PNG. // يمكننا أيضًا تعيين حجم الصورة الناتجة، ودقة، ووضع التنعيم ومستوى جودة JPEG لتنسيق الصورة الناتجة JPEG. PsConverterToImageOptions opt = new PsConverterToImageOptions(ImageFormat.Jpeg); // إضافة مسار ملف الإدخال opt.addDataSource(new FileDataSource(inputPath)); // إذا كان ملف PS الإدخال متعدد الصفحات، ستكون النتائج مجموعة من ملفات الصورة بالأسماء: [\"outputPath\" بدون امتداد][رقم الصفحة يبدأ من 0].[الامتداد من \"outputPath\"] opt.addSaveDataSource(new ByteArrayDataSource()); // بدء عملية التحويل converter.process(opt); // الحصول على مصفوفات البايت الناتجة byte[][] imagesBytes = (byte [][]) ((ByteArrayResult)results.ResultCollection[0]).Data;
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [PsConverter()](#PsConverter--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [dispose()](#dispose--) | تنفيذ IDisposable. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(IPluginOptions options)](#process-com.aspose.page.plugins.IPluginOptions-) | يبدأ معالجة PsConverter بالمعلمات المحددة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PsConverter() {#PsConverter--}
```
public PsConverter()
```


### dispose() {#dispose--}
```
public final void dispose()
```


تنفيذ IDisposable.

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




### process(IPluginOptions options) {#process-com.aspose.page.plugins.IPluginOptions-}
```
public final ResultContainer process(IPluginOptions options)
```


يبدأ معالجة PsConverter بالمعلمات المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| options | [IPluginOptions](../../com.aspose.page.plugins/ipluginoptions) | كائن خيارات يحتوي على تعليمات لـ PsConverter. |

**Returns:**
[ResultContainer](../../com.aspose.page.plugins/resultcontainer) - An ResultContainer object containing the result of the operation.
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

