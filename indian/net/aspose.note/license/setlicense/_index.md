---
title: License.SetLicense
second_title: Aspose.Note .NET API संदर्भ के लिए
description: License तरक. घटक क लइसेंस देत है
type: docs
weight: 20
url: /hi/net/aspose.note/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

घटक को लाइसेंस देता है।

```csharp
public void SetLicense(string licenseName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| licenseName | String | एक पूर्ण या छोटा फ़ाइल नाम या एम्बेडेड संसाधन का नाम हो सकता है। मूल्यांकन मोड पर स्विच करने के लिए एक खाली स्ट्रिंग का उपयोग करें। |

### टिप्पणियों

निम्न स्थानों में लाइसेंस ढूँढने का प्रयास करता है:

1. स्पष्ट पथ।

2. वह फ़ोल्डर जिसमें Aspose घटक असेंबली है।

3. क्लाइंट की कॉलिंग असेंबली वाला फ़ोल्डर।

4. फ़ोल्डर जिसमें प्रविष्टि (स्टार्टअप) असेंबली है।

5. ग्राहक की कॉलिंग असेंबली में एक एम्बेडेड संसाधन।

**टिप्पणी:**.NET कॉम्पैक्ट फ्रेमवर्क पर, केवल इन स्थानों में लाइसेंस खोजने की कोशिश करता है:

1. स्पष्ट पथ।

2. क्लाइंट की कॉलिंग असेंबली में एक एम्बेडेड संसाधन।

### उदाहरण

दिखाता है कि किसी फ़ाइल से Aspose.Note के लिए लाइसेंस कैसे लोड किया जाए।

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

एम्बेडेड फ़ाइल संसाधन से Aspose.Note के लिए लाइसेंस लोड करने का तरीका दिखाता है।

```csharp
// लाइसेंस क्लास को इंस्टेंट करें
Aspose.Note.License license = new Aspose.Note.License();

// केवल असेंबली में एम्बेड की गई लाइसेंस फ़ाइल का नाम पास करें
license.SetLicense("Aspose.Note.lic");
```

### यह सभी देखें

* class [License](../)
* नाम स्थान [Aspose.Note](../../license/)
* सभा [Aspose.Note](../../../)

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

दिखाता है कि स्ट्रीम से Aspose.Note के लिए लाइसेंस कैसे लोड किया जाए।

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

### यह सभी देखें

* class [License](../)
* नाम स्थान [Aspose.Note](../../license/)
* सभा [Aspose.Note](../../../)


