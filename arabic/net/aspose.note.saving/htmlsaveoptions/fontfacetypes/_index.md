---
title: HtmlSaveOptions.FontFaceTypes
second_title: Aspose.Note لمرجع NET API
description: HtmlSaveOptions ملكية. الحصول على أنواع وجه الخط أو تعيينها.
type: docs
weight: 80
url: /ar/net/aspose.note.saving/htmlsaveoptions/fontfacetypes/
---
## HtmlSaveOptions.FontFaceTypes property

الحصول على أنواع وجه الخط أو تعيينها.

```csharp
public FontFaceType FontFaceTypes { get; set; }
```

### Property_Value

أنواع وجه الخط .

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

يوضح كيفية حفظ مستند بتنسيق html مع تخزين جميع الموارد (css / الخطوط / الصور) باستخدام عمليات الاسترجاعات المعرفة من قبل المستخدم.

```csharp
// ينشئ الكود أدناه مجلد "documentFolder" يحتوي على document.html ومجلد "css" بملف "style.css" ومجلد "images" مع صور ومجلد "خطوط" يحتوي على خطوط.
// سيحتوي ملف "style.css" في نهاية السلسلة التالية "/ * هذا السطر مُلحق بالبث يدويًا بواسطة المستخدم * /"
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

### أنظر أيضا

* enum [FontFaceType](../../../aspose.note.saving.html/fontfacetype/)
* class [HtmlSaveOptions](../)
* مساحة الاسم [Aspose.Note.Saving](../../htmlsaveoptions/)
* المجسم [Aspose.Note](../../../)


