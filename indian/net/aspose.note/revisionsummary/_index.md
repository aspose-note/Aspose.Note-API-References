---
title: Class RevisionSummary
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.RevisionSummary कक्ष. नड के संशधन के लए सरंश क प्रतनधत्व करत है
type: docs
weight: 520
url: /hi/net/aspose.note/revisionsummary/
---
## RevisionSummary class

नोड के संशोधन के लिए सारांश का प्रतिनिधित्व करता है।

```csharp
public class RevisionSummary
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [RevisionSummary](revisionsummary/)() | डिफ़ॉल्ट कंस्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [AuthorMostRecent](../../aspose.note/revisionsummary/authormostrecent/) { get; set; } | सबसे हाल के लेखक को प्राप्त या सेट करता है। |
| [LastModifiedTime](../../aspose.note/revisionsummary/lastmodifiedtime/) { get; set; } | अंतिम संशोधित समय प्राप्त या सेट करता है। |

### उदाहरण

पेज की मेटा जानकारी को संपादित करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote दस्तावेज़ लोड करें और पहला बच्चा प्राप्त करें           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

// इस पृष्ठ के लिए सामग्री संशोधन सारांश पढ़ना
var pageRevisionInfo = page.PageContentRevisionSummary;

Console.WriteLine(string.Format(
    "Author:\t{0}\nModified:\t{1}",
    pageRevisionInfo.AuthorMostRecent,
    pageRevisionInfo.LastModifiedTime.ToString("dd.MM.yyyy HH:mm:ss")));

// इस पृष्ठ के लिए अद्यतन पृष्ठ संशोधन सारांश
pageRevisionInfo.AuthorMostRecent = "New Author";
pageRevisionInfo.LastModifiedTime = DateTime.Now;

document.Save(dataDir + "WorkingWithPageRevisions_out.one");
```

दिखाता है कि कैसे जांचें कि कोई पृष्ठ एक विरोध पृष्ठ है (अर्थात इसमें परिवर्तन हैं कि OneNote स्वचालित रूप से विलय नहीं कर सका)।

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote दस्तावेज़ लोड करें
Document doc = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

var history = doc.GetPageHistory(doc.FirstChild);
for (int i = 0; i < history.Count; i++)
{
    var historyPage = history[i];
    Console.Write("    {0}. Author: {1}, {2:dd.MM.yyyy hh.mm.ss}",
                    i,
                    historyPage.PageContentRevisionSummary.AuthorMostRecent,
                    historyPage.PageContentRevisionSummary.LastModifiedTime);
    Console.WriteLine(historyPage.IsConflictPage ? ", IsConflict: true" : string.Empty);

    // डिफ़ॉल्ट रूप से विरोध पृष्ठों को सहेजने पर छोड़ दिया जाता है।
    // यदि इसे गैर-संघर्ष के रूप में चिह्नित किया जाता है तो इसे हमेशा की तरह इतिहास में सहेजा जाएगा।
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### यह सभी देखें

* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


