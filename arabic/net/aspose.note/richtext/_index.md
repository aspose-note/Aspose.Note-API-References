---
title: "الفئة RichText"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "فئة Aspose.Note.RichText. تمثل نصًا غنيًا."
type: docs
weight: 610
url: /ar/net/aspose.note/richtext/
---
## RichText class

يمثل نصًا غنيًا.

```csharp
public sealed class RichText : Node, IEnumerable<char>, IOutlineElementChildNode, ITaggable
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [RichText](richtext/)() | يُنشئ مثيلًا جديدًا لفئة `RichText`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Alignment](../../aspose.note/richtext/alignment/) { get; set; } | يحصل أو يعيّن المحاذاة. |
| [Document](../../aspose.note/node/document/) { get; } | يحصل على مستند العقدة. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه العقدة مركبة. إذا كانت true يمكن للعقدة أن تحتوي على عقد فرعية. |
| [IsTitleDate](../../aspose.note/richtext/istitledate/) { get; } | يحصل على قيمة تشير إلى ما إذا كان عنصر RichText يحتوي على التاريخ في عنوان الصفحة. |
| [IsTitleText](../../aspose.note/richtext/istitletext/) { get; } | يحصل على قيمة تشير إلى ما إذا كان عنصر RichText يحتوي على نص عنوان الصفحة. |
| [IsTitleTime](../../aspose.note/richtext/istitletime/) { get; } | يحصل على قيمة تشير إلى ما إذا كان عنصر RichText يحتوي على الوقت في عنوان الصفحة. |
| [LastModifiedTime](../../aspose.note/richtext/lastmodifiedtime/) { get; set; } | يحصل أو يعيّن وقت آخر تعديل. |
| [Length](../../aspose.note/richtext/length/) { get; } | يحصل على طول النص. |
| [LineSpacing](../../aspose.note/richtext/linespacing/) { get; set; } | يحصل أو يضبط تباعد الأسطر. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | يحصل على العقدة التالية في نفس مستوى شجرة العقد. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | يحصل على نوع العقدة. |
| [ParagraphStyle](../../aspose.note/richtext/paragraphstyle/) { get; set; } | يحصل أو يضبط نمط الفقرة. تُستخدم هذه الإعدادات إذا لم يكن هناك كائن TextStyle مطابق في مجموعة Styles أو إذا لم يحدد هذا الكائن الإعداد المطلوب. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | يحصل على العقدة الأصلية. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | يحصل على العقدة السابقة في نفس مستوى شجرة العقد. |
| [SpaceAfter](../../aspose.note/richtext/spaceafter/) { get; set; } | يحصل أو يضبط الحد الأدنى للمسافة بعد. |
| [SpaceBefore](../../aspose.note/richtext/spacebefore/) { get; set; } | يحصل أو يضبط الحد الأدنى للمسافة قبل. |
| [Tags](../../aspose.note/richtext/tags/) { get; } | يحصل على قائمة جميع العلامات في الفقرة. |
| [Text](../../aspose.note/richtext/text/) { get; set; } | يحصل أو يضبط النص. يجب ألا يحتوي السلسلة على أي أحرف ذات القيمة 10 (سطر جديد). |
| [TextRuns](../../aspose.note/richtext/textruns/) { get; } | يحصل على مجموعة تشغيل النص. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Accept](../../aspose.note/richtext/accept/)(DocumentVisitor) | يقبل زائر العقدة. |
| [Append](../../aspose.note/richtext/append/#append)(string) | يضيف سلسلة إلى نطاق النص الأخير. |
| [Append](../../aspose.note/richtext/append/#append_1)(string, TextStyle) | يضيف سلسلة إلى النهاية. |
| [AppendFront](../../aspose.note/richtext/appendfront/#appendfront)(string) | يضيف سلسلة إلى مقدمة نطاق النص الأول. |
| [AppendFront](../../aspose.note/richtext/appendfront/#appendfront_1)(string, TextStyle) | يضيف سلسلة إلى المقدمة. |
| [Clear](../../aspose.note/richtext/clear/)() | يمسح محتوى هذا الكائن. |
| [GetEnumerator](../../aspose.note/richtext/getenumerator/)() | يرجع عدادًا يتنقل عبر أحرف كائن RichText هذا. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof)(char) | يرجع الفهرس الصفري للظهور الأول للحرف Unicode المحدد في هذه السلسلة. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_3)(string) | يرجع الفهرس الصفري للظهور الأول للسلسلة المحددة في هذا الكائن. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_1)(char, int) | يرجع الفهرس الصفري للظهور الأول للحرف Unicode المحدد في هذه السلسلة. يبدأ البحث من موضع حرف محدد. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_4)(string, int) | يرجع الفهرس الصفري للظهور الأول للسلسلة المحددة في هذا الكائن. يبدأ البحث من موضع حرف محدد. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_8)(string, StringComparison) | يرجع الفهرس الصفري للظهور الأول للسلسلة المحددة في الكائن الحالي. يحدد معامل نوع البحث الذي يُستخدم للسلسلة المحددة. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_2)(char, int, int) | يرجع الفهرس الصفري للظهور الأول للحرف المحدد في هذا الكائن. يبدأ البحث من موضع حرف محدد ويفحص عددًا محددًا من مواضع الأحرف. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_5)(string, int, int) | يرجع الفهرس الصفري للظهور الأول للسلسلة المحددة في هذا الكائن. يبدأ البحث من موضع حرف محدد ويفحص عددًا محددًا من مواضع الأحرف. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_7)(string, int, StringComparison) | يرجع الفهرس الصفري للظهور الأول للسلسلة المحددة في الكائن الحالي. تحدد المعلمات موضع بدء البحث في السلسلة الحالية ونوع البحث الذي يُستخدم للسلسلة المحددة. |
| [IndexOf](../../aspose.note/richtext/indexof/#indexof_6)(string, int, int, StringComparison) | يرجع الفهرس الصفري للظهور الأول للسلسلة المحددة في الكائن الحالي. |
| [Insert](../../aspose.note/richtext/insert/#insert)(int, string) | يدرج سلسلة محددة في موضع فهرس محدد في هذه الحالة. |
| [Insert](../../aspose.note/richtext/insert/#insert_1)(int, string, TextStyle) | يدرج سلسلة محددة مع نمط محدد في موضع فهرس محدد في هذه الحالة. |
| [Remove](../../aspose.note/richtext/remove/#remove)(int) | يزيل جميع الأحرف في الحالة الحالية، بدءًا من موضع محدد ومتابعةً حتى الموضع الأخير. |
| [Remove](../../aspose.note/richtext/remove/#remove_1)(int, int) | يزيل عددًا محددًا من الأحرف في الحالة الحالية بدءًا من موضع محدد. |
| [Replace](../../aspose.note/richtext/replace/#replace)(char, char) | يستبدل جميع تكرارات حرف يونيكود محدد في هذه الحالة بحرف يونيكود آخر محدد. |
| [Replace](../../aspose.note/richtext/replace/#replace_1)(string, string) | يستبدل جميع تكرارات سلسلة محددة في الحالة الحالية بسلسلة أخرى محددة. |
| [Replace](../../aspose.note/richtext/replace/#replace_2)(string, string, TextStyle) | يستبدل جميع تكرارات سلسلة محددة في الحالة الحالية بسلسلة أخرى محددة بنمط محدد. |
| [Trim](../../aspose.note/richtext/trim/#trim)() | يزيل جميع الأحرف البيضاء في البداية والنهاية. |
| [Trim](../../aspose.note/richtext/trim/#trim_1)(char) | يزيل جميع الحالات في البداية والنهاية لحرف. |
| [Trim](../../aspose.note/richtext/trim/#trim_2)(params char[]) | يزيل جميع التكرارات في البداية والنهاية لمجموعة من الأحرف المحددة في مصفوفة. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend)() | يزيل جميع الأحرف البيضاء المتبقية في النهاية. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend_1)(char) | يزيل جميع التكرارات المتبقية لحرف. |
| [TrimEnd](../../aspose.note/richtext/trimend/#trimend_2)(params char[]) | يزيل جميع التكرارات المتبقية لمجموعة من الأحرف المحددة في مصفوفة. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart)() | يزيل جميع الأحرف البيضاء في البداية. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart_1)(char) | يزيل جميع التكرارات في البداية لحرف محدد. |
| [TrimStart](../../aspose.note/richtext/trimstart/#trimstart_2)(params char[]) | يزيل جميع التكرارات في البداية لمجموعة من الأحرف المحددة في مصفوفة. |

## أمثلة

يوضح كيفية الحصول على كل النص من المستند.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Text();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// استرجاع النص
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// طباعة النص على شاشة الإخراج
Console.WriteLine(text);
```

