---
title: "الفئة HtmlSaveOptions"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "الفئة Aspose.Note.Saving.HtmlSaveOptions. يسمح بتحديد خيارات إضافية عند حفظ المستند بتنسيق HTML."
type: docs
weight: 780
url: /ar/net/aspose.note.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

يسمح بتحديد خيارات إضافية عند حفظ المستند بتنسيق HTML.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CssPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/cssperpagegeneration/) { get; set; } | يحصل أو يعيّن ما إذا كان سيتم إنشاء ملف StyleSheet لكل صفحة جديدة على حدة. |
| [CssSavingCallback](../../aspose.note.saving/htmlsaveoptions/csssavingcallback/) { get; set; } | يحصل أو يعيّن الدالة الراجعة التي تُستدعى لإنشاء مورد لتخزين CSS. |
| [DocumentPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/documentperpagegeneration/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان توليد مستند لكل صفحة مفعلاً. |
| [ExportCss](../../aspose.note.saving/htmlsaveoptions/exportcss/) { get; set; } | يحصل أو يعيّن طريقة تصدير css. |
| [ExportFonts](../../aspose.note.saving/htmlsaveoptions/exportfonts/) { get; set; } | يحصل أو يعيّن طريقة تصدير الخطوط. |
| [ExportImages](../../aspose.note.saving/htmlsaveoptions/exportimages/) { get; set; } | يحصل أو يعيّن طريقة تصدير الصور. |
| [FontFaceTypes](../../aspose.note.saving/htmlsaveoptions/fontfacetypes/) { get; set; } | يحصل أو يعيّن أنواع خطوط الواجهة. |
| [FontSavingCallback](../../aspose.note.saving/htmlsaveoptions/fontsavingcallback/) { get; set; } | يحصل أو يعيّن الدالة الراجعة التي تُستدعى لإنشاء مورد لتخزين الخط. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | يحصل أو يضبط إعدادات الخط التي سيتم استخدامها أثناء الحفظ |
| [ImageSavingCallback](../../aspose.note.saving/htmlsaveoptions/imagesavingcallback/) { get; set; } | يحصل أو يضبط رد النداء الذي يتم استدعاؤه لإنشاء مورد لتخزين الصورة. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | يحصل أو يضبط عدد الصفحات التي سيتم حفظها. القيمة الافتراضية هي MaxValue مما يعني أنه سيتم عرض جميع صفحات المستند. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | يحصل أو يضبط فهرس الصفحة الأولى التي سيتم حفظها. القيمة الافتراضية هي 0. |
| [PageSavingCallback](../../aspose.note.saving/htmlsaveoptions/pagesavingcallback/) { get; set; } | يحصل أو يضبط رد النداء الذي يتم استدعاؤه لإنشاء مورد لتخزين الصفحة. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | يحصل على الصيغة التي يُحفظ بها المستند. |

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

يوضح كيفية إنشاء مستند وحفظه بتنسيق html لنطاق محدد من الصفحات.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// تهيئة مستند OneNote.
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// النمط الافتراضي لجميع النصوص في المستند.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// حفظ بتنسيق HTML
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
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

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


