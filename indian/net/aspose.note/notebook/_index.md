---
title: Class Notebook
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.Notebook कक्ष. एक Aspose.Note नटबुक क प्रतनधत्व करत है
type: docs
weight: 410
url: /hi/net/aspose.note/notebook/
---
## Notebook class

एक Aspose.Note नोटबुक का प्रतिनिधित्व करता है।

```csharp
public class Notebook : IEnumerable<INotebookChildNode>, INotebookChildNode
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [Notebook](notebook/#constructor)() | का एक नया उदाहरण प्रारंभ करता है`Notebook` वर्ग. |
| [Notebook](notebook/#constructor_1)(Stream) | का एक नया उदाहरण प्रारंभ करता है`Notebook` class. स्ट्रीम से मौजूदा OneNote नोटबुक खोलता है. |
| [Notebook](notebook/#constructor_3)(string) | का एक नया उदाहरण प्रारंभ करता है`Notebook` class. फ़ाइल से मौजूदा OneNote नोटबुक खोलता है. |
| [Notebook](notebook/#constructor_2)(Stream, NotebookLoadOptions) | का एक नया उदाहरण प्रारंभ करता है`Notebook` class. स्ट्रीम से मौजूदा OneNote नोटबुक खोलता है। अतिरिक्त लोडिंग विकल्प निर्दिष्ट करने की अनुमति देता है। |
| [Notebook](notebook/#constructor_4)(string, NotebookLoadOptions) | का एक नया उदाहरण प्रारंभ करता है`Notebook` class. किसी फ़ाइल से मौजूदा OneNote नोटबुक खोलता है. बच्चों को लोड करने की रणनीति ("आलसी"/तत्काल) जैसे अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Color](../../aspose.note/notebook/color/) { get; set; } | रंग प्राप्त या सेट करता है। |
| [Count](../../aspose.note/notebook/count/) { get; } | में निहित तत्वों की संख्या प्राप्त करता है`Notebook` . |
| [DisplayName](../../aspose.note/notebook/displayname/) { get; set; } | प्रदर्शन नाम प्राप्त या सेट करता है। |
| [FileFormat](../../aspose.note/notebook/fileformat/) { get; } | फ़ाइल स्वरूप प्राप्त करता है (OneNote 2010, OneNote ऑनलाइन)। |
| [Guid](../../aspose.note/notebook/guid/) { get; } | वस्तु की विश्व स्तर पर अद्वितीय आईडी प्राप्त करता है। |
| [IsHistoryEnabled](../../aspose.note/notebook/ishistoryenabled/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो बताता है कि इतिहास सक्षम है या नहीं। |
| [Item](../../aspose.note/notebook/item/) { get; } | दिए गए इंडेक्स द्वारा नोटबुक चाइल्ड नोड प्राप्त करता है। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| [AppendChild](../../aspose.note/notebook/appendchild/)(INotebookChildNode) | सूची के अंत में नोड जोड़ता है। |
| [GetChildNodes&lt;T1&gt;](../../aspose.note/notebook/getchildnodes/)() | नोड प्रकार द्वारा सभी चाइल्ड नोड प्राप्त करें. |
| [GetEnumerator](../../aspose.note/notebook/getenumerator/)() | एक एन्यूमरेटर लौटाता है जो चाइल्ड नोड के माध्यम से पुनरावृति करता है`Notebook` . |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument)(Stream) | चाइल्ड दस्तावेज़ नोड जोड़ता है. स्ट्रीम से मौजूदा OneNote दस्तावेज़ खोलता है. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_2)(string) | चाइल्ड दस्तावेज़ नोड जोड़ता है. फ़ाइल से मौजूदा OneNote दस्तावेज़ खोलता है. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_1)(Stream, LoadOptions) | चाइल्ड दस्तावेज़ नोड जोड़ता है. स्ट्रीम से मौजूदा OneNote दस्तावेज़ खोलता है. अतिरिक्त लोड विकल्प निर्दिष्ट करने की अनुमति देता है। |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_3)(string, LoadOptions) | चाइल्ड दस्तावेज़ नोड जोड़ता है. फ़ाइल से मौजूदा OneNote दस्तावेज़ खोलता है. अतिरिक्त लोड विकल्प निर्दिष्ट करने की अनुमति देता है। |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook)(Stream) | चाइल्ड नोटबुक नोड जोड़ता है. स्ट्रीम से मौजूदा OneNote नोटबुक खोलता है. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_2)(string) | चाइल्ड नोटबुक नोड जोड़ता है. फ़ाइल से मौजूदा OneNote नोटबुक खोलता है. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_1)(Stream, NotebookLoadOptions) | चाइल्ड नोटबुक नोड जोड़ता है. स्ट्रीम से मौजूदा OneNote नोटबुक खोलता है. अतिरिक्त लोड विकल्प निर्दिष्ट करने की अनुमति देता है। |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_3)(string, NotebookLoadOptions) | चाइल्ड नोटबुक नोड जोड़ता है. फ़ाइल से मौजूदा OneNote नोटबुक खोलता है. अतिरिक्त लोड विकल्प निर्दिष्ट करने की अनुमति देता है। |
| [RemoveChild](../../aspose.note/notebook/removechild/)(INotebookChildNode) | चाइल्ड नोड निकालता है. |
| [Save](../../aspose.note/notebook/save/#save)(Stream) | OneNote दस्तावेज़ को स्ट्रीम में सहेजता है. |
| [Save](../../aspose.note/notebook/save/#save_3)(string) | OneNote दस्तावेज़ को फ़ाइल में सहेजता है. |
| [Save](../../aspose.note/notebook/save/#save_2)(Stream, NotebookSaveOptions) | निर्दिष्ट सहेजें विकल्पों का उपयोग करके OneNote दस्तावेज़ को स्ट्रीम में सहेजता है. |
| [Save](../../aspose.note/notebook/save/#save_1)(Stream, SaveFormat) | निर्दिष्ट प्रारूप में एक स्ट्रीम में OneNote दस्तावेज़ सहेजता है। |
| [Save](../../aspose.note/notebook/save/#save_5)(string, NotebookSaveOptions) | निर्दिष्ट सहेजें विकल्पों का उपयोग करके OneNote दस्तावेज़ को फ़ाइल में सहेजता है. |
| [Save](../../aspose.note/notebook/save/#save_4)(string, SaveFormat) | OneNote दस्तावेज़ को निर्दिष्ट स्वरूप में फ़ाइल में सहेजता है. |

### उदाहरण

दिखाता है कि नोटबुक को कैसे सहेजना है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook();

dataDir = dataDir + "test_out.onetoc2";

// नोटबुक को सेव करें
notebook.Save(dataDir);
```

