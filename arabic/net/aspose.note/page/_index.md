---
title: Class Page
second_title: Aspose.Note لمرجع NET API
description: Aspose.Note.Page فصل. يمثل صفحة .
type: docs
weight: 480
url: /ar/net/aspose.note/page/
---
## Page class

يمثل صفحة .

```csharp
public sealed class Page : CompositeNode<IPageChildNode>
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [Page](page/#constructor)() | يقوم بتهيئة مثيل جديد لملف`Page` فئة . |

## الخصائص

| اسم | وصف |
| --- | --- |
| [Author](../../aspose.note/page/author/) { get; set; } | الحصول على أو تعيين المؤلف. |
| [BackgroundColor](../../aspose.note/page/backgroundcolor/) { get; set; } | الحصول على لون خلفية الصفحة أو تعيينه. |
| [CreationTime](../../aspose.note/page/creationtime/) { get; set; } | الحصول على وقت الإنشاء أو تعيينه. |
| [Document](../../aspose.note/node/document/) { get; } | يحصل على وثيقة العقدة . |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [IsConflictPage](../../aspose.note/page/isconflictpage/) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كانت هذه الصفحة عبارة عن صفحة تعارض. |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/page/lastmodifiedtime/) { get; set; } | الحصول على أو تعيين وقت آخر تعديل. |
| [Level](../../aspose.note/page/level/) { get; set; } | الحصول على المستوى أو تحديده . |
| [Margin](../../aspose.note/page/margin/) { get; set; } | الحصول على الهامش أو تحديده . |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | الحصول على العقدة التالية على نفس مستوى شجرة العقدة. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | يحصل على نوع العقدة . |
| [PageContentRevisionSummary](../../aspose.note/page/pagecontentrevisionsummary/) { get; set; } | الحصول على أو تعيين ملخص المراجعة للصفحة والعقد الفرعية. |
| [PageLayoutSize](../../aspose.note/page/pagelayoutsize/) { get; set; } | الحصول على أو تعيين حجم تخطيط الصفحة المعروض في المحرر. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | يحصل على العقدة الأصلية . |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | الحصول على العقدة السابقة على نفس مستوى شجرة العقدة. |
| [SizeType](../../aspose.note/page/sizetype/) { get; set; } | الحصول على نوع حجم الصفحة أو تحديده. |
| [Title](../../aspose.note/page/title/) { get; set; } | الحصول على العنوان أو تعيينه. |

## طُرق

| اسم | وصف |
| --- | --- |
| override [Accept](../../aspose.note/page/accept/)(DocumentVisitor) | يقبل زائر العقدة . |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| [Clone](../../aspose.note/page/clone/)(bool) | استنساخ الصفحة . |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/page/getchildnodes/#getchildnodes_1)() | احصل على جميع العقد الفرعية للصفحة حسب نوع العقدة. |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;IPageChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params IPageChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

### أمثلة

يوضح كيفية تعيين لون خلفية الصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// قم بتحميل مستند OneNote واحصل على الطفل الأول           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in document)
{
    page.BackgroundColor = Color.BlueViolet;
}

document.Save(Path.Combine(dataDir, "SetPageBackgroundColor.one"));
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

يوضح كيفية تعيين عنوان للصفحة.

```csharp
string dataDir = RunExamples.GetDataDir_Text();
string outputPath = dataDir + "CreateTitleMsStyle_out.one";

var doc = new Document();
var page = new Page(doc);

page.Title = new Title(doc)
{
    TitleText = new RichText(doc)
    {
        Text = "Title text.",
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleDate = new RichText(doc)
    {
        Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture),
        ParagraphStyle = ParagraphStyle.Default
    },
    TitleTime = new RichText(doc)
    {
        Text = "12:34",
        ParagraphStyle = ParagraphStyle.Default
    }
};

doc.AppendChildLast(page);

doc.Save(outputPath);
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

يوضح كيفية تحرير المعلومات الوصفية للصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// قم بتحميل مستند OneNote واحصل على الطفل الأول           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

// قراءة ملخص مراجعة المحتوى لهذه الصفحة
var pageRevisionInfo = page.PageContentRevisionSummary;

Console.WriteLine(string.Format(
    "Author:\t{0}\nModified:\t{1}",
    pageRevisionInfo.AuthorMostRecent,
    pageRevisionInfo.LastModifiedTime.ToString("dd.MM.yyyy HH:mm:ss")));

// تحديث ملخص مراجعة الصفحة لهذه الصفحة
pageRevisionInfo.AuthorMostRecent = "New Author";
pageRevisionInfo.LastModifiedTime = DateTime.Now;

document.Save(dataDir + "WorkingWithPageRevisions_out.one");
```

يوضح كيفية المرور عبر جميع الصفحات واستبدالها في النص.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// قم بتحميل المستند في Aspose.
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

// حفظ بأي تنسيق ملف مدعوم
oneFile.Save(dataDir, SaveFormat.Pdf);
```

يوضح كيفية تمرير نص الصفحة واستبداله.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// قم بتحميل المستند في Aspose.
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

