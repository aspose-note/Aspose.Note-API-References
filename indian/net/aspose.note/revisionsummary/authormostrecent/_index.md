---
title: RevisionSummary.AuthorMostRecent
second_title: Aspose.Note .NET API संदर्भ के लिए
description: RevisionSummary संपत्त. सबसे हल के लेखक क प्रप्त य सेट करत है
type: docs
weight: 20
url: /hi/net/aspose.note/revisionsummary/authormostrecent/
---
## RevisionSummary.AuthorMostRecent property

सबसे हाल के लेखक को प्राप्त या सेट करता है।

```csharp
public string AuthorMostRecent { get; set; }
```

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

* class [RevisionSummary](../)
* नाम स्थान [Aspose.Note](../../revisionsummary/)
* सभा [Aspose.Note](../../../)


