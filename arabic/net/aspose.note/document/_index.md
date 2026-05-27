---
title: "الفئة Document"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "الفئة Aspose.Note.Document. تمثل مستند Aspose.Note"
type: docs
weight: 60
url: /ar/net/aspose.note/document/
---
## Document class

يمثل مستند Aspose.Note.

```csharp
public class Document : CompositeNode<Page>, INotebookChildNode
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [Document](document/#constructor)() | يُنشئ مثيلًا جديدًا للفئة `Document`. ينشئ مستند OneNote فارغًا. |
| [Document](document/#constructor_1)(Stream) | يُنشئ مثيلًا جديدًا للفئة `Document`. يفتح مستند OneNote موجود من تدفق. |
| [Document](document/#constructor_3)(string) | يُنشئ مثيلًا جديدًا للفئة `Document`. يفتح مستند OneNote موجود من ملف. |
| [Document](document/#constructor_2)(Stream, LoadOptions) | يُنشئ مثيلًا جديدًا للفئة `Document`. يفتح مستند OneNote موجود من تدفق. يسمح بتحديد خيارات إضافية مثل كلمة مرور التشفير. |
| [Document](document/#constructor_4)(string, LoadOptions) | يُنشئ مثيلًا جديدًا للفئة `Document`. يفتح مستند OneNote موجود من ملف. يسمح بتحديد خيارات إضافية مثل كلمة مرور التشفير. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AutomaticLayoutChangesDetectionEnabled](../../aspose.note/document/automaticlayoutchangesdetectionenabled/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان Aspose.Note يقوم باكتشاف تغييرات التخطيط تلقائيًا. القيمة الافتراضية هي `true`. |
| [Color](../../aspose.note/document/color/) { get; set; } | يحصل أو يعيّن اللون. |
| [CreationTime](../../aspose.note/document/creationtime/) { get; set; } | يحصل أو يعيّن وقت الإنشاء. |
| [DisplayName](../../aspose.note/document/displayname/) { get; set; } | يحصل أو يضبط اسم العرض. |
| [Document](../../aspose.note/node/document/) { get; } | يحصل على مستند العقدة. |
| [FileFormat](../../aspose.note/document/fileformat/) { get; } | يحصل على تنسيق الملف (OneNote 2010، OneNote Online). |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [Guid](../../aspose.note/document/guid/) { get; } | يحصل على المعرف الفريد عالميًا للكائن. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | يحصل على العقدة التالية في نفس مستوى شجرة العقد. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | يحصل على نوع العقدة. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | يحصل على العقدة الأصلية. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | يحصل على العقدة السابقة في نفس مستوى شجرة العقد. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Accept](../../aspose.note/document/accept/)(DocumentVisitor) | يقبل زائر العقدة. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| [DetectLayoutChanges](../../aspose.note/document/detectlayoutchanges/)() | يكتشف جميع التغييرات التي تم إجراؤها على تخطيط المستند منذ الاستدعاء السابق لـ [`DetectLayoutChanges`](./detectlayoutchanges/). في حال تم تعيين [`AutomaticLayoutChangesDetectionEnabled`](./automaticlayoutchangesdetectionenabled/) إلى true، يتم استخدامها تلقائيًا في بداية تصدير المستند. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| [GetPageHistory](../../aspose.note/document/getpagehistory/)(Page) | يحصل على [`PageHistory`](../pagehistory/) التي تحتوي على السجل الكامل لكل صفحة موجودة في المستند (الأقدم في الفهرس 0). يمكن الوصول إلى نسخة الصفحة الحالية عبر [`Current`](../pagehistory/current/) وتُحتفظ بها بشكل منفصل عن مجموعة الإصدارات التاريخية. |
| [Import](../../aspose.note/document/import/#import)(Stream, HtmlImportOptions, MergeOptions) | يستورد مجموعة من الصفحات من مستند HTML المقدم. |
| [Import](../../aspose.note/document/import/#import_1)(Stream, PdfImportOptions, MergeOptions) | يستورد مجموعة من الصفحات من مستند PDF المقدم. |
| [Import](../../aspose.note/document/import/#import_2)(string, HtmlImportOptions, MergeOptions) | يستورد مجموعة من الصفحات من مستند HTML المقدم. |
| [Import](../../aspose.note/document/import/#import_3)(string, PdfImportOptions, MergeOptions) | يستورد مجموعة من الصفحات من مستند PDF المقدم. |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;Page&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params Page[]) |  |
| [Merge](../../aspose.note/document/merge/)(IEnumerable&lt;Page&gt;, MergeOptions) | يدمج مجموعة من الصفحات إلى المستند. |
| [Print](../../aspose.note/document/print/#print)() | يطبع المستند باستخدام الطابعة الافتراضية. |
| [Print](../../aspose.note/document/print/#print_1)(PrintOptions) | يطبع المستند باستخدام الطابعة الافتراضية. |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |
| [Save](../../aspose.note/document/save/#save)(Stream) | يحفظ مستند OneNote إلى تدفق. |
| [Save](../../aspose.note/document/save/#save_3)(string) | يحفظ مستند OneNote إلى ملف. |
| [Save](../../aspose.note/document/save/#save_1)(Stream, SaveFormat) | يحفظ مستند OneNote إلى تدفق بالتنسيق المحدد. |
| [Save](../../aspose.note/document/save/#save_2)(Stream, SaveOptions) | يحفظ مستند OneNote إلى تدفق باستخدام خيارات الحفظ المحددة. |
| [Save](../../aspose.note/document/save/#save_4)(string, SaveFormat) | يحفظ مستند OneNote إلى ملف بالتنسيق المحدد. |
| [Save](../../aspose.note/document/save/#save_5)(string, SaveOptions) | يحفظ مستند OneNote إلى ملف باستخدام خيارات الحفظ المحددة. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted)(Stream, out Document) | يتحقق مما إذا كان المستند من تدفق مشفرًا. للتحقق من ذلك نحتاج إلى تحميل هذا المستند بالكامل. لذا قد يؤدي هذا الأسلوب إلى عقوبة في الأداء. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_3)(string, out Document) | يتحقق مما إذا كان المستند من ملف مشفرًا. للتحقق من ذلك نحتاج إلى تحميل هذا المستند بالكامل. لذا قد يؤدي هذا الأسلوب إلى عقوبة في الأداء. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_1)(Stream, LoadOptions, out Document) | يتحقق مما إذا كان المستند من تدفق مشفرًا. للتحقق من ذلك نحتاج إلى تحميل هذا المستند بالكامل. لذا قد يؤدي هذا الأسلوب إلى عقوبة في الأداء. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_2)(Stream, string, out Document) | يتحقق مما إذا كان المستند من تدفق مشفرًا. للتحقق من ذلك نحتاج إلى تحميل هذا المستند بالكامل. لذا قد يؤدي هذا الأسلوب إلى عقوبة في الأداء. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_4)(string, LoadOptions, out Document) | يتحقق مما إذا كان المستند من ملف مشفرًا. للتحقق من ذلك نحتاج إلى تحميل هذا المستند بالكامل. لذا قد يؤدي هذا الأسلوب إلى عقوبة في الأداء. |
| static [IsEncrypted](../../aspose.note/document/isencrypted/#isencrypted_5)(string, string, out Document) | يتحقق مما إذا كان المستند من ملف مشفرًا. للتحقق من ذلك نحتاج إلى تحميل هذا المستند بالكامل. لذا قد يؤدي هذا الأسلوب إلى عقوبة في الأداء. |

## أمثلة

يوضح كيفية إرسال المستند إلى طابعة باستخدام مربع حوار Windows القياسي مع الخيارات الافتراضية.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

document.Print();
```

