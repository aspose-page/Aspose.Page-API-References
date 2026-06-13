---
title: "PrintTicket"
second_title: "مرجع Aspose.Page لـ Java API"
description: "الفئة التي تنفذ PrintTicket شائع لأي نطاق."
type: docs
weight: 141
url: /ar/java/com.aspose.xps.metadata/printticket/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class PrintTicket implements Iterable<String>
```

الفئة التي تنفّذ PrintTicket شائع لأي نطاق. الفئة الأساسية لتذاكر الطباعة على مستوى الوظيفة، المستند، والصفحة. عنصر PrintTicket هو العنصر الجذر لمستند PrintTicket. عنصر PrintTicket يحتوي على جميع معلومات تنسيق الوظيفة المطلوبة لإخراج وظيفة. https://docs.microsoft.com/en-us/windows/win32/printdocs/printticket
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [PrintTicket(IPrintTicketItem[] items)](#PrintTicket-com.aspose.xps.metadata.IPrintTicketItem...-) | ينشئ نسخة جديدة. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | يعيد مكرّر أسماء عناصر تذكرة الطباعة. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String[] names)](#remove-java.lang.String...-) | يزيل عنصرًا من قائمة عناصر تذكرة الطباعة هذه. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PrintTicket(IPrintTicketItem[] items) {#PrintTicket-com.aspose.xps.metadata.IPrintTicketItem...-}
```
public PrintTicket(IPrintTicketItem[] items)
```


ينشئ نسخة جديدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| items | [IPrintTicketItem\[\]](../../com.aspose.xps.metadata/iprintticketitem) | مصفوفة عشوائية من مثيلات IPrintTicketItem. يجب أن يكون كل منها إما Feature أو ParameterInit أو Property. |

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
### iterator() {#iterator--}
```
public Iterator<String> iterator()
```


يعيد مكرّر أسماء عناصر تذكرة الطباعة.

**Returns:**
java.util.Iterator<java.lang.String> - يعيد مكرّر للقائمة.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(String[] names) {#remove-java.lang.String...-}
```
public void remove(String[] names)
```


يزيل عنصرًا من قائمة عناصر تذكرة الطباعة هذه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الأسماء | java.lang.String[] | مصفوفة من أسماء العناصر. |

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