// حفظ بأي تنسيق ملف مدعوم
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
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

يوضح كيفية إضافة صورة جديدة مع علامة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// إنشاء كائن من فئة المستند
Document doc = new Document();

// تهيئة كائن فئة الصفحة
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// تهيئة كائن فئة المخطط التفصيلي
Outline outline = new Outline(doc);

// تهيئة كائن فئة OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// تحميل صورة
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// أدخل الصورة في عقدة المستند
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// إضافة عقدة عنصر المخطط التفصيلي
outline.AppendChildLast(outlineElem);

// إضافة عقدة المخطط التفصيلي
page.AppendChildLast(outline);

// إضافة عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote
dataDir = dataDir + "AddImageNodeWithTag_out.one";
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

يوضح كيفية إدراج قائمة جديدة بالترقيم الصيني.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// تهيئة مستند OneNote
Aspose.Note.Document doc = new Aspose.Note.Document();

// تهيئة صفحة OneNote
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// تطبيق إعدادات نمط النص
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// يتم زيادة الأرقام الموجودة في نفس المخطط تلقائيًا.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

// ------------------------
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

// ------------------------
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// ------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// حفظ مستند OneNote
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

يوضح كيفية إدراج قائمة ذات تعداد نقطي جديد.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// إنشاء كائن من فئة المستند
Aspose.Note.Document doc = new Aspose.Note.Document();

// تهيئة كائن فئة الصفحة
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// تهيئة كائن فئة المخطط التفصيلي
Outline outline = new Outline(doc);

// تهيئة كائن فئة TextStyle وتعيين خصائص التنسيق
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// تهيئة كائنات فئة OutlineElement وتطبيق الرموز النقطية
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };

// تهيئة كائن فئة RichText وتطبيق نمط النص
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("*", "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// أضف عناصر المخطط التفصيلي
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// إضافة عقدة المخطط التفصيلي
page.AppendChildLast(outline);
// إضافة عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote
dataDir = dataDir + "ApplyBulletsOnText_out.one"; 
doc.Save(dataDir);
```

يوضح كيفية إدراج قائمة جديدة مع الترقيم.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// إنشاء كائن من فئة المستند
Document doc = new Document();

// تهيئة كائن فئة الصفحة
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// تهيئة كائن فئة المخطط التفصيلي
Outline outline = new Outline(doc);

// تهيئة كائن فئة TextStyle وتعيين خصائص التنسيق
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// تهيئة كائنات فئة OutlineElement وتطبيق الترقيم
// يتم زيادة الأرقام الموجودة في نفس المخطط تلقائيًا.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// أضف عناصر المخطط التفصيلي
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// إضافة عقدة المخطط التفصيلي
page.AppendChildLast(outline);

// إضافة عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

يوضح كيفية إضافة صفحة بصفحة فرعية.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Pages();

// إنشاء كائن من فئة المستند
Document doc = new Document();

// تهيئة كائن فئة الصفحة وتعيين مستواه
Aspose.Note.Page page1 = new Aspose.Note.Page(doc) { Level = 1 };

// تهيئة كائن فئة الصفحة وتعيين مستواه
Aspose.Note.Page page2 = new Aspose.Note.Page(doc) { Level = 2 };

// تهيئة كائن فئة الصفحة وتعيين مستواه
Aspose.Note.Page page3 = new Aspose.Note.Page(doc) { Level = 1 };

/*---------- Adding nodes to first Page ----------*/
Outline outline = new Outline(doc);
OutlineElement outlineElem = new OutlineElement(doc);
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText(doc) { Text = "First page.", ParagraphStyle = textStyle };
outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page1.AppendChildLast(outline);

/*---------- Adding nodes to second Page ----------*/
var outline2 = new Outline(doc);
var outlineElem2 = new OutlineElement(doc);
var textStyle2 = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
var text2 = new RichText(doc) { Text = "Second page.", ParagraphStyle = textStyle2 };
outlineElem2.AppendChildLast(text2);
outline2.AppendChildLast(outlineElem2);
page2.AppendChildLast(outline2);

/*---------- Adding nodes to third Page ----------*/
var outline3 = new Outline(doc);
var outlineElem3 = new OutlineElement(doc);
var textStyle3 = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
var text3 = new RichText(doc) { Text = "Third page.", ParagraphStyle = textStyle3 };
outlineElem3.AppendChildLast(text3);
outline3.AppendChildLast(outlineElem3);
page3.AppendChildLast(outline3);

/*---------- Add pages to the OneNote Document ----------*/
doc.AppendChildLast(page1);
doc.AppendChildLast(page2);
doc.AppendChildLast(page3);

// حفظ مستند OneNote
dataDir = dataDir + "CreateDocWithRootAndSubPages_out.one";
doc.Save(dataDir);
```

### أنظر أيضا

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* interface [IPageChildNode](../ipagechildnode/)
* مساحة الاسم [Aspose.Note](../../aspose.note/)
* المجسم [Aspose.Note](../../)