يوضح كيفية حفظ مستند.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

يعرض كيفية التعامل مع مستند مشفر.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

يعرض كيفية حفظ المستند مع التشفير.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

يعرض كيفية حفظ مستند باستخدام تعداد SaveFormat.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

يعرض كيفية حفظ مستند باستخدام OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

يعرض كيفية الحصول على عدد صفحات المستند.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// احصل على عدد الصفحات
int count = oneFile.Count();

// اطبع العدد على شاشة الإخراج
Console.WriteLine(count);
```

يعرض كيفية حفظ مستند بتنسيق pdf باستخدام الإعدادات الافتراضية.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// احفظ المستند كملف PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

يعرض كيفية حفظ مستند بتنسيق gif.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// احفظ المستند كـ gif.
oneFile.Save(dataDir, SaveFormat.Gif);
```

يعرض كيفية ضبط جودة الصورة عند حفظ المستند كصورة بتنسيق JPEG.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// احفظ المستند.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

يعرض كيفية ضبط دقة الصورة عند حفظ المستند كصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// احفظ المستند.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

يعرض كيفية ربط ارتباط تشعبي بصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page();

var image = new Image(dataDir + "image.jpg") { HyperlinkUrl = "https://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

يعرض كيفية الحصول على تنسيق الملف للمستند.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // معالجة OneNote 2010
        break;
    case FileFormat.OneNoteOnline:
        // معالجة OneNote Online
        break;
}
```

يعرض كيفية حفظ مستند إلى تدفق.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// أعد موضع التدفق إلى الصفر لتكون جاهزة للقارئ التالي.
dstStream.Seek(0, SeekOrigin.Begin);
```

