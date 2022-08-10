---
title: HtmlSaveOptions
second_title: Aspose.Note لمرجع NET API
description: يسمح بتحديد خيارات إضافية عند حفظ المستند بتنسيق HTML .
type: docs
weight: 680
url: /ar/net/aspose.note.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

يسمح بتحديد خيارات إضافية عند حفظ المستند بتنسيق HTML .

```csharp
public class HtmlSaveOptions : SaveOptions
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions)() | Default_Constructor |

## الخصائص

| اسم | وصف |
| --- | --- |
| [CssPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/cssperpagegeneration) { get; set; } | يحصل أو يحدد ما إذا كان سيتم إنشاء ملف StyleSheet لكل صفحة جديدة على حدة. |
| [CssSavingCallback](../../aspose.note.saving/htmlsaveoptions/csssavingcallback) { get; set; } | الحصول على أو تعيين رد الاتصال المطلوب لإنشاء مورد لتخزين CSS. |
| [DocumentPerPageGeneration](../../aspose.note.saving/htmlsaveoptions/documentperpagegeneration) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان إنشاء مستند لكل صفحة ممكّنًا . |
| [ExportCss](../../aspose.note.saving/htmlsaveoptions/exportcss) { get; set; } | الحصول على طريقة تصدير css أو تعيينها. |
| [ExportFonts](../../aspose.note.saving/htmlsaveoptions/exportfonts) { get; set; } | الحصول على أو تحديد طريقة تصدير الخطوط . |
| [ExportImages](../../aspose.note.saving/htmlsaveoptions/exportimages) { get; set; } | الحصول على أو تحديد الطريقة التي يتم بها تصدير الصور. |
| [FontFaceTypes](../../aspose.note.saving/htmlsaveoptions/fontfacetypes) { get; set; } | الحصول على أنواع وجه الخط أو تعيينها. |
| [FontSavingCallback](../../aspose.note.saving/htmlsaveoptions/fontsavingcallback) { get; set; } | الحصول على أو تعيين رد الاتصال المطلوب لإنشاء مورد لتخزين الخط. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem) { get; set; } | الحصول على أو تعيين إعدادات الخط لاستخدامها أثناء الحفظ |
| [ImageSavingCallback](../../aspose.note.saving/htmlsaveoptions/imagesavingcallback) { get; set; } | الحصول على أو تعيين رد الاتصال المطلوب لإنشاء مورد لتخزين الصورة. |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount) { get; set; } | الحصول على أو تحديد عدد الصفحات المراد حفظها. افتراضيا هوMaxValue مما يعني أنه سيتم تقديم جميع صفحات المستند. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex) { get; set; } | الحصول على أو تحديد فهرس الصفحة الأولى للحفظ. بشكل افتراضي هو 0. |
| [PageSavingCallback](../../aspose.note.saving/htmlsaveoptions/pagesavingcallback) { get; set; } | الحصول على أو تعيين رد الاتصال المطلوب لإنشاء مورد لتخزين الصفحة. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat) { get; } | يحصل على التنسيق الذي تم حفظ المستند به. |

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

يوضح كيفية إنشاء مستند وحفظه بتنسيق html في نطاق محدد من الصفحات.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// تهيئة مستند OneNote
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// النمط الافتراضي لكل النص في المستند.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// حفظ في تنسيق HTML
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
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

* class [SaveOptions](../saveoptions)
* مساحة الاسم [Aspose.Note.Saving](../../aspose.note.saving)
* المجسم [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
