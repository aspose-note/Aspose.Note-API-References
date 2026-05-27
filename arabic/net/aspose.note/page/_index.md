---
title: "الفئة Page"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "الفئة Aspose.Note.Page. تمثل صفحة."
type: docs
weight: 550
url: /ar/net/aspose.note/page/
---
## Page class

يمثل صفحةً.

```csharp
public sealed class Page : CompositeNode<IPageChildNode>
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [Page](page/)() | يُنشئ مثيلاً جديدًا من الفئة `Page`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Author](../../aspose.note/page/author/) { get; set; } | يحصل أو يضبط المؤلف. |
| [BackgroundColor](../../aspose.note/page/backgroundcolor/) { get; set; } | يحصل أو يضبط لون خلفية الصفحة. |
| [CreationTime](../../aspose.note/page/creationtime/) { get; set; } | يحصل أو يعيّن وقت الإنشاء. |
| [Document](../../aspose.note/node/document/) { get; } | يحصل على مستند العقدة. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [IsConflictPage](../../aspose.note/page/isconflictpage/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كانت هذه الصفحة صفحة تعارض. |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/page/lastmodifiedtime/) { get; set; } | يحصل أو يعيّن وقت آخر تعديل. |
| [Level](../../aspose.note/page/level/) { get; set; } | يحصل أو يضبط المستوى. |
| [Margin](../../aspose.note/page/margin/) { get; set; } | يحصل أو يضبط الهامش. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | يحصل على العقدة التالية في نفس مستوى شجرة العقد. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | يحصل على نوع العقدة. |
| [PageContentRevisionSummary](../../aspose.note/page/pagecontentrevisionsummary/) { get; set; } | يحصل أو يضبط ملخص المراجعة للصفحة وعقدها الفرعية. |
| [PageLayoutSize](../../aspose.note/page/pagelayoutsize/) { get; set; } | يحصل أو يضبط حجم تخطيط الصفحة المعروض في المحرر. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | يحصل على العقدة الأصلية. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | يحصل على العقدة السابقة في نفس مستوى شجرة العقد. |
| [SizeType](../../aspose.note/page/sizetype/) { get; set; } | يحصل أو يضبط نوع حجم الصفحة. |
| [Title](../../aspose.note/page/title/) { get; set; } | يحصل أو يضبط العنوان. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Accept](../../aspose.note/page/accept/)(DocumentVisitor) | يقبل زائر العقدة. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| [Clone](../../aspose.note/page/clone/)(bool) | ينسخ الصفحة. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/page/getchildnodes/#getchildnodes_1)() | احصل على جميع العقد الفرعية للصفحة حسب نوع العقدة. |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;IPageChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params IPageChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

## أمثلة

يوضح كيفية ضبط لون خلفية الصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// تحميل مستند OneNote والحصول على العنصر الفرعي الأول.
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in document)
{
    page.BackgroundColor = Color.BlueViolet;
}

document.Save(Path.Combine(dataDir, "SetPageBackgroundColor.one"));
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

يوضح كيفية تعيين عنوان لصفحة.

```csharp
string dataDir = RunExamples.GetDataDir_Text();
string outputPath = dataDir + "CreateTitleMsStyle_out.one";

var doc = new Document();
var page = new Page();

