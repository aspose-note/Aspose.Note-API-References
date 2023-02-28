---
title: RichText.Replace
second_title: Aspose.Note .NET API संदर्भ के लिए
description: RichText तरक. इस उदहरण में एक नर्दष्ट यूनकड वर्ण क सभ घटनओं क दूसरे नर्दष्ट यूनकड वर्ण के सथ बदल देत है
type: docs
weight: 200
url: /hi/net/aspose.note/richtext/replace/
---
## Replace(char, char) {#replace}

इस उदाहरण में एक निर्दिष्ट यूनिकोड वर्ण की सभी घटनाओं को दूसरे निर्दिष्ट यूनिकोड वर्ण के साथ बदल देता है।

```csharp
public RichText Replace(char oldChar, char newChar)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| oldChar | Char | पुराना वर्ण. |
| newChar | Char | नया वर्ण. |

### प्रतिलाभ की मात्रा

द[`RichText`](../) .

### यह सभी देखें

* class [RichText](../)
* नाम स्थान [Aspose.Note](../../richtext/)
* सभा [Aspose.Note](../../../)

---

## Replace(string, string) {#replace_1}

वर्तमान उदाहरण में निर्दिष्ट स्ट्रिंग की सभी घटनाओं को अन्य निर्दिष्ट स्ट्रिंग के साथ बदलता है।

```csharp
public RichText Replace(string oldValue, string newValue)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| oldValue | String | पुराना मान। |
| newValue | String | नया मान। |

### प्रतिलाभ की मात्रा

द[`RichText`](../) .

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### उदाहरण

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

दिखाता है कि किसी टेम्प्लेट में विशेष टेक्स्ट के टुकड़ों को बदलकर एक नया दस्तावेज़ कैसे बनाया जाता है।

```csharp
string dataDir = RunExamples.GetDataDir_Text();

var D = new Dictionary<string, string>
            {
                { "Company", "Atlas Shrugged Ltd" },
                { "CandidateName", "John Galt" },
                { "JobTitle", "Chief Entrepreneur Officer" },
                { "Department", "Sales" },
                { "Salary", "123456 USD" },
                { "Vacation", "30" },
                { "StartDate", "29 Feb 2024" },
                { "YourName", "Ayn Rand" }
            };

// टेम्पलेट दस्तावेज़ को Aspose.Note में लोड करें।
var d = new Document(Path.Combine(dataDir, "JobOffer.one"));

// आइए सभी टेम्प्लेट शब्दों को बदलें
foreach (var e in d.GetChildNodes<RichText>())
{
    foreach (var replace in D)
    {
        e.Replace($"${{{replace.Key}}}", replace.Value);
    }
}

d.Save(Path.Combine(dataDir, "JobOffer_out.one"));
```

### यह सभी देखें

* class [RichText](../)
* नाम स्थान [Aspose.Note](../../richtext/)
* सभा [Aspose.Note](../../../)

---

## Replace(string, string, TextStyle) {#replace_2}

वर्तमान उदाहरण में निर्दिष्ट स्ट्रिंग की सभी घटनाओं को निर्दिष्ट शैली में अन्य निर्दिष्ट स्ट्रिंग के साथ बदलता है।

```csharp
public RichText Replace(string oldValue, string newValue, TextStyle style)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| oldValue | String | पुराना मान। |
| newValue | String | नया मान। |
| style | TextStyle | नए मान की शैली. |

### प्रतिलाभ की मात्रा

द[`RichText`](../) .

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### यह सभी देखें

* class [TextStyle](../../textstyle/)
* class [RichText](../)
* नाम स्थान [Aspose.Note](../../richtext/)
* सभा [Aspose.Note](../../../)


