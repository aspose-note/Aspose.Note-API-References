---
title: Document
second_title: Aspose.Note لمرجع NET API
description: يمثل وثيقة Aspose.Note .
type: docs
weight: 60
url: /ar/net/aspose.note/document/
---
## Document class

يمثل وثيقة Aspose.Note .

```csharp
public class Document : CompositeNode<Page>, INotebookChildNode
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [Document](document#constructor)() | يقوم بتهيئة مثيل جديد لملف[`Document`](../document) class. ينشئ مستند OneNote فارغًا. |
| [Document](document#constructor_1)(Stream) | يقوم بتهيئة مثيل جديد لملف[`Document`](../document) class. يفتح مستند OneNote موجود من دفق. |
| [Document](document#constructor_3)(string) | يقوم بتهيئة مثيل جديد لملف[`Document`](../document) class. يفتح مستند OneNote موجود من ملف. |
| [Document](document#constructor_2)(Stream, LoadOptions) | يقوم بتهيئة مثيل جديد لملف[`Document`](../document) class. يفتح مستند OneNote موجود من دفق. يسمح بتحديد خيارات إضافية مثل كلمة مرور التشفير. |
| [Document](document#constructor_4)(string, LoadOptions) | يقوم بتهيئة مثيل جديد لملف[`Document`](../document) class. يفتح مستند OneNote موجود من ملف. يسمح بتحديد خيارات إضافية مثل كلمة مرور التشفير. |

## الخصائص

| اسم | وصف |
| --- | --- |
| [AutomaticLayoutChangesDetectionEnabled](../../aspose.note/document/automaticlayoutchangesdetectionenabled) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان Aspose.Note يقوم باكتشاف تغييرات التخطيط تلقائيًا. القيمة الافتراضية هي`حقيقي` . |
| [Color](../../aspose.note/document/color) { get; set; } | الحصول على اللون أو تحديده . |
| [CreationTime](../../aspose.note/document/creationtime) { get; set; } | الحصول على وقت الإنشاء أو تعيينه. |
| [DisplayName](../../aspose.note/document/displayname) { get; set; } | الحصول على أو تحديد اسم العرض . |
| [Document](../../aspose.note/node/document) { get; } | يحصل على مستند العقدة . |
| [FileFormat](../../aspose.note/document/fileformat) { get; } | الحصول على تنسيق الملف (OneNote 2010 ، OneNote Online) . |
| [FirstChild](../../aspose.note/compositenode`1/firstchild) { get; } |  |
| [Guid](../../aspose.note/document/guid) { get; } | يحصل على معرف الكائن الفريد عالميًا . |
| [IsComposite](../../aspose.note/compositenode`1/iscomposite) { get; } |  |
| [LastChild](../../aspose.note/compositenode`1/lastchild) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | الحصول على العقدة التالية على نفس مستوى شجرة العقدة. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | يحصل على نوع العقدة . |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | يحصل على العقدة الأصلية . |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | الحصول على العقدة السابقة على نفس مستوى شجرة العقدة. |

## طُرق

