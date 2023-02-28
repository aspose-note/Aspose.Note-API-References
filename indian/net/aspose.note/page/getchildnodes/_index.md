---
title: Page.GetChildNodes
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Page तरक. पृष्ठ के सभ चइल्ड नड्स क नड प्रकर से प्रप्त करें
type: docs
weight: 150
url: /hi/net/aspose.note/page/getchildnodes/
---
## Page.GetChildNodes&lt;T1&gt; method

पृष्ठ के सभी चाइल्ड नोड्स को नोड प्रकार से प्राप्त करें।

```csharp
public override List<T1> GetChildNodes<T1>()
    where T1 : class, INode
```

| पैरामीटर | विवरण |
| --- | --- |
| T1 | लौटाई गई सूची में तत्वों का प्रकार। |

### प्रतिलाभ की मात्रा

चाइल्ड नोड्स की सूची।

### उदाहरण

दस्तावेज़ से सभी पाठ प्राप्त करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Text();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

// पाठ पुनर्प्राप्त करें
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// आउटपुट स्क्रीन पर टेक्स्ट प्रिंट करें
Console.WriteLine(text);
```

दिखाता है कि पृष्ठ से सभी पाठ कैसे प्राप्त करें।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Text();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

// पेज नोड्स की सूची प्राप्त करें
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // पाठ पुनर्प्राप्त करें
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // आउटपुट स्क्रीन पर टेक्स्ट प्रिंट करें
    Console.WriteLine(text);
}
```

दिखाता है कि कैसे सभी पृष्ठों से गुजरना है और पाठ में एक प्रतिस्थापन करना है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

// सभी रिचटेक्स्ट नोड्स प्राप्त करें
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // किसी आकृति का पाठ बदलें
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// किसी भी समर्थित फ़ाइल स्वरूप में सहेजें
oneFile.Save(dataDir, SaveFormat.Pdf);
```

दिखाता है कि पेज के टेक्स्ट को कैसे पास करना है और कैसे रिप्लेसमेंट करना है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// सभी रिचटेक्स्ट नोड्स प्राप्त करें
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // किसी आकृति का पाठ बदलें
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// किसी भी समर्थित फ़ाइल स्वरूप में सहेजें
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

### यह सभी देखें

* interface [INode](../../inode/)
* class [Page](../)
* नाम स्थान [Aspose.Note](../../page/)
* सभा [Aspose.Note](../../../)


