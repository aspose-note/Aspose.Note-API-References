---
title: Class HtmlSaveOptions
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Aspose.Note.Saving.HtmlSaveOptions कक्ष. दस्तवेज़ क HTML प्ररूप में सहेजते समय अतरक्त वकल्प नर्दष्ट करने क अनुमत देत है
type: docs
weight: 700
url: /hi/net/aspose.note.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

दस्तावेज़ को HTML प्रारूप में सहेजते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।

```csharp
public class HtmlSaveOptions : SaveOptions
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/)() | डिफ़ॉल्ट कंस्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [CssPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/cssperpagegeneration/) { get; set; } | हो जाता है या सेट करता है कि प्रत्येक नए पृष्ठ के लिए स्टाइलशीट फ़ाइल अलग से उत्पन्न होगी या नहीं। |
| [CssSavingCallback](../../aspose.note.saving/htmlsaveoptions/csssavingcallback/) { get; set; } | उस कॉलबैक को प्राप्त या सेट करता है जिसे CSS को स्टोर करने के लिए संसाधन बनाने के लिए कहा जाता है। |
| [DocumentPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/documentperpagegeneration/) { get; set; } | एक मान प्राप्त या सेट करता है जो इंगित करता है कि दस्तावेज़ प्रति पृष्ठ पीढ़ी सक्षम है या नहीं। |
| [ExportCss](../../aspose.note.saving/htmlsaveoptions/exportcss/) { get; set; } | सीएसएस को निर्यात करने का तरीका प्राप्त या सेट करता है। |
| [ExportFonts](../../aspose.note.saving/htmlsaveoptions/exportfonts/) { get; set; } | फोंट निर्यात करने का तरीका प्राप्त या सेट करता है। |
| [ExportImages](../../aspose.note.saving/htmlsaveoptions/exportimages/) { get; set; } | छवियों को निर्यात करने का तरीका प्राप्त या सेट करता है। |
| [FontFaceTypes](../../aspose.note.saving/htmlsaveoptions/fontfacetypes/) { get; set; } | फॉन्ट फेस टाइप प्राप्त या सेट करता है। |
| [FontSavingCallback](../../aspose.note.saving/htmlsaveoptions/fontsavingcallback/) { get; set; } | उस कॉलबैक को प्राप्त या सेट करता है जिसे फ़ॉन्ट स्टोर करने के लिए संसाधन बनाने के लिए कहा जाता है। |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | को सहेजते समय उपयोग किए जाने वाले फ़ॉन्ट की सेटिंग प्राप्त या सेट करता है |
| [ImageSavingCallback](../../aspose.note.saving/htmlsaveoptions/imagesavingcallback/) { get; set; } | उस कॉलबैक को प्राप्त या सेट करता है जिसे इमेज स्टोर करने के लिए संसाधन बनाने के लिए कहा जाता है। |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | सहेजे जाने वाले पृष्ठों की संख्या प्राप्त करता है या सेट करता है। डिफ़ॉल्ट रूप से हैMaxValue जिसका मतलब है कि दस्तावेज़ के सभी पेज रेंडर किए जाएंगे. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | सहेजे जाने वाले पहले पृष्ठ की अनुक्रमणिका प्राप्त करता है या सेट करता है। डिफ़ॉल्ट रूप से 0. है |
| [PageSavingCallback](../../aspose.note.saving/htmlsaveoptions/pagesavingcallback/) { get; set; } | उस कॉलबैक को प्राप्त या सेट करता है जिसे पेज स्टोर करने के लिए संसाधन बनाने के लिए कहा जाता है। |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | उस प्रारूप को प्राप्त करता है जिसमें दस्तावेज़ सहेजा गया है। |

### उदाहरण

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

### यह सभी देखें

* class [SaveOptions](../saveoptions/)
* नाम स्थान [Aspose.Note.Saving](../../aspose.note.saving/)
* सभा [Aspose.Note](../../)


