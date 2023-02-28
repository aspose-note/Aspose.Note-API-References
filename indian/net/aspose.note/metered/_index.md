---
title: Class Metered
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.Metered कक्ष. मटर्ड कुंज सेट करने के तरके प्रदन करत है
type: docs
weight: 350
url: /hi/net/aspose.note/metered/
---
## Metered class

मीटर्ड कुंजी सेट करने के तरीके प्रदान करता है।

```csharp
public class Metered
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [Metered](metered/)() | डिफ़ॉल्ट कंस्ट्रक्टर। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| [ResetMeteredKey](../../aspose.note/metered/resetmeteredkey/)() | पहले के सेटअप लाइसेंस को हटाता है। |
| [SetMeteredKey](../../aspose.note/metered/setmeteredkey/)(string, string) | सार्वजनिक और निजी कुंजियाँ सेट करता है। |
| static [GetConsumptionCredit](../../aspose.note/metered/getconsumptioncredit/)() | उपभोग क्रेडिट प्राप्त करता है। |
| static [GetConsumptionQuantity](../../aspose.note/metered/getconsumptionquantity/)() | उपभोग फ़ाइल आकार प्राप्त करता है। |

### उदाहरण

इस उदाहरण में, मीटर्ड सार्वजनिक और निजी कुंजी सेट करने का प्रयास किया जाएगा

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

दिखाता है कि मीटर्ड लाइसेंस कैसे सेट करें।

```csharp
Metered metered = new Metered();
metered.SetMeteredKey("MyPublicKey", "MyPrivateKey");

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");

// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote दस्तावेज़ लोड करें और पहला बच्चा प्राप्त करें           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

document.Save(Path.Combine(dataDir, "MeteredLicense.pdf"));

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");
```

### यह सभी देखें

* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


