---
title: "XpsConverter"
second_title: "مرجع Aspose.Page لـ Java API"
description: "يمثل إضافة XpsConverter."
type: docs
weight: 10
url: /ar/java/com.aspose.xps.plugins/xpsconverter/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.page.plugins.IPlugin](../../com.aspose.page.plugins/iplugin)
```
public class XpsConverter implements IPlugin
```

يمثل إضافة XpsConverter.

يوضح المثال كيفية تحويل مستند XPS إلى مستند PDF.

// إنشاء XpsConverter XpsConverter converter = new XpsConverter(); // إنشاء كائن XpsConverterToPdfOptions لتعيين نوع بيانات الإخراج كملف XpsConverterToPdfOptions opt = new XpsConverterToPdfOptions(); // إضافة مسار ملف الإدخال opt.addDataSource(new FileDataSource(inputPath)); // تعيين مسار ملف الإخراج opt.addSaveDataSource(new FileDataSource(outputPath)); // بدء عملية التحويل ResultContainer results = converter.process(opt);

يوضح المثال كيفية تحويل مستند XPS إلى صورة مع إخراج ملف.

// إنشاء XpsConverter XpsConverter converter = new XpsConverter(); // إنشاء XpsConverterToImageOptions مع تنسيق صورة هدف JPEG. تنسيق الصورة الافتراضي للصورة الناتجة هو PNG. // يمكننا أيضًا تعيين حجم الصورة الناتجة، ودقة، ووضع التنعيم ومستوى جودة JPEG لتنسيق صورة JPEG الناتجة. XpsConverterToImageOptions opt = new XpsConverterToImageOptions(ImageFormat.Jpeg); // إضافة مسار ملف الإدخال opt.addDataSource(new FileDataSource(inputPath)); // إذا كان ملف XPS الإدخال متعدد الصفحات، فإن النتائج ستكون مجموعة من ملفات الصور بالاسم: [\"outputPath\" بدون امتداد][رقم الصفحة يبدأ من 0].[الامتداد من \"outputPath\"] opt.addSaveDataSource(new FileDataSource(outputPath)); // بدء عملية التحويل converter.process(opt);

يوضح المثال كيفية تحويل مستند XPS إلى صورة مع إخراج مصفوفات بايت.

في مصدر بيانات إخراج مصفوفات البايت (byte[][]) تحتوي كل مصفوفة بايت على صورة صفحة واحدة. وبالتالي، بالنسبة للمستندات ذات صفحة واحدة سيكون الناتج يحتوي على مصفوفة [1][], أما المستندات متعددة الصفحات فسيكون الناتج يحتوي على مصفوفة عدد الصفحات في مستند XPS الإدخال []. // إنشاء XpsConverter XpsConverter converter = new XpsConverter(); // إنشاء XpsConverterToImageOptions مع تنسيق صورة هدف JPEG. تنسيق الصورة الافتراضي للصورة الناتجة هو PNG. // يمكننا أيضًا تعيين حجم الصورة الناتجة، ودقة، ووضع التنعيم ومستوى جودة JPEG لتنسيق صورة JPEG الناتجة. XpsConverterToImageOptions opt = new XpsConverterToImageOptions(ImageFormat.Jpeg); // إضافة مسار ملف الإدخال opt.addDataSource(new FileDataSource(inputPath)); // إذا كان ملف XPS الإدخال متعدد الصفحات، فإن النتائج ستكون مجموعة من ملفات الصور بالاسم: [\"outputPath\" بدون امتداد][رقم الصفحة يبدأ من 1].[الامتداد من \"outputPath\"] opt.addSaveDataSource(new ByteArrayDataSource()); // بدء عملية التحويل converter.process(opt); // الحصول على مصفوفات البايت الناتجة byte[][] imagesBytes = (byte [][]) ((ByteArrayResult)results.ResultCollection[0]).Data;
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [XpsConverter()](#XpsConverter--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [dispose()](#dispose--) | تنفيذ IDisposable. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(IPluginOptions options)](#process-com.aspose.page.plugins.IPluginOptions-) | يبدأ معالجة XpsConverter بالمعلمات المحددة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### XpsConverter() {#XpsConverter--}
```
public XpsConverter()
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


يبدأ معالجة XpsConverter بالمعلمات المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| options | [IPluginOptions](../../com.aspose.page.plugins/ipluginoptions) | كائن خيارات يحتوي على تعليمات لمحول XpsConverter. |

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