पीडीएफ प्रारूप में नोटबुक को बचाने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();

// एक OneNote नोटबुक लोड करें
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToPDF_out.pdf";

// नोटबुक को सेव करें
notebook.Save(dataDir);
```

नोटबुक को छवि के रूप में सहेजने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();

// एक OneNote नोटबुक लोड करें
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToImage_out.png";

// नोटबुक को सेव करें
notebook.Save(dataDir);
```

दिखाता है कि नोटबुक से सभी पाठ कैसे प्राप्त करें।

```csharp
string inputFile = "notebook.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

Notebook rootNotebook = new Notebook(dataDir + inputFile);

IList<RichText> allRichTextNodes = rootNotebook.GetChildNodes<RichText>();
foreach (RichText richTextNode in allRichTextNodes)
{
    Console.WriteLine(richTextNode.Text);
}
```

चपटा नोटबुक को पीडीएफ प्रारूप में सहेजने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();

// एक OneNote नोटबुक लोड करें
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// नोटबुक को सेव करें
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

आलसी तरीके से लोड हो रहे नोटबुक के दस्तावेज़ों के माध्यम से पुनरावृति करने का तरीका दिखाता है।

```csharp
string inputFile = "Notizbuch öffnen.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

// डिफ़ॉल्ट रूप से बच्चे लोड करना "आलसी" है।
Notebook notebook = new Notebook(dataDir + inputFile);

foreach (var notebookChildNode in notebook.OfType<Document>()) 
{
    // चाइल्ड डॉक्यूमेंट की वास्तविक लोडिंग केवल यहीं होती है।
    // चाइल्ड डॉक्यूमेंट के साथ कुछ करें
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

दिखाता है कि स्ट्रीम से नोटबुक कैसे लोड करें।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

एक एन्क्रिप्टेड नोटबुक को कैसे दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

निर्दिष्ट विकल्पों के साथ नोटबुक को छवि के रूप में सहेजने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();

// एक OneNote नोटबुक लोड करें
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// नोटबुक को सेव करें
notebook.Save(dataDir, notebookSaveOptions);
```

छवि के रूप में चपटी नोटबुक को सहेजने का तरीका दिखाता है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();

// एक OneNote नोटबुक लोड करें
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// नोटबुक को सेव करें
notebook.Save(dataDir, notebookSaveOptions);
```

दिखाता है कि किसी नोटबुक से किसी अनुभाग को कैसे निकालना है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();

// एक OneNote नोटबुक लोड करें
var notebook = new Notebook(dataDir + "test.onetoc2");

// वांछित चाइल्ड आइटम को खोजने के लिए उसके चाइल्ड नोड के माध्यम से ट्रैवर्स करें
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // चाइल्ड आइटम को नोटबुक से निकालें
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// नोटबुक को सेव करें
notebook.Save(dataDir);
```

दिखाता है कि किसी नोटबुक के पहले से लोड किए गए दस्तावेज़ों के माध्यम से पुनरावृति कैसे करें।

```csharp
// डिफ़ॉल्ट रूप से बच्चे लोड करना "आलसी" है।
// इसलिए तत्काल लोडिंग हुई है,
// NotebookLoadOptions.InstantLoading फ़्लैग सेट करना आवश्यक है।
NotebookLoadOptions loadOptions = new NotebookLoadOptions { InstantLoading = true };

String inputFile = "Notizbuch öffnen.onetoc2";
String dataDir = RunExamples.GetDataDir_NoteBook();
Notebook notebook = new Notebook(dataDir + inputFile, loadOptions);

// सभी बाल दस्तावेज़ पहले ही लोड हो चुके हैं।
foreach (INotebookChildNode notebookChildNode in notebook.OfType<Document>()) 
{
   // चाइल्ड डॉक्यूमेंट के साथ कुछ करें
}
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

### यह सभी देखें

* interface [INotebookChildNode](../inotebookchildnode/)
* नाम स्थान [Aspose.Note](../../aspose.note/)
* सभा [Aspose.Note](../../)