يعرض كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

يوضح كيفية إضافة قسم جديد إلى الدفتر.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر OneNote
var notebook = new Notebook(dataDir + "Notebook.onetoc2");

// إلحاق عنصر فرعي جديد إلى الدفتر
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// احفظ الدفتر
notebook.Save(dataDir);
```

يعرض كيفية التحقق مما إذا فشل تحميل المستند لأن تنسيق OneNote 2007 غير مدعوم.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "OneNote2007.one");

try
{
    new Document(fileName);
}
catch (UnsupportedFileFormatException e)
{
    if (e.FileFormat == FileFormat.OneNote2007)
    {
        Console.WriteLine("It looks like the provided file is in OneNote 2007 format that is not supported.");
    }
    else
        throw;
}
```

يعرض كيفية استعادة النسخة السابقة لصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// تحميل مستند OneNote والحصول على العنصر الفرعي الأول.
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

يعرض كيفية استنساخ صفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// تحميل مستند OneNote.
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// استنساخ إلى مستند جديد بدون تاريخ
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// استنساخ إلى مستند جديد مع التاريخ
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

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

يظهر كيفية تعيين وصف نصي لصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page();
var image = new Image(dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

يظهر كيفية الحصول على معلومات ميتا حول صفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

foreach (Page page in oneFile)
{
    Console.WriteLine("LastModifiedTime: {0}", page.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", page.CreationTime);
    Console.WriteLine("Title: {0}", page.Title);
    Console.WriteLine("Level: {0}", page.Level);
    Console.WriteLine("Author: {0}", page.Author);
    Console.WriteLine();
}
```

عند حفظ صفحات OneNote الطويلة بتنسيق pdf يتم تقسيمها عبر صفحات. يوضح المثال كيفية تكوين منطق التقسيم للكائنات الموجودة على فواصل الصفحات.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// أو
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

يظهر كيفية حفظ مستند بتنسيق png.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// تهيئة كائن ImageSaveOptions 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // تعيين فهرس الصفحة
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// حفظ المستند كـ PNG.
oneFile.Save(dataDir, opts);
```

يوضح كيفية تعديل تاريخ الصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// تحميل مستند OneNote والحصول على العنصر الفرعي الأول.
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page();
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page());

    pageHistory.Insert(1, new Page());

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
```

يظهر كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور محددة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

يظهر كيفية تطبيق نمط السمة الداكنة على مستند.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Text();

// حمّل المستند إلى Aspose.Note.
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
```

يوضح كيفية المرور عبر محتوى الدفتر.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = "Open Notebook.onetoc2";
try
{
    var notebook = new Notebook(dataDir + fileName);
    foreach (var notebookChildNode in notebook)
    {
        Console.WriteLine(notebookChildNode.DisplayName);
        if (notebookChildNode is Document)
        {
            // قم بعمل شيء مع المستند الفرعي
        }
        else if (notebookChildNode is Notebook)
        {
            // قم بعمل شيء مع دفتر فرعي
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

يظهر كيفية الحصول على صورة من مستند.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// الحصول على جميع عقد Image
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // حفظ بايتات الصورة إلى ملف
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

يظهر كيفية حفظ مستند بتنسيق pdf.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// تهيئة كائن PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // تعيين فهرس الصفحة الأولى التي سيتم حفظها
                              PageIndex = 0,

                              // تعيين عدد الصفحات
                              PageCount = 1,
                          };

// احفظ المستند كملف PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

يظهر كيفية حفظ مستند بتنسيق pdf باستخدام إعدادات محددة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// تهيئة كائن PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // استخدام ضغط Jpeg
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // جودة ضغط JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

يظهر كيفية إرسال المستند إلى طابعة باستخدام مربع حوار Windows القياسي مع الخيارات المحددة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
               {
                   PrinterSettings = printerSettings,
                   Resolution = 1200,
                   PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
                   DocumentName = "Test.one"
               });
```

يظهر كيفية الحصول على محتوى ملف مرفق.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Attachments();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// احصل على قائمة بعقد الملفات المرفقة
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// تكرار عبر جميع العقد
foreach (AttachedFile file in nodes)
{
    // تحميل الملف المرفق إلى كائن تدفق
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // إنشاء ملف محلي
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // نسخ تدفق الملف
            CopyStream(outputStream, fileStream);
        }
    }
}
```

يظهر كيفية الحصول على معلومات ميتا للصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// الحصول على جميع عقد Image
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

يظهر كيفية الحصول على تاريخ الصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// تحميل مستند OneNote.
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// احصل على الصفحة الأولى
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

يظهر كيفية إضافة ملف إلى مستند باستخدام مسار الملف.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Attachments();

// إنشاء كائن من فئة Document
Document doc = new Document();

// تهيئة كائن فئة Page
Page page = new Page();

// تهيئة كائن فئة Outline
Outline outline = new Outline();

// تهيئة كائن فئة OutlineElement
OutlineElement outlineElem = new OutlineElement();

// تهيئة كائن فئة AttachedFile
AttachedFile attachedFile = new AttachedFile(dataDir + "attachment.txt");

// إضافة ملف مرفق
outlineElem.AppendChildLast(attachedFile);

// إضافة عقدة عنصر المخطط
outline.AppendChildLast(outlineElem);

// إضافة عقدة المخطط
page.AppendChildLast(outline);

// إضافة عقدة صفحة
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

يوضح كيفية إنشاء مستند وحفظه بتنسيق html باستخدام الخيارات الافتراضية.

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
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

يعرض كيفية التحقق مما إذا كانت الصفحة صفحة تعارض (أي أنها تحتوي على تغييرات لم يتمكن OneNote من دمجها تلقائيًا).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// تحميل مستند OneNote.
Document doc = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

var history = doc.GetPageHistory(doc.FirstChild);
for (int i = 0; i < history.Count; i++)
{
    var historyPage = history[i];
    Console.Write("    {0}. Author: {1}, {2:dd.MM.yyyy hh.mm.ss}",
                    i,
                    historyPage.PageContentRevisionSummary.AuthorMostRecent,
                    historyPage.PageContentRevisionSummary.LastModifiedTime);
    Console.WriteLine(historyPage.IsConflictPage ? ", IsConflict: true" : string.Empty);

    // بشكل افتراضي، يتم تخطي صفحات التعارض عند الحفظ.
    // إذا تم وضع علامة بأنها غير متعارضة، فسيتم حفظها كصفحة عادية في السجل.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

يظهر كيفية إضافة صورة من ملف إلى مستند مع خصائص محددة من قبل المستخدم.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

// تحميل المستند من الدفق.
Document doc = new Document(dataDir + "Aspose.one");

// احصل على الصفحة الأولى من المستند.
Page page = doc.FirstChild;

// تحميل صورة من الملف.
Image image = new Image(dataDir + "image.jpg")
                          {
                              // غيّر حجم الصورة وفقًا لاحتياجاتك (اختياري).
                              Width = 100,
                              Height = 100,

                              // حدد موقع الصورة في الصفحة (اختياري).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // ضبط محاذاة الصورة
                              Alignment = HorizontalAlignment.Right
                          };

// أضف الصورة إلى الصفحة.
page.AppendChildLast(image);
```

يظهر كيفية إضافة ملف من تدفق إلى مستند.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Attachments();

// إنشاء كائن من فئة Document
Document doc = new Document();

// تهيئة كائن فئة Page
Page page = new Page();

// تهيئة كائن فئة Outline
Outline outline = new Outline();

// تهيئة كائن فئة OutlineElement
OutlineElement outlineElem = new OutlineElement();

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // تهيئة كائن فئة AttachedFile وتمرير مسار أيقونته أيضًا
    AttachedFile attachedFile = new AttachedFile(dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // إضافة ملف مرفق
    outlineElem.AppendChildLast(attachedFile);
}

// إضافة عقدة عنصر المخطط
outline.AppendChildLast(outlineElem);

// إضافة عقدة المخطط
page.AppendChildLast(outline);

// إضافة عقدة صفحة
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

يظهر كيفية إضافة صورة من الدفق إلى مستند.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

// إنشاء كائن من فئة Document
Document doc = new Document();

// تهيئة كائن فئة Page
Page page = new Page();

Outline outline1 = new Outline();
OutlineElement outlineElem1 = new OutlineElement();

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // تحميل الصورة الثانية باستخدام اسم الصورة، الامتداد، والدفق.
    Image image1 = new Image("Penguins.jpg", fs)
                                   {
                                       // ضبط محاذاة الصورة
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// حفظ مستند OneNote.
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

يوضح كيفية إنشاء مستند بصفحة معنونة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// إنشاء كائن من فئة Document
Document doc = new Document();

// تهيئة كائن فئة Page
Page page = new Page();

// النمط الافتراضي لجميع النصوص في المستند.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// تعيين خصائص عنوان الصفحة
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// إلحاق عقدة Page في المستند
doc.AppendChildLast(page);

// حفظ مستند OneNote.
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

عند حفظ صفحات OneNote الطويلة بتنسيق PDF يتم تقسيمها عبر صفحات متعددة. يوضح المثال كيفية تكوين منطق التقسيم للكائنات الموجودة على فواصل الصفحات.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// حمّل المستند إلى Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// أو
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// أو
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// أو
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// أو
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

يظهر كيفية إضافة صورة من ملف إلى مستند.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

// إنشاء كائن من فئة Document
Document doc = new Document();

// تهيئة كائن فئة Page
Page page = new Page();

// تهيئة كائن فئة Outline وتعيين خصائص الإزاحة
Outline outline = new Outline();

// تهيئة كائن فئة OutlineElement
OutlineElement outlineElem = new OutlineElement();

// تحميل صورة عبر مسار الملف.
Image image = new Image(dataDir + "image.jpg")
                          {
                              // ضبط محاذاة الصورة
                              Alignment = HorizontalAlignment.Right
                          };

// إضافة صورة
outlineElem.AppendChildLast(image);

// إضافة عناصر المخطط
outline.AppendChildLast(outlineElem);

// إضافة عقدة المخطط
page.AppendChildLast(outline);

// إضافة عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote.
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
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

يظهر كيفية إنشاء مستند بنص.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// إنشاء كائن من فئة Document
Document doc = new Document();

// تهيئة كائن فئة Page
Page page = new Page();

// تهيئة كائن فئة Outline
Outline outline = new Outline();

// تهيئة كائن فئة OutlineElement
OutlineElement outlineElem = new OutlineElement();

// تهيئة كائن الفئة TextStyle وتعيين خصائص التنسيق
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// تهيئة كائن الفئة RichText وتطبيق نمط النص
RichText text = new RichText() { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// إضافة عقدة RichText
outlineElem.AppendChildLast(text);

// إضافة عقدة OutlineElement
outline.AppendChildLast(outlineElem);

// إضافة عقدة المخطط
page.AppendChildLast(outline);

// إضافة عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote.
dataDir = dataDir + "CreateDocWithSimpleRichText_out.one";
doc.Save(dataDir);
```

يوضح كيفية حفظ مستند بتنسيقات مختلفة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// تهيئة المستند الجديد
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// تهيئة الصفحة الجديدة
Page page = new Page();

// النمط الافتراضي لجميع النصوص في المستند.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// إلحاق عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote بصيغ مختلفة، ضبط حجم خط النص واكتشاف تغييرات التخطيط يدويًا.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
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

يظهر كيفية ربط ارتباط تشعبي بنص.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tasks();

// إنشاء كائن من فئة Document
Document doc = new Document();

RichText titleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append("Title!");

Outline outline = new Outline()
                      {
                          MaxWidth = 200,
                          MaxHeight = 200,
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };

TextStyle textStyleRed = new TextStyle
                             {
                                 FontColor = Color.Red,
                                 FontName = "Arial",
                                 FontSize = 10,
                             };

TextStyle textStyleHyperlink = new TextStyle
                                   {
                                       HyperlinkAddress = "https://www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// إضافة عناصر المخطط
outline.AppendChildLast(outlineElem);

// تهيئة كائن فئة Title
Title title = new Title() { TitleText = titleText };

// تهيئة كائن فئة Page
Page page = new Note.Page() { Title = title };

// إضافة عقدة المخطط
page.AppendChildLast(outline);

// إضافة عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote.
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

يعرض كيفية الوصول إلى محتوى مستند باستخدام الزائر.

```csharp
public static void Run()
{
    // المسار إلى دليل المستندات.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // افتح المستند الذي نريد تحويله.
    Document doc = new Document(dataDir + "Aspose.one");

    // أنشئ كائنًا يرث من الفئة DocumentVisitor.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // هذا هو نمط الزائر المعروف. اجعل النموذج يقبل زائرًا.
    // سيقوم النموذج بالتكرار على نفسه عن طريق استدعاء الطرق المقابلة
    // على كائن الزائر (يُطلق على ذلك زيارة).
    //
    // لاحظ أن كل عقدة في نموذج الكائن لديها طريقة Accept بحيث يمكن للزيارة
    // يمكن تنفيذها ليس فقط للمستند بالكامل، بل لأي عقدة في المستند.
    doc.Accept(myConverter);

    // بمجرد اكتمال الزيارة، يمكننا استرجاع نتيجة العملية،
    // التي في هذا المثال، تم تجميعها في الزائر.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// تنفيذ بسيط لحفظ مستند بتنسيق النص العادي. تم تنفيذها كزائر.
/// </summary>
public class MyOneNoteToTxtWriter : DocumentVisitor
{
    public MyOneNoteToTxtWriter()
    {
        nodecount = 0;
        mIsSkipText = false;
        mBuilder = new StringBuilder();
    }

    /// <summary>
    /// يحصل على النص العادي للمستند الذي تم تجميعه بواسطة الزائر.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// يضيف نصًا إلى الإخراج الحالي. يراعي علامة الإخراج المفعلة/المعطلة.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// يُستدعى عندما يتم العثور على عقدة RichText في المستند.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// يُستدعى عندما يتم العثور على عقدة Document في المستند.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// يُستدعى عندما يتم العثور على عقدة Page في المستند.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// يُستدعى عند انتهاء معالجة عقدة Page.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// يُستدعى عندما يتم العثور على عقدة Title في المستند.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// يُستدعى عندما يتم العثور على عقدة Image في المستند.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// يُستدعى عندما يتم العثور على عقدة OutlineGroup في المستند.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// يُستدعى عندما يتم العثور على عقدة Outline في المستند.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// يُستدعى عندما يتم العثور على عقدة OutlineElement في المستند.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// يحصل على العدد الإجمالي للعقد بواسطة الزائر
    /// </summary>
    public Int32 NodeCount
    {
        get { return this.nodecount; }
    }

    private readonly StringBuilder mBuilder;
    private bool mIsSkipText;
    private Int32 nodecount;
}
```

### انظر أيضًا

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* class [Page](../page/)
* interface [INotebookChildNode](../inotebookchildnode/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