| اسم | وصف |
| --- | --- |
| override [Accept](../../aspose.note/document/accept)(DocumentVisitor) | يقبل زائر العقدة . |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildfirst)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode`1/appendchildlast)(T1) |  |
| [DetectLayoutChanges](../../aspose.note/document/detectlayoutchanges)() | يكتشف جميع التغييرات التي تم إجراؤها على تخطيط المستند منذ السابق[`DetectLayoutChanges`](./detectlayoutchanges) call. في حالة[`AutomaticLayoutChangesDetectionEnabled`](./automaticlayoutchangesdetectionenabled) اضبط على "صحيح" ، ويستخدم تلقائيًا في بداية تصدير المستند. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode`1/getchildnodes)() |  |
| [GetEnumerator](../../aspose.note/compositenode`1/getenumerator)() |  |
| [GetPageHistory](../../aspose.note/document/getpagehistory)(Page) | يحصل على ملف[`PageHistory`](../pagehistory) الذي يحتوي على التاريخ الكامل لكل صفحة معروضة في مستند (الأقدم في الفهرس 0) . يمكن الوصول إلى مراجعة الصفحة الحالية كـ[`Current`](../pagehistory/current)ومضمنة بشكل منفصل عن مجموعة الإصدارات التاريخية. |
| [Import](../../aspose.note/document/import#import)(Stream, PdfImportOptions, MergeOptions) | يستورد مجموعة من الصفحات من مستند PDF المقدم. |
| [Import](../../aspose.note/document/import#import_1)(string, PdfImportOptions, MergeOptions) | يستورد مجموعة من الصفحات من مستند PDF المقدم. |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode`1/insertchild)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, IEnumerable&lt;Page&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode`1/insertchildrenrange)(int, params Page[]) |  |
| [Merge](../../aspose.note/document/merge)(IEnumerable&lt;Page&gt;, MergeOptions) | يدمج مجموعة من الصفحات في المستند. |
| [Print](../../aspose.note/document/print#print)() | طباعة المستند باستخدام الطابعة الافتراضية. |
| [Print](../../aspose.note/document/print#print_1)(PrintOptions) | طباعة المستند باستخدام الطابعة الافتراضية. |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode`1/removechild)(T1) |  |
| [Save](../../aspose.note/document/save#save)(Stream) | يحفظ مستند OneNote في دفق. |
| [Save](../../aspose.note/document/save#save_3)(string) | يحفظ مستند OneNote في ملف. |
| [Save](../../aspose.note/document/save#save_1)(Stream, SaveFormat) | يحفظ مستند OneNote في دفق بالتنسيق المحدد. |
| [Save](../../aspose.note/document/save#save_2)(Stream, SaveOptions) | يحفظ مستند OneNote في دفق باستخدام خيارات الحفظ المحددة. |
| [Save](../../aspose.note/document/save#save_4)(string, SaveFormat) | يحفظ مستند OneNote في ملف بالتنسيق المحدد. |
| [Save](../../aspose.note/document/save#save_5)(string, SaveOptions) | يحفظ مستند OneNote في ملف باستخدام خيارات الحفظ المحددة. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted)(Stream, out Document) | للتحقق مما إذا كان مستند من دفق مشفر . للتحقق من ذلك ، نحتاج إلى تحميل هذا المستند بالكامل. لذلك يمكن أن تؤدي هذه الطريقة إلى عقوبة الأداء. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_3)(string, out Document) | للتحقق مما إذا كان مستند من ملف مشفر . للتحقق من ذلك ، نحتاج إلى تحميل هذا المستند بالكامل. لذلك يمكن أن تؤدي هذه الطريقة إلى عقوبة الأداء. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_1)(Stream, LoadOptions, out Document) | للتحقق مما إذا كان مستند من دفق مشفر . للتحقق من ذلك ، نحتاج إلى تحميل هذا المستند بالكامل. لذلك يمكن أن تؤدي هذه الطريقة إلى عقوبة الأداء. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_2)(Stream, string, out Document) | للتحقق مما إذا كان مستند من دفق مشفر . للتحقق من ذلك ، نحتاج إلى تحميل هذا المستند بالكامل. لذلك يمكن أن تؤدي هذه الطريقة إلى عقوبة الأداء. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_4)(string, LoadOptions, out Document) | للتحقق مما إذا كان مستند من ملف مشفر . للتحقق من ذلك ، نحتاج إلى تحميل هذا المستند بالكامل. لذلك يمكن أن تؤدي هذه الطريقة إلى عقوبة الأداء. |
| static [IsEncrypted](../../aspose.note/document/isencrypted#isencrypted_5)(string, string, out Document) | للتحقق مما إذا كان مستند من ملف مشفر . للتحقق من ذلك ، نحتاج إلى تحميل هذا المستند بالكامل. لذلك يمكن أن تؤدي هذه الطريقة إلى عقوبة الأداء. |

### أمثلة

يوضح كيفية إرسال المستند إلى الطابعة باستخدام مربع حوار Windows القياسي مع الخيارات الافتراضية.

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

يوضح كيفية عمل مستند مشفر.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

LoadOptions loadOptions = new LoadOptions { DocumentPassword = "password" };
Document doc = new Document(dataDir + "Sample1.one", loadOptions);
```

يوضح كيفية حفظ المستند مع التشفير.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

يوضح كيفية حفظ مستند باستخدام تعداد SaveFormat.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

يوضح كيفية حفظ مستند باستخدام OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

يوضح كيفية الحصول على عدد الصفحات للمستند.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "Aspose.one");

// احصل على عدد الصفحات
int count = oneFile.Count();

// عدد الطباعة على شاشة الإخراج
Console.WriteLine(count);
```

يوضح كيفية حفظ مستند بتنسيق pdf باستخدام الإعدادات الافتراضية.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "Aspose.one");

// احفظ المستند بصيغة PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

يوضح كيفية حفظ مستند بتنسيق gif.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// احفظ المستند بصيغة gif.
oneFile.Save(dataDir, SaveFormat.Gif);
```

يوضح كيفية ضبط جودة الصورة عند حفظ المستند كصورة بتنسيق JPEG.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// احفظ المستند.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

يوضح كيفية ضبط دقة الصورة عند حفظ المستند كصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// احفظ المستند.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

يوضح كيفية الحصول على تنسيق ملف للمستند.

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
        // معالجة OneNote عبر الإنترنت
        break;
}
```

يوضح كيفية ربط ارتباط تشعبي بصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com "} ;

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

يوضح كيفية حفظ مستند في دفق.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// قم بإرجاع موضع الدفق إلى الصفر بحيث يكون جاهزًا للقارئ التالي.
dstStream.Seek(0, SeekOrigin.Begin);
```

يوضح كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور.

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

يوضح كيفية إضافة قسم جديد إلى دفتر ملاحظات.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر ملاحظات OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// إلحاق طفل جديد بدفتر الملاحظات
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// حفظ دفتر الملاحظات
notebook.Save(dataDir);
```

يوضح كيفية التحقق من فشل تحميل المستند لأن تنسيق OneNote 2007 غير مدعوم.

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

يوضح كيفية استعادة الإصدار السابق من الصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// قم بتحميل مستند OneNote واحصل على الطفل الأول           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

يوضح كيفية استنساخ الصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// تحميل مستند OneNote
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// استنساخ في مستند جديد بدون محفوظات
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// استنساخ في مستند جديد مع المحفوظات
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

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

يوضح كيفية تعيين وصف نصي للصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page(document);
var image = new Image(document, dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

يوضح كيفية الحصول على معلومات التعريف حول الصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// قم بتحميل المستند في Aspose.
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

عندما يتم حفظ صفحات OneNote الطويلة بتنسيق pdf ، يتم تقسيمها عبر الصفحات. يوضح النموذج كيفية تكوين منطق تقسيم الكائنات الموجودة في فواصل الصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// أو
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

يوضح كيفية حفظ مستند بتنسيق png.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "Aspose.one");

// تهيئة كائن ImageSaveOptions 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // تعيين فهرس الصفحة
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// احفظ المستند بصيغة PNG.
oneFile.Save(dataDir, opts);
```

يوضح كيفية تحرير محفوظات الصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// قم بتحميل مستند OneNote واحصل على الطفل الأول           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
```

يوضح كيفية التحقق مما إذا كان المستند محميًا بكلمة مرور معينة.

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

يوضح كيفية المرور عبر محتوى دفتر ملاحظات.

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
            // افعل شيئًا مع المستند الفرعي
        }
        else if (notebookChildNode is Notebook)
        {
            // افعل شيئًا باستخدام دفتر ملاحظات الأطفال
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

يوضح كيفية الحصول على صورة من مستند.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "Aspose.one");

// احصل على جميع عُقد الصور
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // حفظ بايت الصورة في ملف
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

يوضح كيفية حفظ مستند بتنسيق pdf.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "Aspose.one");

// تهيئة كائن PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // تعيين فهرس الصفحة للصفحة الأولى ليتم حفظها
                              PageIndex = 0,

                              // تعيين عدد الصفحات
                              PageCount = 1,
                          };

// احفظ المستند بصيغة PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

يوضح كيفية حفظ مستند بتنسيق pdf باستخدام إعدادات محددة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
Document doc = new Document(dataDir + "Aspose.one");

// تهيئة كائن PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // استخدم ضغط Jpeg
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // جودة ضغط JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

يوضح كيفية إرسال المستند إلى طابعة باستخدام مربع حوار Windows القياسي مع خيارات محددة.

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

يوضح كيفية الحصول على المعلومات الوصفية للصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "Aspose.one");

// احصل على جميع عُقد الصور
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

يوضح كيفية الحصول على محتوى ملف مرفق.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Attachments();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "Sample1.one");

// احصل على قائمة بعقد الملفات المرفقة
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// كرر عبر جميع العقد
foreach (AttachedFile file in nodes)
{
    // تحميل الملف المرفق إلى كائن تيار
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // إنشاء ملف محلي
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // نسخ الملف
            CopyStream(outputStream, fileStream);
        }
    }
}
```

يوضح كيفية الحصول على محفوظات الصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// تحميل مستند OneNote
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

يوضح كيفية إضافة ملف إلى مستند باستخدام مسار الملف.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Attachments();

// إنشاء كائن من فئة المستند
Document doc = new Document();

// تهيئة كائن فئة الصفحة
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// تهيئة كائن فئة المخطط التفصيلي
Outline outline = new Outline(doc);

// تهيئة كائن فئة OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// تهيئة كائن فئة AttachedFile
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// أضف الملف المرفق
outlineElem.AppendChildLast(attachedFile);

// إضافة عقدة عنصر المخطط التفصيلي
outline.AppendChildLast(outlineElem);

// إضافة عقدة المخطط التفصيلي
page.AppendChildLast(outline);

// إضافة عقدة الصفحة
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

يوضح كيفية إنشاء مستند وحفظه بتنسيق html باستخدام الخيارات الافتراضية.

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
dataDir = dataDir + "CreateOneNoteDocAndSaveToHTML_out.html";
doc.Save(dataDir);
```

