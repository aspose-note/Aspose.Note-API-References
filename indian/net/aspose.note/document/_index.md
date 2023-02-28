---
title: Class Document
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.Document कक्ष. एक Aspose.Note दस्तवेज़ क प्रतनधत्व करत है
type: docs
weight: 60
url: /hi/net/aspose.note/document/
---
## Document class

एक Aspose.Note दस्तावेज़ का प्रतिनिधित्व करता है।

```csharp
public class Document : CompositeNode<Page>, INotebookChildNode
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [Document](document/#constructor)() | का एक नया उदाहरण प्रारंभ करता है`Document` class. एक रिक्त OneNote दस्तावेज़ बनाता है. |
| [Document](document/#constructor_1)(Stream) | का एक नया उदाहरण प्रारंभ करता है`Document` class. स्ट्रीम से मौजूदा OneNote दस्तावेज़ खोलता है. |
| [Document](document/#constructor_3)(string) | का एक नया उदाहरण प्रारंभ करता है`Document` class. फ़ाइल से मौजूदा OneNote दस्तावेज़ खोलता है. |
| [Document](document/#constructor_2)(Stream, LoadOptions) | का एक नया उदाहरण प्रारंभ करता है`Document` class. स्ट्रीम से मौजूदा OneNote दस्तावेज़ खोलता है। एन्क्रिप्शन पासवर्ड जैसे अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है. |
| [Document](document/#constructor_4)(string, LoadOptions) | का एक नया उदाहरण प्रारंभ करता है`Document`class. फ़ाइल से मौजूदा OneNote दस्तावेज़ खोलता है। एन्क्रिप्शन पासवर्ड जैसे अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है. |

## गुण

| नाम | विवरण |
| --- | --- |
| [AutomaticLayoutChangesDetectionEnabled](../../aspose.note/document/automaticlayoutchangesdetectionenabled/) { get; set; } | एक मान प्राप्त या सेट करता है जो इंगित करता है कि Aspose.Note स्वचालित रूप से लेआउट परिवर्तनों का पता लगाता है। डिफ़ॉल्ट मान है`सत्य` . |
| [Color](../../aspose.note/document/color/) { get; set; } | रंग प्राप्त या सेट करता है। |
| [CreationTime](../../aspose.note/document/creationtime/) { get; set; } | निर्माण समय प्राप्त या सेट करता है। |
| [DisplayName](../../aspose.note/document/displayname/) { get; set; } | प्रदर्शन नाम प्राप्त या सेट करता है। |
| [Document](../../aspose.note/node/document/) { get; } | नोड का दस्तावेज़ प्राप्त करता है। |
| [FileFormat](../../aspose.note/document/fileformat/) { get; } | फ़ाइल स्वरूप प्राप्त करता है (OneNote 2010, OneNote ऑनलाइन)। |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [Guid](../../aspose.note/document/guid/) { get; } | वस्तु की विश्व स्तर पर अद्वितीय आईडी प्राप्त करता है। |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | उसी नोड ट्री स्तर पर अगला नोड प्राप्त करता है। |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | नोड प्रकार प्राप्त करता है। |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | मूल नोड प्राप्त करता है। |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | पिछले नोड को उसी नोड ट्री स्तर पर प्राप्त करता है। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| override [Accept](../../aspose.note/document/accept/)(DocumentVisitor) | नोड के आगंतुक को स्वीकार करता है। |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| [DetectLayoutChanges](../../aspose.note/document/detectlayoutchanges/)() | पिछले के बाद से दस्तावेज़ लेआउट में किए गए सभी परिवर्तनों का पता लगाता है[`DetectLayoutChanges`](./detectlayoutchanges/) कॉल. मामले में[`AutomaticLayoutChangesDetectionEnabled`](./automaticlayoutchangesdetectionenabled/) सही पर सेट, दस्तावेज़ निर्यात की शुरुआत में स्वचालित रूप से उपयोग किया जाता है। |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| [GetPageHistory](../../aspose.note/document/getpagehistory/)(Page) | हो जाता है[`PageHistory`](../pagehistory/) जिसमें एक दस्तावेज़ में प्रस्तुत प्रत्येक पृष्ठ के लिए पूरा इतिहास होता है (जल्द से जल्द सूचकांक 0 पर)। वर्तमान पृष्ठ संशोधन के रूप में पहुँचा जा सकता है[`Current`](../pagehistory/current/) और ऐतिहासिक संस्करणों के संग्रह से अलग समाहित है। |
| [Import](../../aspose.note/document/import/#import)(Stream, PdfImportOptions, MergeOptions) | प्रदान किए गए पीडीएफ दस्तावेज़ से पृष्ठों का एक सेट आयात करता है। |
| [Import](../../aspose.note/document/import/#import_1)(string, PdfImportOptions, MergeOptions) | प्रदान किए गए पीडीएफ दस्तावेज़ से पृष्ठों का एक सेट आयात करता है। |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;Page&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params Page[]) |  |
| [Merge](../../aspose.note/document/merge/)(IEnumerable&lt;Page&gt;, MergeOptions) | पृष्ठों के एक सेट को दस्तावेज़ में मर्ज करता है। |
| [Print](../../aspose.note/document/print/#print)() | दस्तावेज़ को डिफ़ॉल्ट प्रिंटर का उपयोग करके प्रिंट करता है. |
| [Print](../../aspose.note/document/print/#print_1)(PrintOptions) | दस्तावेज़ को डिफ़ॉल्ट प्रिंटर का उपयोग करके प्रिंट करता है. |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |
| [Save](../../aspose.note/document/save/#save)(Stream) | OneNote दस्तावेज़ को स्ट्रीम में सहेजता है. |
| [Save](../../aspose.note/document/save/#save_3)(string) | OneNote दस्तावेज़ को फ़ाइल में सहेजता है. |
| [Save](../../aspose.note/document/save/#save_1)(Stream, SaveFormat) | निर्दिष्ट प्रारूप में एक स्ट्रीम में OneNote दस्तावेज़ सहेजता है। |
| [Save](../../aspose.note/document/save/#save_2)(Stream, SaveOptions) | निर्दिष्ट सहेजें विकल्पों का उपयोग करके OneNote दस्तावेज़ को स्ट्रीम में सहेजता है. |
| [Save](../../aspose.note/document/save/#save_4)(string, SaveFormat) | OneNote दस्तावेज़ को निर्दिष्ट स्वरूप में फ़ाइल में सहेजता है. |
| [Save](../../aspose.note/document/save/#save_5)(string, SaveOptions) | निर्दिष्ट सहेजें विकल्पों का उपयोग करके OneNote दस्तावेज़ को फ़ाइल में सहेजता है. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted)(Stream, out Document) | जांचता है कि स्ट्रीम से कोई दस्तावेज़ एन्क्रिप्ट किया गया है या नहीं। इसे जांचने के लिए हमें इस दस्तावेज़ को पूरी तरह लोड करने की आवश्यकता है। तो इस विधि से प्रदर्शन जुर्माना हो सकता है। |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_3)(string, out Document) | जांचता है कि फ़ाइल से कोई दस्तावेज़ एन्क्रिप्ट किया गया है या नहीं। इसे जांचने के लिए हमें इस दस्तावेज़ को पूरी तरह लोड करने की आवश्यकता है। तो इस विधि से प्रदर्शन जुर्माना हो सकता है। |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_1)(Stream, LoadOptions, out Document) | जांचता है कि स्ट्रीम से कोई दस्तावेज़ एन्क्रिप्ट किया गया है या नहीं। इसे जांचने के लिए हमें इस दस्तावेज़ को पूरी तरह लोड करने की आवश्यकता है। तो इस विधि से प्रदर्शन जुर्माना हो सकता है। |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_2)(Stream, string, out Document) | जांचता है कि स्ट्रीम से कोई दस्तावेज़ एन्क्रिप्ट किया गया है या नहीं। इसे जांचने के लिए हमें इस दस्तावेज़ को पूरी तरह लोड करने की आवश्यकता है। तो इस विधि से प्रदर्शन जुर्माना हो सकता है। |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_4)(string, LoadOptions, out Document) | जांचता है कि फ़ाइल से कोई दस्तावेज़ एन्क्रिप्ट किया गया है या नहीं। इसे जांचने के लिए हमें इस दस्तावेज़ को पूरी तरह लोड करने की आवश्यकता है। तो इस विधि से प्रदर्शन जुर्माना हो सकता है। |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_5)(string, string, out Document) | जांचता है कि फ़ाइल से कोई दस्तावेज़ एन्क्रिप्ट किया गया है या नहीं। इसे जांचने के लिए हमें इस दस्तावेज़ को पूरी तरह लोड करने की आवश्यकता है। तो इस विधि से प्रदर्शन जुर्माना हो सकता है। |

### उदाहरण

डिफ़ॉल्ट विकल्पों के साथ मानक विंडोज संवाद का उपयोग करके प्रिंटर को दस्तावेज़ भेजने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
```