يوضح كيفية الحصول على كل النص من الصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Text();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// احصل على قائمة بعقد الصفحة
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // استرجاع النص
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // طباعة النص على شاشة الإخراج
    Console.WriteLine(text);
}
```

دعنا نبرز عناوين الصفحة بين العناوين الأخرى بزيادة حجم الخط.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// حمّل المستند إلى Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// تكرار عبر عناوين الصفحة.
foreach (var title in document.Select(e => e.Title.TitleText))
{
    title.ParagraphStyle.FontSize = 24;
    title.ParagraphStyle.IsBold = true;

    foreach (var run in title.TextRuns)
    {
        run.Style.FontSize = 24;
        run.Style.IsBold = true;
    }
}

document.Save(Path.Combine(dataDir, "ChangePageTitleStyle.pdf"));
```

يوضح كيفية الحصول على النص من كل صف في الجدول.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tables();

// حمّل المستند إلى Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// احصل على قائمة بعقد الجدول
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // التكرار عبر صفوف الجدول
    foreach (TableRow row in table)
    {
        // استرجاع النص
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // طباعة النص على شاشة الإخراج
        Console.WriteLine(text);
    }
}
```

يوضح كيفية الحصول على النص من جدول.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tables();

// حمّل المستند إلى Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// احصل على قائمة بعقد الجدول
IList<Table> nodes = document.GetChildNodes<Table>();

// تعيين عدد الجداول
int tblCount = 0;

foreach (Table table in nodes)
{
    tblCount++;
    Console.WriteLine("table # " + tblCount);

    // استرجاع النص
    string text = string.Join(Environment.NewLine, table.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

    // طباعة النص على شاشة الإخراج
    Console.WriteLine(text);
}
```

