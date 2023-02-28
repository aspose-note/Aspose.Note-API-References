---
title: Class License
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.License कक्ष. घटक क लइसेंस देने के तरके प्रदन करत है
type: docs
weight: 310
url: /hi/net/aspose.note/license/
---
## License class

घटक को लाइसेंस देने के तरीके प्रदान करता है।

```csharp
public class License
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [License](license/)() | डिफ़ॉल्ट कंस्ट्रक्टर। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense)(Stream) | घटक को लाइसेंस देता है। |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense_1)(string) | घटक को लाइसेंस देता है। |

### उदाहरण

दिखाता है कि किसी फ़ाइल से Aspose.Note के लिए लाइसेंस कैसे लोड किया जाए।

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

दिखाता है कि स्ट्रीम से Aspose.Note के लिए लाइसेंस कैसे लोड किया जाए।

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

एम्बेडेड फ़ाइल संसाधन से Aspose.Note के लिए लाइसेंस लोड करने का तरीका दिखाता है।

```csharp
// लाइसेंस क्लास को इंस्टेंट करें
Aspose.Note.License license = new Aspose.Note.License();

// केवल असेंबली में एम्बेड की गई लाइसेंस फ़ाइल का नाम पास करें
license.SetLicense("Aspose.Note.lic");
```

### यह सभी देखें

* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