दस्तावेज़ को सहेजने का तरीका दिखाता है।

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

एक एन्क्रिप्टेड दस्तावेज़ को कैसे दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

दिखाता है कि एन्क्रिप्शन के साथ दस्तावेज़ को कैसे सहेजना है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

दिखाता है कि SaveFormat गणन का उपयोग करके दस्तावेज़ को कैसे सहेजना है।

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

दिखाता है कि OneSaveOptions का उपयोग करके किसी दस्तावेज़ को कैसे सहेजना है।

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

दिखाता है कि किसी दस्तावेज़ के पृष्ठ की संख्या कैसे प्राप्त करें।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Pages();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

// पृष्ठों की संख्या प्राप्त करें
int count = oneFile.Count();

// आउटपुट स्क्रीन पर प्रिंट काउंट
Console.WriteLine(count);
```

दिखाता है कि डिफ़ॉल्ट सेटिंग्स का उपयोग करके किसी दस्तावेज़ को पीडीएफ प्रारूप में कैसे सहेजा जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

// दस्तावेज़ को पीडीएफ के रूप में सहेजें
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

किसी दस्तावेज़ को GIF प्रारूप में सहेजने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// दस्तावेज़ को GIF के रूप में सहेजें।
oneFile.Save(dataDir, SaveFormat.Gif);
```