دعنا نبرز تغييرات النص الأخيرة عن طريق التظليل.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// حمّل المستند إلى Aspose.Note.
Document document = new Document(dataDir + "Aspose.one");

// احصل على عقد RichText المعدلة الأسبوع الماضي.
var richTextNodes = document.GetChildNodes<RichText>().Where(e => e.LastModifiedTime >= DateTime.Today.Subtract(TimeSpan.FromDays(7)));

foreach (var node in richTextNodes)
{
    // تعيين لون التظليل
    node.ParagraphStyle.Highlight = Color.DarkGreen;
    foreach (var run in node.TextRuns)
    {
        // تعيين لون التظليل
        run.Style.Highlight = Color.DarkSeaGreen;
    }
}

document.Save(Path.Combine(dataDir, "HighlightAllRecentChanges.pdf"));
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

تعيين لغة التدقيق لنص.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = ParagraphStyle.Default };
text.Append("United States", new TextStyle() { Language = CultureInfo.GetCultureInfo("en-US") })
    .Append(" Germany", new TextStyle() { Language = CultureInfo.GetCultureInfo("de-DE") })
    .Append(" China", new TextStyle() { Language = CultureInfo.GetCultureInfo("zh-CN") });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetProofingLanguageForText.one"));
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

التعامل مع تنسيق النص باستخدام نمط الفقرة.

