---
title: "HtmlSaveOptions.FontSavingCallback"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية HtmlSaveOptions. يحصل أو يضبط الـ callback الذي يُستدعى لإنشاء مورد لتخزين الخط"
type: docs
weight: 90
url: /ar/net/aspose.note.saving/htmlsaveoptions/fontsavingcallback/
---
## HtmlSaveOptions.FontSavingCallback property

يحصل أو يعيّن الدالة الراجعة التي تُستدعى لإنشاء مورد لتخزين الخط.

```csharp
public IFontSavingCallback FontSavingCallback { get; set; }
```

## أمثلة

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

* interface [IFontSavingCallback](../../../aspose.note.saving.html/ifontsavingcallback/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Note.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Note](../../../)


