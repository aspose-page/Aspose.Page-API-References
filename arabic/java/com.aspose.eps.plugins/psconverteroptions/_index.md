---
title: "PsConverterOptions"
second_title: "مرجع Aspose.Page لـ Java API"
description: "يمثل الفئة الأساسية للخيارات الخاصة بالمكوّن الإضافي."
type: docs
weight: 11
url: /ar/java/com.aspose.eps.plugins/psconverteroptions/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.page.plugins.IPluginOptions](../../com.aspose.page.plugins/ipluginoptions), [com.aspose.page.plugins.IDataContainer](../../com.aspose.page.plugins/idatacontainer), [com.aspose.page.plugins.ISaveInstruction](../../com.aspose.page.plugins/isaveinstruction)
```
public class PsConverterOptions implements IPluginOptions, IDataContainer, ISaveInstruction
```

يمثل الفئة الأساسية للخيارات للملحق [PsConverter](../../com.aspose.eps.plugins/psconverter).
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addDataSource(IDataSource dataSource)](#addDataSource-com.aspose.page.plugins.IDataSource-) | يضيف مصدر بيانات جديد إلى مجموعة بيانات ملحق PsConverter. |
| [addSaveDataSource(IDataSource saveDataSource)](#addSaveDataSource-com.aspose.page.plugins.IDataSource-) | يضيف مصدر بيانات جديد إلى مجموعة بيانات ملحق PsConverterOptions. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAdditionalFontsFolders()](#getAdditionalFontsFolders--) | يعيد مجلدات الخطوط الإضافية التي يجب على المحول العثور على الخطوط فيها للمستند المدخل. |
| [getClass()](#getClass--) |  |
| [getDataCollection()](#getDataCollection--) | يعيد مجموعة بيانات ملحق PsConverterOptions. |
| [getExceptions()](#getExceptions--) | يعيد قائمة بالأخطاء غير الحرجة. |
| [getJpegQualityLevel()](#getJpegQualityLevel--) | يعيد القيمة التي تحدد مستوى الضغط لصورة. |
| [getOperationName()](#getOperationName--) | يعيد اسم العملية. |
| [getSaveTargetsCollection()](#getSaveTargetsCollection--) | يحصل على مجموعة الأهداف المضافة لحفظ نتائج العملية. |
| [hashCode()](#hashCode--) |  |
| [isDebug()](#isDebug--) | يحصل على العلامة التي تسمح بإخراج التحذيرات والرسائل أثناء التحويل. |
| [isSupressErrors()](#isSupressErrors--) | يعيد قيمة تشير إلى ما إذا كانت الأخطاء ستُقمع أثناء التحويل. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAdditionalFontsFolders(String[] fontsFolders)](#setAdditionalFontsFolders-java.lang.String---) | يحدد مجلدات الخطوط الإضافية التي يجب على المحول العثور على الخطوط فيها للمستند المدخل. |
| [setDebug(boolean debug)](#setDebug-boolean-) | يحدد العلامة التي تسمح بإخراج التحذيرات والرسائل أثناء التحويل. |
| [setJpegQualityLevel(int value)](#setJpegQualityLevel-int-) | يضبط القيمة التي تحدد مستوى الضغط للصورة. |
| [setSupressErrors(boolean supressErrors)](#setSupressErrors-boolean-) | يحدد العلم الذي يشير إلى ما إذا كان سيتم قمع الأخطاء أثناء التحويل. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addDataSource(IDataSource dataSource) {#addDataSource-com.aspose.page.plugins.IDataSource-}
```
public final void addDataSource(IDataSource dataSource)
```


يضيف مصدر بيانات جديد إلى مجموعة بيانات ملحق PsConverter.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| dataSource | [IDataSource](../../com.aspose.page.plugins/idatasource) | مصدر البيانات للإضافة. |

### addSaveDataSource(IDataSource saveDataSource) {#addSaveDataSource-com.aspose.page.plugins.IDataSource-}
```
public final void addSaveDataSource(IDataSource saveDataSource)
```


يضيف مصدر بيانات جديد إلى مجموعة بيانات ملحق PsConverterOptions.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| saveDataSource | [IDataSource](../../com.aspose.page.plugins/idatasource) | مصدر البيانات (ملف أو تدفق) لحفظ نتائج العملية. |

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
### getDataCollection() {#getDataCollection--}
```
public final List<IDataSource> getDataCollection()
```


يعيد مجموعة بيانات ملحق PsConverterOptions.

**Returns:**
java.util.List<com.aspose.page.plugins.IDataSource>
### getExceptions() {#getExceptions--}
```
public List<Exception> getExceptions()
```


يعيد قائمة بالأخطاء غير الحرجة.

**Returns:**
java.util.List<java.lang.Exception> - قائمة الاستثناءات
### getJpegQualityLevel() {#getJpegQualityLevel--}
```
public int getJpegQualityLevel()
```


يعيد القيمة التي تحدد مستوى الضغط للصورة. القيم المتاحة من 0 إلى 100. كلما كان الرقم المحدد أقل، زاد الضغط وبالتالي انخفضت جودة الصورة. القيمة 0 تؤدي إلى أدنى جودة للصورة، بينما القيمة 100 تؤدي إلى أعلى جودة.

**Returns:**
int - القيمة التي تحدد مستوى الضغط للصورة.
### getOperationName() {#getOperationName--}
```
public String getOperationName()
```


يعيد اسم العملية.

**Returns:**
java.lang.String
### getSaveTargetsCollection() {#getSaveTargetsCollection--}
```
public final List<IDataSource> getSaveTargetsCollection()
```


يحصل على مجموعة الأهداف المضافة لحفظ نتائج العملية.

**Returns:**
java.util.List<com.aspose.page.plugins.IDataSource>
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

### setDebug(boolean debug) {#setDebug-boolean-}
```
public void setDebug(boolean debug)
```


يحدد العلامة التي تسمح بإخراج التحذيرات والرسائل أثناء التحويل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| debug | boolean | قيمة منطقية. |

### setJpegQualityLevel(int value) {#setJpegQualityLevel-int-}
```
public void setJpegQualityLevel(int value)
```


يضبط القيمة التي تحدد مستوى الضغط للصورة. القيم المتاحة من 0 إلى 100. كلما كان الرقم المحدد أقل، زاد الضغط وبالتالي انخفضت جودة الصورة. القيمة 0 تؤدي إلى أدنى جودة للصورة، بينما القيمة 100 تؤدي إلى أعلى جودة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | القيمة التي تحدد مستوى الضغط للصورة. |

### setSupressErrors(boolean supressErrors) {#setSupressErrors-boolean-}
```
public void setSupressErrors(boolean supressErrors)
```


يحدد العلم الذي يشير إلى ما إذا كان سيتم قمع الأخطاء أثناء التحويل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| supressErrors | boolean | قيمة منطقية. |

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

