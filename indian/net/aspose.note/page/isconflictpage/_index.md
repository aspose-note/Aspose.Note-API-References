---
title: Page.IsConflictPage
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Page संपत्त. यह इंगत करने वल मन प्रप्त य सेट करत है क यह पृष्ठ एक वरध पृष्ठ है
type: docs
weight: 50
url: /hi/net/aspose.note/page/isconflictpage/
---
## Page.IsConflictPage property

यह इंगित करने वाला मान प्राप्त या सेट करता है कि यह पृष्ठ एक विरोध पृष्ठ है।

```csharp
public bool IsConflictPage { get; set; }
```

### टिप्पणियों

विरोध पृष्ठ तब उत्पन्न होता है जब दो उपयोगकर्ता एक ही सामग्री को अपडेट करने का प्रयास करते हैं। इस मामले में पहले उपयोगकर्ता के परिवर्तन हमेशा की तरह लिखे जाते हैं। लेकिन किसी अन्य उपयोगकर्ता के परिवर्तनों को मर्ज नहीं किया जा सकता है। तो बस पृष्ठ की एक प्रति बनाई जाती है और संघर्ष के रूप में चिह्नित।

इस संस्करण में पहले उपयोगकर्ता के परिवर्तनों के पक्ष में विरोधों का समाधान किया जाता है। इसलिए यदि दस्तावेज़ में विरोध पृष्ठ हैं तो उन्हें इतिहास में दिखाया जाएगा लेकिन सहेजने पर उन्हें छोड़ दिया जाएगा। इस पृष्ठ को सहेजने के लिए इस ध्वज को रीसेट करना संभव है इतिहास में हमेशा की तरह.

विरोध पृष्ठ द्वारा हेरफेर का विस्तृत नमूना ऑनलाइन दस्तावेज़ीकरण में पाया जा सकता है।

### उदाहरण

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

* class [Page](../)
* नाम स्थान [Aspose.Note](../../page/)
* सभा [Aspose.Note](../../../)


