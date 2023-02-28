---
title: Document.GetPageHistory
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Document तरक. ह जत हैPageHistory जसमें एक दस्तवेज़ में प्रस्तुत प्रत्येक पृष्ठ के लए पूर इतहस हत है जल्द से जल्द सूचकंक 0 पर वर्तमन पृष्ठ संशधन के रूप में पहुँच ज सकत हैCurrent और ऐतहसक संस्करणं के संग्रह से अलग समहत है
type: docs
weight: 100
url: /hi/net/aspose.note/document/getpagehistory/
---
## Document.GetPageHistory method

हो जाता है[`PageHistory`](../../pagehistory/) जिसमें एक दस्तावेज़ में प्रस्तुत प्रत्येक पृष्ठ के लिए पूरा इतिहास होता है (जल्द से जल्द सूचकांक 0 पर)। वर्तमान पृष्ठ संशोधन के रूप में पहुँचा जा सकता है[`Current`](../../pagehistory/current/) और ऐतिहासिक संस्करणों के संग्रह से अलग समाहित है।

```csharp
public PageHistory GetPageHistory(Page page)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| page | Page | पृष्ठ का वर्तमान संशोधन। |

### प्रतिलाभ की मात्रा

द[`PageHistory`](../../pagehistory/) .

### उदाहरण

पृष्ठ के पिछले संस्करण को पुनर्स्थापित करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote दस्तावेज़ लोड करें और पहला बच्चा प्राप्त करें           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

पृष्ठ के इतिहास को संपादित करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote दस्तावेज़ लोड करें और पहला बच्चा प्राप्त करें           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
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

* class [PageHistory](../../pagehistory/)
* class [Page](../../page/)
* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)


