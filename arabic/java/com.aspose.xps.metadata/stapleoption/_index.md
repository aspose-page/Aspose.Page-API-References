---
title: "Staple.StapleOption"
second_title: "مرجع Aspose.Page لـ Java API"
description: "يصف خيارات ميزات JobStapleAllDocuments و DocumentStaple."
type: docs
weight: 10
url: /ar/java/com.aspose.xps.metadata/staple.stapleoption/
---
**Inheritance:**
java.lang.Object, [com.aspose.xps.metadata.PrintTicketElement](../../com.aspose.xps.metadata/printticketelement), [com.aspose.xps.metadata.CompositePrintTicketElement](../../com.aspose.xps.metadata/compositeprintticketelement), [com.aspose.xps.metadata.Option](../../com.aspose.xps.metadata/option)
```
public static final class Staple.StapleOption extends Option
```

يصف خيارات ميزات  JobStapleAllDocuments  و  DocumentStaple .
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [StapleOption(String optionName, Staple.IStapleOptionItem[] items)](#StapleOption-java.lang.String-com.aspose.xps.metadata.Staple.IStapleOptionItem...-) | ينشئ نسخة جديدة. |
## الحقول

| حقل | الوصف |
| --- | --- |
| [None](#None) | يحدد عدم وجود تثبيت. |
| [SaddleStitch](#SaddleStitch) | يحدد تثبيت بخياطة السرج. |
| [StapleBottomLeft](#StapleBottomLeft) | يحدد دبوسًا واحدًا في الزاوية السفلية اليسرى. |
| [StapleBottomRight](#StapleBottomRight) | يحدد دبوسًا واحدًا في الزاوية السفلية اليمنى. |
| [StapleDualBottom](#StapleDualBottom) | يحدد دبوسين على طول الحافة السفلية. |
| [StapleDualLeft](#StapleDualLeft) | يحدد دبوسين على طول الحافة اليسرى. |
| [StapleDualRight](#StapleDualRight) | يحدد دبوسين على طول الحافة اليمنى. |
| [StapleDualTop](#StapleDualTop) | يحدد دبوسين على طول الحافة العلوية |
| [StapleTopLeft](#StapleTopLeft) | يحدد دبوسًا واحدًا في الزاوية العلوية اليسرى. |
| [StapleTopRight](#StapleTopRight) | يحدد دبوسًا واحدًا في الزاوية العلوية اليمنى. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(IOptionItem[] items)](#add-com.aspose.xps.metadata.IOptionItem...-) | يضيف قائمة من العناصر إلى نهاية قائمة العناصر لهذا الخيار. |
| [add(Staple.IStapleOptionItem[] items)](#add-com.aspose.xps.metadata.Staple.IStapleOptionItem...-) | يضيف مصفوفة من  IStapleOptionItem  إلى الميزة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | يحصل على اسم العنصر. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAngle(int angle)](#setAngle-int-) | يضبط قيمة خاصية  Angle  المُقيمة. |
| [setSheetCapacity(int sheetCapacity)](#setSheetCapacity-int-) | يضبط قيمة خاصية  SheetCapacity  المُقيمة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### StapleOption(String optionName, Staple.IStapleOptionItem[] items) {#StapleOption-java.lang.String-com.aspose.xps.metadata.Staple.IStapleOptionItem...-}
```
public StapleOption(String optionName, Staple.IStapleOptionItem[] items)
```


ينشئ نسخة جديدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| optionName | java.lang.String | اسم خيار. |
| items | [IStapleOptionItem\[\]](../../com.aspose.xps.metadata/istapleoptionitem) | مصفوفة عشوائية من  IStapleOptionItem  كائنات. |

### None {#None}
```
public static final Staple.StapleOption None
```


يحدد عدم وجود تثبيت.

### SaddleStitch {#SaddleStitch}
```
public static final Staple.StapleOption SaddleStitch
```


يحدد تثبيت بخياطة السرج.

### StapleBottomLeft {#StapleBottomLeft}
```
public static final Staple.StapleOption StapleBottomLeft
```


يحدد دبوسًا واحدًا في الزاوية السفلية اليسرى.

### StapleBottomRight {#StapleBottomRight}
```
public static final Staple.StapleOption StapleBottomRight
```


يحدد دبوسًا واحدًا في الزاوية السفلية اليمنى.

### StapleDualBottom {#StapleDualBottom}
```
public static final Staple.StapleOption StapleDualBottom
```


يحدد دبوسين على طول الحافة السفلية.

### StapleDualLeft {#StapleDualLeft}
```
public static final Staple.StapleOption StapleDualLeft
```


يحدد دبوسين على طول الحافة اليسرى.

### StapleDualRight {#StapleDualRight}
```
public static final Staple.StapleOption StapleDualRight
```


يحدد دبوسين على طول الحافة اليمنى.

### StapleDualTop {#StapleDualTop}
```
public static final Staple.StapleOption StapleDualTop
```


يحدد دبوسين على طول الحافة العلوية

### StapleTopLeft {#StapleTopLeft}
```
public static final Staple.StapleOption StapleTopLeft
```


يحدد دبوسًا واحدًا في الزاوية العلوية اليسرى.

### StapleTopRight {#StapleTopRight}
```
public static final Staple.StapleOption StapleTopRight
```


يحدد دبوسًا واحدًا في الزاوية العلوية اليمنى.

### add(IOptionItem[] items) {#add-com.aspose.xps.metadata.IOptionItem...-}
```
public void add(IOptionItem[] items)
```


يضيف قائمة من العناصر إلى نهاية قائمة العناصر لهذا الخيار. يجب أن يكون كل عنصر إما  ScoredProperty  أو  Property  مثيل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| items | [IOptionItem\[\]](../../com.aspose.xps.metadata/ioptionitem) | قائمة العناصر للإضافة. |

### add(Staple.IStapleOptionItem[] items) {#add-com.aspose.xps.metadata.Staple.IStapleOptionItem...-}
```
public Staple.StapleOption add(Staple.IStapleOptionItem[] items)
```


يضيف مصفوفة من  IStapleOptionItem  إلى الميزة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| items | [IStapleOptionItem\[\]](../../com.aspose.xps.metadata/istapleoptionitem) | مصفوفة عشوائية من  IStapleOptionItem  كائنات. |

**Returns:**
[StapleOption](../../com.aspose.xps.metadata/stapleoption) - This options instance.
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




### setAngle(int angle) {#setAngle-int-}
```
public final Staple.StapleOption setAngle(int angle)
```


يضبط قيمة خاصية  Angle  المُقيمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| angle | int | قيمة خاصية  Angle  المُقيمة. |

**Returns:**
[StapleOption](../../com.aspose.xps.metadata/stapleoption) - This option instance.
### setSheetCapacity(int sheetCapacity) {#setSheetCapacity-int-}
```
public final Staple.StapleOption setSheetCapacity(int sheetCapacity)
```


يضبط قيمة خاصية  SheetCapacity  المُقيمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetCapacity | int | قيمة خاصية  SheetCapacity  المُقيمة. |

**Returns:**
[StapleOption](../../com.aspose.xps.metadata/stapleoption) - This option instance.
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