page.Title = new Title()
{
    TitleText = new RichText()
    {
        Text = "Title text.",
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleDate = new RichText()
    {
        Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture),
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleTime = new RichText()
    {
        Text = "12:34",
        ParagraphStyle = ParagraphStyle.Default
    }
};

doc.AppendChildLast(page);

doc.Save(outputPath);
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

يعرض كيفية تعديل معلومات التعريف للصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// تحميل مستند OneNote والحصول على العنصر الفرعي الأول.
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

// قراءة ملخص مراجعة المحتوى لهذه الصفحة.
var pageRevisionInfo = page.PageContentRevisionSummary;

Console.WriteLine(string.Format(
    "Author:\t{0}\nModified:\t{1}",
    pageRevisionInfo.AuthorMostRecent,
    pageRevisionInfo.LastModifiedTime.ToString("dd.MM.yyyy HH:mm:ss")));

// تحديث ملخص مراجعة الصفحة لهذه الصفحة.
pageRevisionInfo.AuthorMostRecent = "New Author";
pageRevisionInfo.LastModifiedTime = DateTime.Now;

document.Save(dataDir + "WorkingWithPageRevisions_out.one");
```

يوضح كيفية المرور عبر جميع الصفحات وإجراء استبدال في النص.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// احصل على جميع عقد RichText
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // استبدال نص الشكل
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// احفظ بأي تنسيق ملف مدعوم
oneFile.Save(dataDir, SaveFormat.Pdf);
```

يوضح كيفية المرور عبر نص الصفحة وإجراء استبدال.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// احصل على جميع عقد RichText
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // استبدال نص الشكل
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// احفظ بأي تنسيق ملف مدعوم
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

يعرض كيفية إضافة صورة جديدة مع علامة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// إنشاء كائن من فئة Document
Document doc = new Document();

// تهيئة كائن فئة Page
Page page = new Page();

// تهيئة كائن فئة Outline
Outline outline = new Outline();

// تهيئة كائن فئة OutlineElement
OutlineElement outlineElem = new OutlineElement();

// تحميل صورة.
Image image = new Image(dataDir + "icon.jpg");

// إدراج صورة في عقدة المستند.
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// إضافة عقدة عنصر المخطط
outline.AppendChildLast(outlineElem);

// إضافة عقدة المخطط
page.AppendChildLast(outline);

// إضافة عقدة صفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote.
dataDir = dataDir + "AddImageNodeWithTag_out.one";
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

يعرض كيفية إدراج قائمة جديدة بترقيم صيني.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// تهيئة مستند OneNote.
Document doc = new Document();

// تهيئة صفحة OneNote.
Page page = new Page();
Outline outline = new Outline();

// تطبيق إعدادات نمط النص.
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// الأرقام في نفس المخطط تُزاد تلقائيًا.
OutlineElement outlineElem1 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText() { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

//------------------------
OutlineElement outlineElem2 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText() { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//------------------------
OutlineElement outlineElem3 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText() { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

//------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// حفظ مستند OneNote.
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

يعرض كيفية إدراج قائمة نقطية جديدة.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// إنشاء كائن من فئة Document
Document doc = new Document();

// تهيئة كائن فئة Page
Page page = new Page();

// تهيئة كائن فئة Outline
Outline outline = new Outline();

// تهيئة كائن الفئة TextStyle وتعيين خصائص التنسيق
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// تهيئة كائنات الفئة OutlineElement وتطبيق النقاط
OutlineElement outlineElem1 = new OutlineElement() { NumberList = new NumberList("*", "Arial", 10) };

// تهيئة كائن الفئة RichText وتطبيق نمط النص
RichText text1 = new RichText() { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement() { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(  ) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement() { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText() { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// إضافة عناصر المخطط
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// إضافة عقدة المخطط
page.AppendChildLast(outline);
// إضافة عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote.
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

يعرض كيفية إدراج قائمة جديدة مع الترقيم.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// إنشاء كائن من فئة Document
Document doc = new Document();

// تهيئة كائن فئة Page
Page page = new Page();

// تهيئة كائن فئة Outline
Outline outline = new Outline();

// تهيئة كائن الفئة TextStyle وتعيين خصائص التنسيق
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// تهيئة كائنات الفئة OutlineElement وتطبيق الترقيم.
// الأرقام في نفس المخطط تُزاد تلقائيًا.
OutlineElement outlineElem1 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText() { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText() { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement() { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText() { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// إضافة عناصر المخطط
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// إضافة عقدة المخطط
page.AppendChildLast(outline);

// إضافة عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote.
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

يوضح كيفية إضافة صفحة مع صفحة فرعية.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// إنشاء كائن من فئة Document
Document doc = new Document();

// تهيئة كائن فئة Page وضبط مستواه
Page page1 = new Page() { Level = 1 };

// تهيئة كائن فئة Page وضبط مستواه
Page page2 = new Page() { Level = 2 };

// تهيئة كائن فئة Page وضبط مستواه
Page page3 = new Page() { Level = 1 };

/*---------- Adding nodes to first Page ----------*/
Outline outline = new Outline();
OutlineElement outlineElem = new OutlineElement();
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText() { Text = "First page.", ParagraphStyle = textStyle };
outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page1.AppendChildLast(outline);

/*---------- Adding nodes to second Page ----------*/
var outline2 = new Outline();
var outlineElem2 = new OutlineElement();
var textStyle2 = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
var text2 = new RichText() { Text = "Second page.", ParagraphStyle = textStyle2 };
outlineElem2.AppendChildLast(text2);
outline2.AppendChildLast(outlineElem2);
page2.AppendChildLast(outline2);

/*---------- Adding nodes to third Page ----------*/
var outline3 = new Outline();
var outlineElem3 = new OutlineElement();
var textStyle3 = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
var text3 = new RichText() { Text = "Third page.", ParagraphStyle = textStyle3 };
outlineElem3.AppendChildLast(text3);
outline3.AppendChildLast(outlineElem3);
page3.AppendChildLast(outline3);

/*---------- Add pages to the OneNote Document ----------*/
doc.AppendChildLast(page1);
doc.AppendChildLast(page2);
doc.AppendChildLast(page3);

// حفظ مستند OneNote.
dataDir = dataDir + "CreateDocWithRootAndSubPages_out.one";
doc.Save(dataDir);
```

### انظر أيضًا

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* interface [IPageChildNode](../ipagechildnode/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


