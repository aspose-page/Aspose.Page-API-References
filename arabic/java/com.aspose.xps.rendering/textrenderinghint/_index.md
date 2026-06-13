---
title: "TextRenderingHint"
second_title: "مرجع Aspose.Page لـ Java API"
description: "يحدد جودة عرض النص."
type: docs
weight: 25
url: /ar/java/com.aspose.xps.rendering/textrenderinghint/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum TextRenderingHint extends Enum<TextRenderingHint>
```

يحدد جودة عرض النص.
## الحقول

| حقل | الوصف |
| --- | --- |
| [AntiAlias](#AntiAlias) | يتم رسم كل حرف باستخدام صورة glyph bitmap المضادة للتنعيم دون توجيه. |
| [AntiAliasGridFit](#AntiAliasGridFit) | يتم رسم كل حرف باستخدام صورة glyph bitmap المضادة للتنعيم مع التوجيه. |
| [ClearTypeGridFit](#ClearTypeGridFit) | يتم رسم كل حرف باستخدام صورة glyph ClearType bitmap مع التوجيه. |
| [SingleBitPerPixel](#SingleBitPerPixel) | يتم رسم كل حرف باستخدام صورة glyph bitmap. |
| [SingleBitPerPixelGridFit](#SingleBitPerPixelGridFit) | يتم رسم كل حرف باستخدام صورة glyph bitmap. |
| [SystemDefault](#SystemDefault) | يتم رسم كل حرف باستخدام صورة glyph bitmap، مع تلميح العرض الافتراضي للنظام. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [<T>valueOf(Class<T> arg0, String arg1)](#-T-valueOf-java.lang.Class-T--java.lang.String-) |  |
| [compareTo(E arg0)](#compareTo-E-) |  |
| [describeConstable()](#describeConstable--) |  |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDeclaringClass()](#getDeclaringClass--) |  |
| [hashCode()](#hashCode--) |  |
| [name()](#name--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [ordinal()](#ordinal--) |  |
| [toString()](#toString--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AntiAlias {#AntiAlias}
```
public static final TextRenderingHint AntiAlias
```


يتم رسم كل حرف باستخدام صورة glyph bitmap المضادة للتنعيم دون توجيه. جودة أفضل بفضل التنعيم. قد تكون فروق عرض الساق ملحوظة لأن التوجيه معطل.

### AntiAliasGridFit {#AntiAliasGridFit}
```
public static final TextRenderingHint AntiAliasGridFit
```


يتم رسم كل حرف باستخدام صورة glyph bitmap المضادة للتنعيم مع التوجيه. جودة أفضل بكثير بفضل التنعيم، لكن بتكلفة أداء أعلى.

### ClearTypeGridFit {#ClearTypeGridFit}
```
public static final TextRenderingHint ClearTypeGridFit
```


يتم رسم كل حرف باستخدام صورة glyph ClearType bitmap مع التوجيه. أعلى إعداد للجودة. يُستخدم للاستفادة من ميزات خط ClearType.

### SingleBitPerPixel {#SingleBitPerPixel}
```
public static final TextRenderingHint SingleBitPerPixel
```


يتم رسم كل حرف باستخدام صورة glyph bitmap. لا يتم استخدام التوجيه.

### SingleBitPerPixelGridFit {#SingleBitPerPixelGridFit}
```
public static final TextRenderingHint SingleBitPerPixelGridFit
```


يتم رسم كل حرف باستخدام صورة glyph bitmap. يُستخدم التوجيه لتحسين مظهر الحرف على الساقيات والانحناءات.

### SystemDefault {#SystemDefault}
```
public static final TextRenderingHint SystemDefault
```


يتم رسم كل حرف باستخدام صورة glyph bitmap، مع تلميح العرض الافتراضي للنظام. سيتم رسم النص باستخدام أي إعدادات تنعيم للخط اختارها المستخدم للنظام.

### <T>valueOf(Class<T> arg0, String arg1) {#-T-valueOf-java.lang.Class-T--java.lang.String-}
```
public static T <T>valueOf(Class<T> arg0, String arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.lang.Class<T> |  |
| arg1 | java.lang.String |  |

**Returns:**
T
### compareTo(E arg0) {#compareTo-E-}
```
public final int compareTo(E arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | E |  |

**Returns:**
int
### describeConstable() {#describeConstable--}
```
public final Optional<Enum.EnumDesc<E>> describeConstable()
```




**Returns:**
java.util.Optional<java.lang.Enum.EnumDesc<E>>
### equals(Object arg0) {#equals-java.lang.Object-}
```
public final boolean equals(Object arg0)
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
### getDeclaringClass() {#getDeclaringClass--}
```
public final Class<E> getDeclaringClass()
```




**Returns:**
java.lang.Class<E>
### hashCode() {#hashCode--}
```
public final int hashCode()
```




**Returns:**
int
### name() {#name--}
```
public final String name()
```




**Returns:**
java.lang.String
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### ordinal() {#ordinal--}
```
public final int ordinal()
```




**Returns:**
int
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static TextRenderingHint valueOf(String name)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الاسم | java.lang.String |  |

**Returns:**
[TextRenderingHint](../../com.aspose.xps.rendering/textrenderinghint)
### values() {#values--}
```
public static TextRenderingHint[] values()
```




**Returns:**
com.aspose.xps.rendering.TextRenderingHint[]
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

