---
title: HtmlSaveOptions.ExportFonts
second_title: Aspose.Note .NET API संदर्भ के लिए
description: HtmlSaveOptions संपत्त. फंट नर्यत करने क तरक प्रप्त य सेट करत है
type: docs
weight: 60
url: /hi/net/aspose.note.saving/htmlsaveoptions/exportfonts/
---
## HtmlSaveOptions.ExportFonts property

फोंट निर्यात करने का तरीका प्राप्त या सेट करता है।

```csharp
public ResourceExportType ExportFonts { get; set; }
```

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

### यह सभी देखें

* enum [ResourceExportType](../../../aspose.note.saving.html/resourceexporttype/)
* class [HtmlSaveOptions](../)
* नाम स्थान [Aspose.Note.Saving](../../htmlsaveoptions/)
* सभा [Aspose.Note](../../../)


