---
title: HtmlSaveOptions.ExportFonts
second_title: Aspose.Note لمرجع NET API
description: HtmlSaveOptions ملكية. الحصول على أو تحديد طريقة تصدير الخطوط .
type: docs
weight: 60
url: /ar/net/aspose.note.saving/htmlsaveoptions/exportfonts/
---
## HtmlSaveOptions.ExportFonts property

الحصول على أو تحديد طريقة تصدير الخطوط .

```csharp
public ResourceExportType ExportFonts { get; set; }
```

### أمثلة

يوضح كيفية حفظ مستند بتنسيق html مع تخزين جميع الموارد (css / الخطوط / الصور) في ملفات منفصلة.

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

يوضح كيفية حفظ مستند إلى تدفق بتنسيق html مع تضمين جميع الموارد (css / الخطوط / الصور).

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

### أنظر أيضا

* enum [ResourceExportType](../../../aspose.note.saving.html/resourceexporttype/)
* class [HtmlSaveOptions](../)
* مساحة الاسم [Aspose.Note.Saving](../../htmlsaveoptions/)
* المجسم [Aspose.Note](../../../)