يوضح كيفية التحقق مما إذا كانت الصفحة عبارة عن صفحة تعارض (أي أنها تحتوي على تغييرات يتعذر على OneNote دمجها تلقائيًا).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// تحميل مستند OneNote
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

    // بشكل افتراضي يتم تخطي صفحات التعارض فقط عند الحفظ.
    // إذا قمت بتمييزه على أنه غير متعارض ، فسيتم حفظه كالمعتاد في السجل.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

يوضح كيفية إضافة صورة من ملف إلى مستند بخصائص يحددها المستخدم.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

// تحميل المستند من الدفق.
Document doc = new Document(dataDir + "Aspose.one");

// احصل على الصفحة الأولى من المستند.
Aspose.Note.Page page = doc.FirstChild;

// قم بتحميل صورة من الملف.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // قم بتغيير حجم الصورة وفقًا لاحتياجاتك (اختياري).
                              Width = 100,
                              Height = 100,

                              // تعيين موقع الصورة في الصفحة (اختياري).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // تعيين محاذاة الصورة
                              Alignment = HorizontalAlignment.Right
                          };

// أضف الصورة إلى الصفحة.
page.AppendChildLast(image);
```

يوضح كيفية إضافة ملف من دفق إلى مستند.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Attachments();

// إنشاء كائن من فئة المستند
Document doc = new Document();

// تهيئة كائن فئة الصفحة
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// تهيئة كائن فئة المخطط التفصيلي
Outline outline = new Outline(doc);

// تهيئة كائن فئة OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // Initialize AttachedFile class object وكذلك تمرير مسار الرمز الخاص به
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // أضف الملف المرفق
    outlineElem.AppendChildLast(attachedFile);
}

// إضافة عقدة عنصر المخطط التفصيلي
outline.AppendChildLast(outlineElem);

// إضافة عقدة المخطط التفصيلي
page.AppendChildLast(outline);

// إضافة عقدة الصفحة
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

عندما يتم حفظ صفحات OneNote الطويلة بتنسيق pdf ، يتم تقسيمها عبر الصفحات. يوضح المثال كيفية تكوين منطق تقسيم الكائنات الموجودة في فواصل الصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// قم بتحميل المستند في Aspose.
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

يوضح كيفية إنشاء مستند بصفحة معنونة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// إنشاء كائن من فئة المستند
Document doc = new Aspose.Note.Document();

// تهيئة كائن فئة الصفحة
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// النمط الافتراضي لكل النص في المستند.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// تعيين خصائص عنوان الصفحة
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// إلحاق عقدة الصفحة في المستند
doc.AppendChildLast(page);

// حفظ مستند OneNote
dataDir = dataDir + "CreateDocWithPageTitle_out.one";
doc.Save(dataDir);
```