जेपीईजी प्रारूप में दस्तावेज़ को छवि के रूप में सहेजते समय छवि गुणवत्ता कैसे सेट करें दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// दस्तावेज़ को सहेजें।
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

दस्तावेज़ को छवि के रूप में सहेजते समय छवि रिज़ॉल्यूशन सेट करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// दस्तावेज़ को सहेजें।
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

दस्तावेज़ का फ़ाइल स्वरूप प्राप्त करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // प्रक्रिया OneNote 2010
        break;
    case FileFormat.OneNoteOnline:
        // प्रक्रिया OneNote ऑनलाइन
        break;
}
```

दिखाता है कि हाइपरलिंक को इमेज से कैसे बाइंड किया जाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

किसी दस्तावेज़ को स्ट्रीम में सहेजने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// स्ट्रीम की स्थिति को वापस शून्य पर रिवाइंड करें ताकि यह अगले पाठक के लिए तैयार हो।
dstStream.Seek(0, SeekOrigin.Begin);
```

दिखाता है कि कैसे जांचें कि कोई दस्तावेज़ पासवर्ड से सुरक्षित है या नहीं।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

दिखाता है कि किसी नोटबुक में नया अनुभाग कैसे जोड़ा जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();

// एक OneNote नोटबुक लोड करें
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// नोटबुक में एक नया बच्चा जोड़ें
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// नोटबुक को सेव करें
notebook.Save(dataDir);
```

दिखाता है कि कैसे जांचें कि दस्तावेज़ लोड विफल हो गया है क्योंकि OneNote 2007 प्रारूप समर्थित नहीं है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "OneNote2007.one");

try
{
    new Document(fileName);
}
catch (UnsupportedFileFormatException e)
{
    if (e.FileFormat == FileFormat.OneNote2007)
    {
        Console.WriteLine("It looks like the provided file is in OneNote 2007 format that is not supported.");
    }
    else
        throw;
}
```

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

पेज को क्लोन करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote दस्तावेज़ लोड करें
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// इतिहास के बिना नए दस्तावेज़ में क्लोन करें
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// इतिहास के साथ नए दस्तावेज़ में क्लोन करें
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

