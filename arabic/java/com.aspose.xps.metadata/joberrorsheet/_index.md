---
title: "JobErrorSheet"
second_title: "مرجع Aspose.Page لـ Java API"
description: "يصف إخراج ورقة الخطأ."
type: docs
weight: 53
url: /ar/java/com.aspose.xps.metadata/joberrorsheet/
---
**Inheritance:**
java.lang.Object, [com.aspose.xps.metadata.PrintTicketElement](../../com.aspose.xps.metadata/printticketelement), [com.aspose.xps.metadata.CompositePrintTicketElement](../../com.aspose.xps.metadata/compositeprintticketelement), [com.aspose.xps.metadata.Feature](../../com.aspose.xps.metadata/feature)

**All Implemented Interfaces:**
[com.aspose.xps.metadata.IJobPrintTicketItem](../../com.aspose.xps.metadata/ijobprintticketitem)
```
public final class JobErrorSheet extends Feature implements IJobPrintTicketItem
```

يصف إخراج ورقة الخطأ. سيتضمن العمل بالكامل ورقة خطأ واحدة. يجب إخراج ورقة الخطأ على حجم الصفحة الافتراضي PageMediaSize وباستخدام نوع الصفحة الافتراضي PageMediaType. يجب عزل ورقة الخطأ عن باقي العمل. وهذا يعني أن أي خيارات تشطيب أو معالجة (مثل JobDuplex أو JobStaple أو JobBinding) لا يجب أن تشمل ورقة الخطأ. يجب أن تكون ورقة الخطأ هي الورقة النهائية في العمل. https://docs.microsoft.com/en-us/windows/win32/printdocs/joberrorsheet
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [JobErrorSheet(JobErrorSheet.IJobErrorSheetItem[] items)](#JobErrorSheet-com.aspose.xps.metadata.JobErrorSheet.IJobErrorSheetItem...-) | ينشئ نسخة جديدة. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(IFeatureItem[] items)](#add-com.aspose.xps.metadata.IFeatureItem...-) | يضيف قائمة من العناصر إلى نهاية قائمة العناصر لهذه الميزة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | يحصل على اسم العنصر. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### JobErrorSheet(JobErrorSheet.IJobErrorSheetItem[] items) {#JobErrorSheet-com.aspose.xps.metadata.JobErrorSheet.IJobErrorSheetItem...-}
```
public JobErrorSheet(JobErrorSheet.IJobErrorSheetItem[] items)
```


ينشئ نسخة جديدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| items | [IJobErrorSheetItem\[\]](../../com.aspose.xps.metadata/ijoberrorsheetitem) | مصفوفة من العناصر الخاصة بالميزة. |

### add(IFeatureItem[] items) {#add-com.aspose.xps.metadata.IFeatureItem...-}
```
public void add(IFeatureItem[] items)
```


يضيف قائمة من العناصر إلى نهاية قائمة عناصر هذه الميزة. يجب أن يكون كل عنصر إما Feature أو Option أو Property.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| items | [IFeatureItem\[\]](../../com.aspose.xps.metadata/ifeatureitem) | قائمة العناصر للإضافة. |

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