يوضح كيفية إضافة صورة من دفق إلى مستند.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

// إنشاء كائن من فئة المستند
Document doc = new Document();

// تهيئة كائن فئة الصفحة
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // قم بتحميل الصورة الثانية باستخدام اسم الصورة والامتداد والدفق.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // تعيين محاذاة الصورة
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// حفظ مستند OneNote
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

يوضح كيفية إضافة صورة من ملف إلى مستند.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

// إنشاء كائن من فئة المستند
Document doc = new Document();

// تهيئة كائن فئة الصفحة
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// تهيئة كائن فئة المخطط التفصيلي وتعيين خصائص الإزاحة
Outline outline = new Outline(doc);

// تهيئة كائن فئة OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// قم بتحميل صورة عن طريق مسار الملف.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // تعيين محاذاة الصورة
                              Alignment = HorizontalAlignment.Right
                          };

// إضافة صورة
outlineElem.AppendChildLast(image);

// أضف عناصر المخطط التفصيلي
outline.AppendChildLast(outlineElem);

// إضافة عقدة المخطط التفصيلي
page.AppendChildLast(outline);

// إضافة عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

يوضح كيفية إنشاء مستند بنص.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// إنشاء كائن من فئة المستند
Document doc = new Document();

// تهيئة كائن فئة الصفحة
Page page = new Page(doc);