सभी संसाधनों (सीएसएस/फोंट/छवियों) को एक अलग फाइल में संग्रहीत करने के साथ एचटीएमएल प्रारूप में एक दस्तावेज़ को बचाने का तरीका दिखाता है।

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportAsStream,
                 ExportFonts = ResourceExportType.ExportAsStream,
                 ExportImages = ResourceExportType.ExportAsStream,
                 FontFaceTypes = FontFaceType.Ttf
             };
document.Save(dataDir + "document_out.html", options);
```

सभी संसाधनों (सीएसएस/फोंट/छवियों) के एम्बेडिंग के साथ एचटीएमएल प्रारूप में एक दस्तावेज़ को स्ट्रीम में सहेजने का तरीका दिखाता है।

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportEmbedded,
                 ExportFonts = ResourceExportType.ExportEmbedded,
                 ExportImages = ResourceExportType.ExportEmbedded,
                 FontFaceTypes = FontFaceType.Ttf
             };

var r = new MemoryStream();
document.Save(r, options);
```

छवि के लिए टेक्स्ट विवरण सेट करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page(document);
var image = new Image(document, dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

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

जब लंबे OneNote पृष्ठ pdf स्वरूप में सहेजे जाते हैं, तो वे पृष्ठों में विभाजित हो जाते हैं. नमूना दिखाता है कि पृष्ठ के विरामों पर स्थित वस्तुओं के विभाजन तर्क को कैसे कॉन्फ़िगर किया जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// या
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

दिखाता है कि दस्तावेज़ को पीएनजी प्रारूप में कैसे सहेजना है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

// ImageSaveOptions ऑब्जेक्ट को इनिशियलाइज़ करें 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // पेज इंडेक्स सेट करें
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// दस्तावेज़ को पीएनजी के रूप में सहेजें।
oneFile.Save(dataDir, opts);
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

दिखाता है कि कैसे जांचें कि कोई दस्तावेज़ विशिष्ट पासवर्ड द्वारा पासवर्ड से सुरक्षित है या नहीं।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

किसी दस्तावेज़ में डार्क थीम शैली को लागू करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Text();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
```

दिखाता है कि नोटबुक की सामग्री को कैसे पास किया जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = "Open Notebook.onetoc2";
try
{
    var notebook = new Notebook(dataDir + fileName);
    foreach (var notebookChildNode in notebook)
    {
        Console.WriteLine(notebookChildNode.DisplayName);
        if (notebookChildNode is Document)
        {
            // चाइल्ड डॉक्यूमेंट के साथ कुछ करें
        }
        else if (notebookChildNode is Notebook)
        {
            // चाइल्ड नोटबुक के साथ कुछ करें
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

दस्तावेज़ से छवि प्राप्त करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Images();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

// सभी छवि नोड्स प्राप्त करें
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // इमेज बाइट्स को फाइल में सेव करें
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

दिखाता है कि पीडीएफ प्रारूप में दस्तावेज़ को कैसे सहेजना है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

// PdfSaveOptions ऑब्जेक्ट को इनिशियलाइज़ करें
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // सहेजे जाने वाले पहले पेज का पेज इंडेक्स सेट करें
                              PageIndex = 0,

                              // पेज काउंट सेट करें
                              PageCount = 1,
                          };

// दस्तावेज़ को पीडीएफ के रूप में सहेजें
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

दिखाता है कि विशिष्ट सेटिंग्स का उपयोग करके दस्तावेज़ को पीडीएफ प्रारूप में कैसे सहेजा जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document doc = new Document(dataDir + "Aspose.one");

// PdfSaveOptions ऑब्जेक्ट को इनिशियलाइज़ करें
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // जेपीईजी संपीड़न का प्रयोग करें
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // जेपीईजी संपीड़न के लिए गुणवत्ता
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

निर्दिष्ट विकल्पों के साथ मानक विंडोज संवाद का उपयोग करके प्रिंटर को दस्तावेज़ भेजने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
               {
                   PrinterSettings = printerSettings,
                   Resolution = 1200,
                   PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
                   DocumentName = "Test.one"
               });
```

संलग्न फ़ाइल की सामग्री प्राप्त करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Attachments();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Sample1.one");

// संलग्न फ़ाइल नोड्स की सूची प्राप्त करें
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// सभी नोड्स के माध्यम से पुनरावृति करें
foreach (AttachedFile file in nodes)
{
    // संलग्न फ़ाइल को स्ट्रीम ऑब्जेक्ट में लोड करें
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // एक स्थानीय फ़ाइल बनाएँ
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // फ़ाइल स्ट्रीम कॉपी करें
            CopyStream(outputStream, fileStream);
        }
    }
}
```

छवि की मेटा जानकारी प्राप्त करने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Images();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document oneFile = new Document(dataDir + "Aspose.one");

// सभी छवि नोड्स प्राप्त करें
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
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

फ़ाइलपथ का उपयोग करके दस्तावेज़ में फ़ाइल जोड़ने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Attachments();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
Document doc = new Document();

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// आउटलाइन क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Outline outline = new Outline(doc);

// आउटलाइन एलिमेंट क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
OutlineElement outlineElem = new OutlineElement(doc);

// अटैच्डफाइल क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// संलग्न फ़ाइल जोड़ें
outlineElem.AppendChildLast(attachedFile);

// रूपरेखा तत्व नोड जोड़ें
outline.AppendChildLast(outlineElem);

// आउटलाइन नोड जोड़ें
page.AppendChildLast(outline);

// पेज नोड जोड़ें
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
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

उपयोगकर्ता परिभाषित गुणों के साथ फ़ाइल से दस्तावेज़ में छवि जोड़ने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Images();

// धारा से दस्तावेज़ लोड करें।
Document doc = new Document(dataDir + "Aspose.one");

// दस्तावेज़ का पहला पृष्ठ प्राप्त करें।
Aspose.Note.Page page = doc.FirstChild;

// फ़ाइल से एक छवि लोड करें।
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // अपनी आवश्यकताओं के अनुसार छवि का आकार बदलें (वैकल्पिक)।
                              Width = 100,
                              Height = 100,

                              // पृष्ठ में छवि का स्थान सेट करें (वैकल्पिक)।
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // छवि संरेखण सेट करें
                              Alignment = HorizontalAlignment.Right
                          };

// छवि को पेज में जोड़ें।
page.AppendChildLast(image);
```

