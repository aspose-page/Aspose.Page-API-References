---
title: "رخصة"
second_title: "مرجع Aspose.Page لـ Java API"
description: "يوفر طرقًا لترخيص المكوّن."
type: docs
weight: 14
url: /ar/java/com.aspose.page/license/
---
**Inheritance:**
java.lang.Object
```
public class License
```

يوفر طرقًا لترخيص المكوّن.

في هذا المثال، سيتم محاولة العثور على ملف ترخيص اسمه MyLicense.lic في المجلد الذي يحتوي على المكوّن، في المجلد الذي يحتوي على التجميع المستدعي، في مجلد تجميع الدخول ثم في الموارد المدمجة للتجميع المستدعي.

License license = new License();
license.setLicense("MyLicense.lic");
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [License()](#License--) | ينشئ نسخة جديدة من هذه الفئة. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [isInternalFIPSSecurity()](#isInternalFIPSSecurity--) | بشكل افتراضي نستخدم أمان jdk الافتراضي. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setInternalFIPSSecurity(boolean internalFIPSSecurity)](#setInternalFIPSSecurity-boolean-) | بشكل افتراضي نستخدم أمان jre الافتراضي. |
| [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | يرخص المكوّن. |
| [setLicense(String licenseName)](#setLicense-java.lang.String-) | يرخص المكوّن. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### License() {#License--}
```
public License()
```


ينشئ نسخة جديدة من هذه الفئة.

في هذا المثال، سيتم محاولة العثور على ملف ترخيص اسمه MyLicense.lic في المجلد الذي يحتوي على المكوّن، في المجلد الذي يحتوي على التجميع المستدعي، في مجلد تجميع الدخول ثم في الموارد المدمجة للتجميع المستدعي.

License license = new License();
license.setLicense("MyLicense.lic");

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
### isInternalFIPSSecurity() {#isInternalFIPSSecurity--}
```
public static boolean isInternalFIPSSecurity()
```


بشكل افتراضي نستخدم أمان jdk الافتراضي. القيمة الافتراضية == false. في بعض الحالات لا يمكن لبيئة جافا المخصصة دعم الخوارزميات المطلوبة، لذلك يمكننا اقتراح استخدام أمان FIPS المدمج الداخلي.

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




### setInternalFIPSSecurity(boolean internalFIPSSecurity) {#setInternalFIPSSecurity-boolean-}
```
public static void setInternalFIPSSecurity(boolean internalFIPSSecurity)
```


بشكل افتراضي نستخدم أمان jre الافتراضي. القيمة الافتراضية == false. في بعض الحالات لا يمكن لبيئة جافا المخصصة دعم الخوارزميات المطلوبة، لذلك يمكننا اقتراح استخدام أمان FIPS المدمج الداخلي.

لاحظ أيضًا: وفقًا لخوارزمية JVM SecureRandom على بعض أنظمة التشغيل ينتظر /dev/random كمية معينة من \\u201cnoise\\u201d لتُولد على الجهاز المضيف قبل إرجاع النتيجة. المكتبة المستخدمة لتوليد الأرقام العشوائية في JVM الخاصة بـ Oracle’s تعتمد على /dev/random بشكل افتراضي لمنصات UNIX. على الرغم من أن /dev/random أكثر أمانًا، يُنصح باستخدام /dev/urandom إذا كان تكوين JVM الافتراضي يسبب تأخيرات، أو إضافة أجهزة تولد العشوائية لـ /dev/random.

يمكن لخيار جافا التالي المساعدة في تجنب التأخيرات وتجاوز إعداد securerandom.source. -Djava.security.egd=file:/dev/./urandom

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| internalFIPSSecurity | boolean | قيمة منطقية |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public void setLicense(InputStream stream)
```


يرخص المكوّن.

دفق يحتوي على الترخيص.

استخدم هذه الطريقة لتحميل ترخيص من دفق.

License license = new License();
license.setLicense(myStream);

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| دفق | java.io.InputStream | دفق الترخيص |

### setLicense(String licenseName) {#setLicense-java.lang.String-}
```
public void setLicense(String licenseName)
```


يرخص المكوّن.

يحاول العثور على الترخيص في المواقع التالية:

1. مسار صريح.

2. مجلد ملف jar الخاص بالمكوّن.

في هذا المثال، سيتم محاولة العثور على ملف ترخيص اسمه MyLicense.lic في المجلد الذي يحتوي على المكوّن، في المجلد الذي يحتوي على التجميع المستدعي، في مجلد تجميع الدخول ثم في الموارد المدمجة للتجميع المستدعي.

License license = new License();
license.setLicense("MyLicense.lic");

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| licenseName | java.lang.String | يمكن أن يكون اسم ملف كامل أو قصير أو اسم مورد مدمج. استخدم سلسلة فارغة للتبديل إلى وضع التقييم. |

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

