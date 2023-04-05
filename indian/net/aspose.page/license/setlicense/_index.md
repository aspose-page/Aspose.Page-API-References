---
title: License.SetLicense
second_title: .NET API संदर्भ के लिए Aspose.Page
description: License तरक. घटक क लइसेंस देत है
type: docs
weight: 30
url: /hi/net/aspose.page/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

घटक को लाइसेंस देता है।

```csharp
public void SetLicense(string licenseName)
```

### टिप्पणियों

निम्न स्थानों में लाइसेंस ढूँढने का प्रयास करता है:

1. स्पष्ट पथ।

2. घटक असेंबली का फ़ोल्डर।

3. क्लाइंट की कॉलिंग असेंबली का फोल्डर।

4. एंट्री असेंबली का फोल्डर।

5. ग्राहक की कॉलिंग असेंबली में एक एम्बेडेड संसाधन।

**टिप्पणी:**.NET कॉम्पैक्ट फ्रेमवर्क पर, केवल इन स्थानों में लाइसेंस खोजने की कोशिश करता है:

1. स्पष्ट पथ।

2. क्लाइंट की कॉलिंग असेंबली में एक एम्बेडेड संसाधन।

2. घटक जार फ़ाइल का फ़ोल्डर।

### उदाहरण

इस उदाहरण में, MyLicense.lic नामक एक लाइसेंस फ़ाइल को फ़ोल्डर में खोजने का प्रयास किया जाएगा जिसमें है घटक, कॉलिंग असेंबली वाले फ़ोल्डर में, एंट्री असेंबली के फ़ोल्डर में और फिर कॉलिंग असेंबली के एम्बेडेड संसाधनों में।

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As License = New License
license.SetLicense("MyLicense.lic")
```

घटक जार फ़ाइल:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

फ़ाइल का पूरा या छोटा नाम हो सकता है या एक एम्बेडेड संसाधन का नाम. मूल्यांकन मोड पर स्विच करने के लिए खाली स्ट्रिंग का उपयोग करें।

### यह सभी देखें

* class [License](../)
* नाम स्थान [Aspose.Page](../../license/)
* सभा [Aspose.Page](../../../)

---

## SetLicense(Stream) {#setlicense}

घटक को लाइसेंस देता है।

```csharp
public void SetLicense(Stream stream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| stream | Stream | एक धारा जिसमें लाइसेंस शामिल है। |

### टिप्पणियों

स्ट्रीम से लाइसेंस लोड करने के लिए इस विधि का उपयोग करें।

### उदाहरण

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)

License license = new License();
license.setLicense(myStream);
```

### यह सभी देखें

* class [License](../)
* नाम स्थान [Aspose.Page](../../license/)
* सभा [Aspose.Page](../../../)