दिखाता है कि किसी फ़ाइल को स्ट्रीम से दस्तावेज़ में कैसे जोड़ा जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Attachments();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
Document doc = new Document();

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// आउटलाइन क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Outline outline = new Outline(doc);

// आउटलाइन एलिमेंट क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // अटैच्डफाइल क्लास ऑब्जेक्ट को इनिशियलाइज़ करें और इसके आइकन पाथ को भी पास करें
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // संलग्न फ़ाइल जोड़ें
    outlineElem.AppendChildLast(attachedFile);
}

// रूपरेखा तत्व नोड जोड़ें
outline.AppendChildLast(outlineElem);

// आउटलाइन नोड जोड़ें
page.AppendChildLast(outline);

// पेज नोड जोड़ें
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

जब लंबे OneNote पृष्ठ pdf स्वरूप में सहेजे जाते हैं, तो वे पृष्ठों में विभाजित हो जाते हैं. उदाहरण दिखाता है कि पृष्ठ के विरामों पर स्थित वस्तुओं के विभाजन तर्क को कैसे कॉन्फ़िगर किया जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ को Aspose.Note में लोड करें।
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// या
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// या
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// या
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// या
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
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

दिखाता है कि किसी छवि को स्ट्रीम से किसी दस्तावेज़ में कैसे जोड़ा जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Images();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
Document doc = new Document();

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // छवि नाम, एक्सटेंशन और स्ट्रीम का उपयोग करके दूसरी छवि लोड करें।
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // छवि संरेखण सेट करें
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// OneNote दस्तावेज़ सहेजें
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

फ़ाइल से दस्तावेज़ में छवि जोड़ने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Images();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
Document doc = new Document();

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// आउटलाइन क्लास ऑब्जेक्ट को इनिशियलाइज़ करें और ऑफ़सेट प्रॉपर्टी सेट करें
Outline outline = new Outline(doc);

