---
title: "HtmlSaveOptions.ExportImages"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية HtmlSaveOptions. يحصل أو يضبط طريقة تصدير الصور"
type: docs
weight: 70
url: /ar/net/aspose.note.saving/htmlsaveoptions/exportimages/
---
## HtmlSaveOptions.ExportImages property

يحصل أو يعيّن طريقة تصدير الصور.

```csharp
public ResourceExportType ExportImages { get; set; }
```

## أمثلة

يظهر كيفية حفظ مستند بتنسيق html مع تخزين جميع الموارد (css/خطوط/صور) في ملفات منفصلة.

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

يظهر كيفية حفظ مستند إلى تدفق بتنسيق html مع تضمين جميع الموارد (css/خطوط/صور).

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

### انظر أيضًا

* enum [ResourceExportType](../../../aspose.note.saving.html/resourceexporttype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Note.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Note](../../../)


