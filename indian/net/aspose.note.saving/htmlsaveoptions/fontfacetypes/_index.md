---
title: HtmlSaveOptions.FontFaceTypes
second_title: Aspose.Note .NET API संदर्भ के लिए
description: HtmlSaveOptions संपत्त. फन्ट फेस टइप प्रप्त य सेट करत है
type: docs
weight: 80
url: /hi/net/aspose.note.saving/htmlsaveoptions/fontfacetypes/
---
## HtmlSaveOptions.FontFaceTypes property

फॉन्ट फेस टाइप प्राप्त या सेट करता है।

```csharp
public FontFaceType FontFaceTypes { get; set; }
```

### संपत्ति मूल्य

फॉन्ट फेस प्रकार।

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

* enum [FontFaceType](../../../aspose.note.saving.html/fontfacetype/)
* class [HtmlSaveOptions](../)
* नाम स्थान [Aspose.Note.Saving](../../htmlsaveoptions/)
* सभा [Aspose.Note](../../../)