// आउटलाइन एलिमेंट क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
OutlineElement outlineElem = new OutlineElement(doc);

// फ़ाइल पथ द्वारा एक छवि लोड करें।
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // छवि संरेखण सेट करें
                              Alignment = HorizontalAlignment.Right
                          };

// छवि जोड़ें
outlineElem.AppendChildLast(image);

// रूपरेखा तत्व जोड़ें
outline.AppendChildLast(outlineElem);

// आउटलाइन नोड जोड़ें
page.AppendChildLast(outline);

// पेज नोड जोड़ें
doc.AppendChildLast(page);

// OneNote दस्तावेज़ सहेजें
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

पाठ के साथ दस्तावेज़ बनाने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
Document doc = new Document();

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Page page = new Page(doc);

// आउटलाइन क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Outline outline = new Outline(doc);

// आउटलाइन एलिमेंट क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
OutlineElement outlineElem = new OutlineElement(doc);

// टेक्स्ट स्टाइल क्लास ऑब्जेक्ट प्रारंभ करें और स्वरूपण गुण सेट करें
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// RichText क्लास ऑब्जेक्ट को इनिशियलाइज़ करें और टेक्स्ट स्टाइल लागू करें
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// रिचटेक्स्ट नोड जोड़ें
outlineElem.AppendChildLast(text);

// आउटलाइन एलिमेंट नोड जोड़ें
outline.AppendChildLast(outlineElem);

// आउटलाइन नोड जोड़ें
page.AppendChildLast(outline);

// पेज नोड जोड़ें
doc.AppendChildLast(page);

// OneNote दस्तावेज़ सहेजें
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
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

उपयोगकर्ता परिभाषित कॉलबैक का उपयोग कर सभी संसाधनों (सीएसएस/फोंट/छवियों) को संग्रहीत करने के साथ एचटीएमएल प्रारूप में दस्तावेज़ को कैसे सहेजना दिखाता है।

```csharp
// नीचे दिया गया कोड 'documentFolder' फोल्डर बनाता है जिसमें document.html, 'css' फोल्डर 'style.css' फाइल के साथ, 'इमेज' फोल्डर इमेज के साथ और 'फोंट' फोल्डर फॉन्ट के साथ होता है।
// 'style.css' फ़ाइल में अंत में निम्न स्ट्रिंग होगी "/* यह लाइन उपयोगकर्ता द्वारा मैन्युअल रूप से स्ट्रीम करने के लिए जोड़ी गई है */"
var savingCallbacks = new UserSavingCallbacks()
                          {
                              RootFolder = "documentFolder",
                              CssFolder = "css",
                              KeepCssStreamOpened = true,
                              ImagesFolder = "images",
                              FontsFolder = "fonts"
                          };
var options = new HtmlSaveOptions
              {
                  FontFaceTypes = FontFaceType.Ttf,
                  CssSavingCallback = savingCallbacks,
                  FontSavingCallback = savingCallbacks,
                  ImageSavingCallback = savingCallbacks
              };

if (!Directory.Exists(savingCallbacks.RootFolder))
{
    Directory.CreateDirectory(savingCallbacks.RootFolder);
}

string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

using (var stream = File.Create(Path.Combine(savingCallbacks.RootFolder, "document.html")))
{
    document.Save(stream, options);
}

using (var writer = new StreamWriter(savingCallbacks.CssStream))
{
    writer.WriteLine();
    writer.WriteLine("/* This line is appended to stream manually by user */");
}
```

दिखाता है कि हाइपरलिंक को टेक्स्ट से कैसे बाइंड किया जाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tasks();

// दस्तावेज़ वर्ग का एक ऑब्जेक्ट बनाएँ
Document doc = new Document();

RichText titleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append("Title!");

Outline outline = new Outline()
                      {
                          MaxWidth = 200,
                          MaxHeight = 200,
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };

TextStyle textStyleRed = new TextStyle
                             {
                                 FontColor = Color.Red,
                                 FontName = "Arial",
                                 FontSize = 10,
                             };