// تهيئة كائن فئة المخطط التفصيلي
Outline outline = new Outline(doc);

// تهيئة كائن فئة OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// تهيئة كائن فئة TextStyle وتعيين خصائص التنسيق
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// تهيئة كائن فئة RichText وتطبيق نمط النص
RichText text = new RichText(doc) { Text = "Hello OneNote text!", ParagraphStyle = textStyle };

// إضافة عقدة RichText
outlineElem.AppendChildLast(text);

// إضافة عقدة OutlineElement
outline.AppendChildLast(outlineElem);

// إضافة عقدة المخطط التفصيلي
page.AppendChildLast(outline);

// إضافة عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote
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
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// النمط الافتراضي لكل النص في المستند.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// إلحاق عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote بتنسيقات مختلفة وتعيين حجم خط النص واكتشاف تغييرات التخطيط يدويًا.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
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

يوضح كيفية ربط ارتباط تشعبي بنص.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tasks();

// إنشاء كائن من فئة المستند
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
                                       IsHyperlink = true,
                                       HyperlinkAddress = "www.google.com"
                                   };

RichText text = new RichText() { ParagraphStyle = ParagraphStyle.Default }
                    .Append("This is ", textStyleRed)
                    .Append("hyperlink", textStyleHyperlink)
                    .Append(". This text is not a hyperlink.", TextStyle.Default);

OutlineElement outlineElem = new OutlineElement();
outlineElem.AppendChildLast(text);

// أضف عناصر المخطط التفصيلي
outline.AppendChildLast(outlineElem);

// تهيئة كائن فئة العنوان
Title title = new Title() { TitleText = titleText };

// تهيئة كائن فئة الصفحة
Page page = new Note.Page() { Title = title };

// إضافة عقدة المخطط التفصيلي
page.AppendChildLast(outline);

