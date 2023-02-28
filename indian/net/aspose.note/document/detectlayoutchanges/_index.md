---
title: Document.DetectLayoutChanges
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Document तरक. पछले के बद से दस्तवेज़ लेआउट में कए गए सभ परवर्तनं क पत लगत हैDetectLayoutChanges कल. ममले मेंAutomaticLayoutChangesDetectionEnabled सह पर सेट दस्तवेज़ नर्यत क शुरुआत में स्वचलत रूप से उपयग कय जत है
type: docs
weight: 90
url: /hi/net/aspose.note/document/detectlayoutchanges/
---
## Document.DetectLayoutChanges method

पिछले के बाद से दस्तावेज़ लेआउट में किए गए सभी परिवर्तनों का पता लगाता है`DetectLayoutChanges` कॉल. मामले में[`AutomaticLayoutChangesDetectionEnabled`](../automaticlayoutchangesdetectionenabled/) सही पर सेट, दस्तावेज़ निर्यात की शुरुआत में स्वचालित रूप से उपयोग किया जाता है।

```csharp
public void DetectLayoutChanges()
```

### उदाहरण

दस्तावेज़ को विभिन्न स्वरूपों में सहेजने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// नए दस्तावेज़ को प्रारंभ करें
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// नए पेज को इनिशियलाइज़ करें
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// दस्तावेज़ में सभी पाठ के लिए डिफ़ॉल्ट शैली।
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// पेज नोड जोड़ें
doc.AppendChildLast(page);

// OneNote दस्तावेज़ को विभिन्न स्वरूपों में सहेजें, टेक्स्ट फ़ॉन्ट आकार सेट करें और मैन्युअल रूप से लेआउट परिवर्तनों का पता लगाएं।
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

### यह सभी देखें

* class [Document](../)
* नाम स्थान [Aspose.Note](../../document/)
* सभा [Aspose.Note](../../../)