TextStyle textStyleHyperlink = new TextStyle
                                   {
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// रूपरेखा तत्व जोड़ें
outline.AppendChildLast(outlineElem);

// टाइटल क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Title title = new Title() { TitleText = titleText };

// पेज क्लास ऑब्जेक्ट को इनिशियलाइज़ करें
Page page = new Note.Page() { Title = title };

// आउटलाइन नोड जोड़ें
page.AppendChildLast(outline);

// पेज नोड जोड़ें
doc.AppendChildLast(page);

// OneNote दस्तावेज़ सहेजें
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

विज़िटर का उपयोग करके किसी दस्तावेज़ की सामग्री तक पहुँचने का तरीका दिखाता है।

```csharp
public static void Run()
{
    // दस्तावेज़ निर्देशिका का पथ।
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // वह दस्तावेज़ खोलें जिसे हम कनवर्ट करना चाहते हैं।
    Document doc = new Document(dataDir + "Aspose.one");

    // एक ऐसी वस्तु बनाएँ जो DocumentVisitor वर्ग से विरासत में मिली हो।
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // यह प्रसिद्ध विज़िटर पैटर्न है। एक आगंतुक को स्वीकार करने के लिए मॉडल प्राप्त करें।
    // संबंधित विधियों को कॉल करके मॉडल स्वयं के माध्यम से पुनरावृति करेगा
    // विज़िटर ऑब्जेक्ट पर (इसे विज़िटिंग कहा जाता है)।
    //
    // ध्यान दें कि ऑब्जेक्ट मॉडल में प्रत्येक नोड में एक्सेप्ट मेथड है इसलिए विजिटिंग
    // न केवल पूरे दस्तावेज़ के लिए, बल्कि दस्तावेज़ में किसी भी नोड के लिए निष्पादित किया जा सकता है।
    doc.Accept(myConverter);

    // एक बार दौरा पूरा हो जाने के बाद, हम ऑपरेशन के परिणाम को पुनः प्राप्त कर सकते हैं,
    // कि इस उदाहरण में, विज़िटर में जमा हो गया है।
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// सादे पाठ प्रारूप में दस्तावेज़ को सहेजने का सरल कार्यान्वयन। एक आगंतुक के रूप में लागू किया गया।
/// </summary>
public class MyOneNoteToTxtWriter : DocumentVisitor
{
    public MyOneNoteToTxtWriter()
    {
        nodecount = 0;
        mIsSkipText = false;
        mBuilder = new StringBuilder();
    }

    /// <summary>
    /// आगंतुक द्वारा जमा किए गए दस्तावेज़ का सादा पाठ प्राप्त करता है।
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// वर्तमान आउटपुट में टेक्स्ट जोड़ता है। सक्षम/अक्षम आउटपुट फ़्लैग का सम्मान करता है।
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// जब दस्तावेज़ में एक RichText नोड का सामना किया जाता है तो कॉल किया जाता है।
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// जब दस्तावेज़ में दस्तावेज़ नोड का सामना किया जाता है तो कॉल किया जाता है।
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// कॉल किया जाता है जब दस्तावेज़ में पृष्ठ नोड का सामना होता है।
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// पेज नोड की प्रोसेसिंग समाप्त होने पर कॉल किया जाता है।
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// जब दस्तावेज़ में शीर्षक नोड का सामना किया जाता है तो कॉल किया जाता है।
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// दस्तावेज़ में एक छवि नोड का सामना करने पर कॉल किया जाता है।
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// कॉल किया जाता है जब दस्तावेज़ में एक OutlineGroup नोड का सामना होता है।
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// कॉल किया जाता है जब दस्तावेज़ में एक रूपरेखा नोड का सामना करना पड़ता है।
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// कॉल किया जाता है जब दस्तावेज़ में एक OutlineElement नोड का सामना होता है।
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// विज़िटर द्वारा नोड्स की कुल संख्या प्राप्त करता है
    /// </summary>
    public Int32 NodeCount
    {
        get { return this.nodecount; }
    }

    private readonly StringBuilder mBuilder;
    private bool mIsSkipText;
    private Int32 nodecount;
}
```

### यह सभी देखें

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* class [Page](../page/)
* interface [INotebookChildNode](../inotebookchildnode/)
* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