// إضافة عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote
dataDir = dataDir + "AddHyperlink_out.one";
doc.Save(dataDir);
```

يوضح كيفية الوصول إلى محتوى مستند باستخدام الزائر.

```csharp
public static void Run()
{
    // المسار إلى دليل المستندات.
    string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

    // افتح المستند الذي نريد تحويله.
    Document doc = new Document(dataDir + "Aspose.one");

    // إنشاء كائن يرث من فئة DocumentVisitor.
    MyOneNoteToTxtWriter myConverter = new MyOneNoteToTxtWriter();

    // هذا هو نمط الزائر المعروف. احصل على النموذج لقبول زائر.
    // سيقوم النموذج بالتكرار من خلال نفسه عن طريق استدعاء الطرق المقابلة
    // على كائن الزائر (وهذا ما يسمى بالزيارة).
    //
    // لاحظ أن كل عقدة في نموذج الكائن لها طريقة Accept لذا فإن زيارة
    يمكن تنفيذ // ليس فقط للمستند بأكمله ، ولكن لأي عقدة في المستند.
    doc.Accept(myConverter);

    // بمجرد اكتمال الزيارة ، يمكننا استرداد نتيجة العملية ،
    // التي في هذا المثال تراكمت في الزائر.
    Console.WriteLine(myConverter.GetText());
    Console.WriteLine(myConverter.NodeCount);            
}

/// <summary>
/// تنفيذ بسيط لحفظ مستند بتنسيق النص العادي. تم تنفيذه كزائر.
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
    /// يحصل على النص العادي للمستند الذي قام الزائر بتجميعه.
    /// </summary>
    public string GetText()
    {
        return mBuilder.ToString();
    }

    /// <summary>
    /// يضيف نصًا إلى الإخراج الحالي. يكرم علامة الإخراج الممكنة / المعطلة.
    /// </summary>
    private void AppendText(string text)
    {
        if (!mIsSkipText)
        {
            mBuilder.AppendLine(text);
        }
    }

    /// <summary>
    /// يتم الاستدعاء عند مواجهة عقدة RichText في المستند.
    /// </summary>
    public override void VisitRichTextStart(RichText run)
    {
        ++nodecount;
        AppendText(run.Text);
    }

    /// <summary>
    /// يتم الاستدعاء عند مواجهة عقدة المستند في المستند.
    /// </summary>
    public override void VisitDocumentStart(Document document)
    {
        ++nodecount;
    }

    /// <summary>
    /// يتم الاستدعاء عند مواجهة عقدة الصفحة في المستند.
    /// </summary>
    public override void VisitPageStart(Page page)
    {
        ++nodecount;
        this.AppendText($"*** Page '{page.Title?.TitleText?.Text ?? "(no title)"}' ***");
    }

    /// <summary>
    /// يتم الاستدعاء عند انتهاء معالجة عقدة الصفحة.
    /// </summary>
    public override void VisitPageEnd(Page page)
    {
        this.AppendText(string.Empty);
    }

    /// <summary>
    /// يتم استدعاؤها عند مواجهة عقدة العنوان في المستند.
    /// </summary>
    public override void VisitTitleStart(Title title)
    {
        ++nodecount;
    }

    /// <summary>
    /// يتم استدعاؤها عند مواجهة عقدة صورة في المستند.
    /// </summary>
    public override void VisitImageStart(Image image)
    {
        ++nodecount;
    }

    /// <summary>
    /// يتم الاستدعاء عند مواجهة عقدة OutlineGroup في المستند.
    /// </summary>
    public override void VisitOutlineGroupStart(OutlineGroup outlineGroup)
    {
        ++nodecount;
    }

    /// <summary>
    /// يتم الاستدعاء عند مواجهة عقدة مخطط تفصيلي في المستند.
    /// </summary>
    public override void VisitOutlineStart(Outline outline)
    {
        ++nodecount;
    }

    /// <summary>
    /// يتم استدعاؤه عند مواجهة عقدة OutlineElement في المستند.
    /// </summary>
    public override void VisitOutlineElementStart(OutlineElement outlineElement)
    {
        ++nodecount;
    }

    /// <summary>
    /// الحصول على العدد الإجمالي للعقد بواسطة الزائر
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

### أنظر أيضا

* class [CompositeNode&lt;T&gt;](../compositenode-1)
* class [Page](../page)
* interface [INotebookChildNode](../inotebookchildnode)
* مساحة الاسم [Aspose.Note](../../aspose.note)
* المجسم [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
