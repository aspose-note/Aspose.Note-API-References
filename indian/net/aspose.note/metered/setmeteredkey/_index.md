---
title: Metered.SetMeteredKey
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Metered तरक. सर्वजनक और नज कुंजयँ सेट करत है
type: docs
weight: 30
url: /hi/net/aspose.note/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

सार्वजनिक और निजी कुंजियाँ सेट करता है।

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| publicKey | String | सार्वजनिक कुंजी। |
| privateKey | String | निजी कुंजी। |

### टिप्पणियों

यदि आप मीटर्ड लाइसेंस खरीदते हैं, तो इस एपीआई को एप्लिकेशन स्टार्टअप पर कॉल किया जाना चाहिए, सामान्य रूप से, यह पर्याप्त है। हालांकि, यदि मीटर्ड 24 घंटे की अवधि के दौरान खपत डेटा अपलोड करने में विफल रहता है, तो लाइसेंस मूल्यांकन स्थिति पर सेट हो जाएगा। ऐसे मामले से बचने के लिए, आपको नियमित रूप से लाइसेंस की स्थिति की जांच करनी चाहिए यदि यह मूल्यांकन की स्थिति है, तो इस एपीआई को दोबारा कॉल करें।

### उदाहरण

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

* class [Metered](../)
* नाम स्थान [Aspose.Note](../../metered/)
* सभा [Aspose.Note](../../../)