```csharp
var document = new Document();
var page = new Page();
var outline = new Outline();
var outlineElem = new OutlineElement();

var text = new RichText() { ParagraphStyle = new ParagraphStyle() { FontName = "Courier New", FontSize = 20 } }
                .Append($"DefaultParagraphFontAndSize{Environment.NewLine}")
                .Append($"OnlyDefaultParagraphFont{Environment.NewLine}", new TextStyle() { FontSize = 14 })
                .Append("OnlyDefaultParagraphFontSize", new TextStyle() { FontName = "Verdana" });

outlineElem.AppendChildLast(text);
outline.AppendChildLast(outlineElem);
page.AppendChildLast(outline);
document.AppendChildLast(page);

document.Save(Path.Combine(RunExamples.GetDataDir_Text(), "SetDefaultParagraphStyle.one"));
```

يوضح كيفية الحصول على النص من خلايا الجدول.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tables();

// حمّل المستند إلى Aspose.Note.
Document document = new Document(dataDir + "Sample1.one");

// احصل على قائمة بعقد الجدول
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // التكرار عبر صفوف الجدول
    foreach (TableRow row in table)
    {
        // احصل على قائمة بعقد TableCell
        // التكرار عبر خلايا الجدول
        foreach (TableCell cell in row)
        {
            // استرجاع النص
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // طباعة النص على شاشة الإخراج
            Console.WriteLine(text);
        }
    }
}
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

يعرض كيفية إضافة فقرة جديدة مع العلامة.

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
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText() { Text = "OneNote text.", ParagraphStyle = textStyle };
text.Tags.Add(NoteTag.CreateYellowStar());

// إضافة عقدة نصية
outlineElem.AppendChildLast(text);

// إضافة عقدة عنصر المخطط
outline.AppendChildLast(outlineElem);

// إضافة عقدة المخطط
page.AppendChildLast(outline);

// إضافة عقدة صفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote.
dataDir = dataDir + "AddTextNodeWithTag_out.one";
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

يظهر كيفية الوصول إلى تفاصيل العلامة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// حمّل المستند إلى Aspose.Note.
Document oneFile = new Document(dataDir + "TagFile.one");

// احصل على جميع عقد RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// تكرار عبر كل عقدة
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // استرجاع الخصائص
            Console.WriteLine($"    Completed Time: {noteTag.CompletedTime}");
            Console.WriteLine($"    Create Time: {noteTag.CreationTime}");
            Console.WriteLine($"    Font Color: {noteTag.FontColor}");
            Console.WriteLine($"    Status: {noteTag.Status}");
            Console.WriteLine($"    Label: {noteTag.Label}");
            Console.WriteLine($"    Icon: {noteTag.Icon}");
            Console.WriteLine($"    High Light: {noteTag.Highlight}");
        }
    }
}
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

يعرض كيفية إعداد قالب للاجتماع الأسبوعي.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// إنشاء كائن من فئة Document
var headerStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 16 };
var bodyStyle = new ParagraphStyle() { FontName = "Calibri", FontSize = 12 };

var d = new Document();
bool restartFlag = true;
var outline = d.AppendChildLast(new Page()
                                    {
                                        Title = new Title() { TitleText = new RichText() { Text = $"Weekly meeting {DateTime.Today:d}", ParagraphStyle = ParagraphStyle.Default } }
                                    })
               .AppendChildLast(new Outline() { VerticalOffset = 30, HorizontalOffset = 30 });

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "Important", ParagraphStyle = headerStyle });
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle });
    restartFlag = false;
}

outline.AppendChildLast(new OutlineElement())
       .AppendChildLast(new RichText() { Text = "TO DO", ParagraphStyle = headerStyle, SpaceBefore = 15 });
restartFlag = true;
foreach (var e in new[] { "First", "Second", "Third" })
{
    outline.AppendChildLast(new OutlineElement() { NumberList = CreateListNumberingStyle(bodyStyle, restartFlag) })
           .AppendChildLast(new RichText() { Text = e, ParagraphStyle = bodyStyle, Tags = { NoteCheckBox.CreateBlueCheckBox() } });
    restartFlag = false;
}

d.Save(Path.Combine(dataDir, "meetingNotes.one"));
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

### انظر أيضًا

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [ITaggable](../itaggable/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


