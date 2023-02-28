---
title: Page.Title
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Page संपत्त. शर्षक प्रप्त य सेट करत है
type: docs
weight: 120
url: /hi/net/aspose.note/page/title/
---
## Page.Title property

शीर्षक प्राप्त या सेट करता है।

```csharp
public Title Title { get; set; }
```

### संपत्ति मूल्य

द`Title` .

### उदाहरण

दिखाता है कि किसी पृष्ठ के बारे में मेटा जानकारी कैसे प्राप्त करें।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Pages();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

foreach (Page page in oneFile)
{
    Console.WriteLine("LastModifiedTime: {0}", page.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", page.CreationTime);
    Console.WriteLine("Title: {0}", page.Title);
    Console.WriteLine("Level: {0}", page.Level);
    Console.WriteLine("Author: {0}", page.Author);
    Console.WriteLine();
}
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

दिखाता है कि पृष्ठ के लिए शीर्षक कैसे सेट करें।

```csharp
string dataDir = RunExamples.GetDataDir_Text();
string outputPath = dataDir + "CreateTitleMsStyle_out.one";

var doc = new Document();
var page = new Page(doc);

page.Title = new Title(doc)
{
    TitleText = new RichText(doc)
    {
        Text = "Title text.",
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleDate = new RichText(doc)
    {
        Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture),
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleTime = new RichText(doc)
    {
        Text = "12:34",
        ParagraphStyle = ParagraphStyle.Default
    }
};

doc.AppendChildLast(page);

doc.Save(outputPath);
```

दिखाता है कि पृष्ठ का इतिहास कैसे प्राप्त करें।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote दस्तावेज़ लोड करें
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// पहला पेज प्राप्त करें
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

दिखाता है कि एक दस्तावेज़ कैसे बनाया जाए और इसे डिफ़ॉल्ट विकल्पों का उपयोग करके HTML प्रारूप में कैसे सहेजा जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote दस्तावेज़ को प्रारंभ करें
Document doc = new Document();
Page page = doc.AppendChildLast(new Page());

// दस्तावेज़ में सभी पाठ के लिए डिफ़ॉल्ट शैली।
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
                 {
                     TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                     TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                     TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
                 };

// HTML फॉर्मेट में सेव करें
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

दिखाता है कि दस्तावेज़ कैसे बनाया जाए और HTML प्रारूप में निर्दिष्ट पृष्ठों की श्रेणी में सहेजा जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// OneNote दस्तावेज़ को प्रारंभ करें
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// दस्तावेज़ में सभी पाठ के लिए डिफ़ॉल्ट शैली।
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// HTML फॉर्मेट में सेव करें
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

शीर्षक वाले पृष्ठ के साथ दस्तावेज़ बनाने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
Document doc = new Aspose.Note.Document();

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// दस्तावेज़ में सभी पाठ के लिए डिफ़ॉल्ट शैली।
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// पृष्ठ शीर्षक गुण सेट करें
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// दस्तावेज़ में पेज नोड जोड़ें
doc.AppendChildLast(page);

// OneNote दस्तावेज़ सहेजें
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

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

* class [Title](../../title/)
* class [Page](../)
* नाम स्थान [Aspose.Note](../../page/)
* सभा [Aspose.Note](../../../)


