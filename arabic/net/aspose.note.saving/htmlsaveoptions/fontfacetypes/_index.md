---
title: "HtmlSaveOptions.FontFaceTypes"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية HtmlSaveOptions. يحصل أو يضبط أنواع خطوط الوجه"
type: docs
weight: 80
url: /ar/net/aspose.note.saving/htmlsaveoptions/fontfacetypes/
---
## HtmlSaveOptions.FontFaceTypes property

يحصل أو يعيّن أنواع خطوط الواجهة.

```csharp
public FontFaceType FontFaceTypes { get; set; }
```

### Property Value

أنواع خطوط الوجه.

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

يظهر كيفية حفظ مستند بتنسيق HTML مع تخزين جميع الموارد (css/خطوط/صور) باستخدام ردود نداء معرفة من قبل المستخدم.

```csharp
// الكود أدناه ينشئ مجلد 'documentFolder' يحتوي على document.html، ومجلد 'css' به ملف 'style.css'، ومجلد 'images' يحتوي على صور، ومجلد 'fonts' يحتوي على خطوط.
// 'style.css' سيحتوي في النهاية على السلسلة التالية "/* This line is appended to stream manually by user */"
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

### انظر أيضًا

* enum [FontFaceType](../../../aspose.note.saving.html/fontfacetype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Note.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Note](../../../)


