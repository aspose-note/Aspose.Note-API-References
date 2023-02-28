---
title: Document.AutomaticLayoutChangesDetectionEnabled
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Document संपत्त. एक मन प्रप्त य सेट करत है ज इंगत करत है क Aspose.Note स्वचलत रूप से लेआउट परवर्तनं क पत लगत है डफ़ल्ट मन हैसत्य .
type: docs
weight: 20
url: /hi/net/aspose.note/document/automaticlayoutchangesdetectionenabled/
---
## Document.AutomaticLayoutChangesDetectionEnabled property

एक मान प्राप्त या सेट करता है जो इंगित करता है कि Aspose.Note स्वचालित रूप से लेआउट परिवर्तनों का पता लगाता है। डिफ़ॉल्ट मान है`सत्य` .

```csharp
public bool AutomaticLayoutChangesDetectionEnabled { get; set; }
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


