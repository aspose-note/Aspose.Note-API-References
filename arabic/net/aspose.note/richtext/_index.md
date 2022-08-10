---
title: RichText
second_title: Aspose.Note لمرجع NET API
description: يمثل نصًا غنيًا .
type: docs
weight: 510
url: /ar/net/aspose.note/richtext/
---
## RichText class

يمثل نصًا غنيًا .

```csharp
public sealed class RichText : Node, IEnumerable<char>, IOutlineElementChildNode, ITaggable
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [RichText](richtext#constructor)() | يقوم بتهيئة مثيل جديد لملف[`RichText`](../richtext) فئة . |

## الخصائص

| اسم | وصف |
| --- | --- |
| [Alignment](../../aspose.note/richtext/alignment) { get; set; } | الحصول على المحاذاة أو تعيينها. |
| [Document](../../aspose.note/node/document) { get; } | يحصل على مستند العقدة . |
| virtual [IsComposite](../../aspose.note/node/iscomposite) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه العقدة مركبة. إذا كان هذا صحيحًا ، يمكن أن تحتوي العقدة على عقد فرعية. |
| [LastModifiedTime](../../aspose.note/richtext/lastmodifiedtime) { get; set; } | الحصول على أو تعيين وقت آخر تعديل. |
| [Length](../../aspose.note/richtext/length) { get; } | الحصول على طول النص. |
| [LineSpacing](../../aspose.note/richtext/linespacing) { get; set; } | الحصول على تباعد الأسطر أو تعيينه. |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | الحصول على العقدة التالية على نفس مستوى شجرة العقدة. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | يحصل على نوع العقدة . |
| [ParagraphStyle](../../aspose.note/richtext/paragraphstyle) { get; set; } | الحصول على نمط الفقرة أو تعيينه. يتم استخدام هذه الإعدادات في حالة عدم وجود كائن TextStyle مطابق فيStyles مجموعة إما أن هذا الكائن لا يحدد الإعداد المطلوب. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | يحصل على العقدة الأصلية . |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | الحصول على العقدة السابقة على نفس مستوى شجرة العقدة. |
| [SpaceAfter](../../aspose.note/richtext/spaceafter) { get; set; } | الحصول على أو تعيين الحد الأدنى من المساحة بعد . |
| [SpaceBefore](../../aspose.note/richtext/spacebefore) { get; set; } | الحصول على أو تعيين الحد الأدنى من المساحة قبل . |
| [Tags](../../aspose.note/richtext/tags) { get; } | يحصل على قائمة بكافة علامات الفقرة . |
| [Text](../../aspose.note/richtext/text) { get; set; } | الحصول على النص أو تعيينه. يجب ألا تحتوي السلسلة على أي أحرف بالقيمة 10 (تغذية السطر) . |
| [TextRuns](../../aspose.note/richtext/textruns) { get; } | يحصل على مجموعة من تشغيلات النص. |

## طُرق

| اسم | وصف |
| --- | --- |
| override [Accept](../../aspose.note/richtext/accept)(DocumentVisitor) | يقبل زائر العقدة . |
| [Append](../../aspose.note/richtext/append#append)(string) | يضيف سلسلة إلى آخر نطاق نصي. |
| [Append](../../aspose.note/richtext/append#append_1)(string, TextStyle) | يضيف سلسلة إلى النهاية . |
| [AppendFront](../../aspose.note/richtext/appendfront#appendfront)(string) | يضيف سلسلة إلى مقدمة نطاق النص الأول. |
| [AppendFront](../../aspose.note/richtext/appendfront#appendfront_1)(string, TextStyle) | يضيف سلسلة للأمام . |
| [Clear](../../aspose.note/richtext/clear)() | يمحو محتوى هذا المثال . |
| [GetEnumerator](../../aspose.note/richtext/getenumerator)() | إرجاع عداد يتكرر خلال أحرف كائن RichText هذا. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof)(char) | إرجاع الفهرس الصفري لأول تكرار لحرف Unicode المحدد في هذه السلسلة. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_3)(string) | إرجاع الفهرس الصفري لأول تكرار للسلسلة المحددة في هذا المثال. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_1)(char, int) | إرجاع الفهرس الصفري للتواجد الأول لحرف Unicode المحدد في هذه السلسلة. يبدأ البحث في موضع حرف محدد. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_4)(string, int) | إرجاع الفهرس الصفري للتواجد الأول للسلسلة المحددة في هذا المثيل. يبدأ البحث في موضع حرف محدد. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_8)(string, StringComparison) | إرجاع الفهرس الصفري للتواجد الأول للسلسلة المحددة في المثيل الحالي. تحدد المعلمة نوع البحث الذي سيتم استخدامه للسلسلة المحددة. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_2)(char, int, int) | إرجاع الفهرس الصفري لأول تكرار للحرف المحدد في هذا المثيل. يبدأ البحث في موضع حرف محدد ويفحص عددًا محددًا من مواضع الأحرف. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_5)(string, int, int) | إرجاع الفهرس الصفري للتواجد الأول للسلسلة المحددة في هذا المثيل. يبدأ البحث في موضع حرف محدد ويفحص عددًا محددًا من مواضع الأحرف. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_7)(string, int, StringComparison) | إرجاع الفهرس الصفري للتواجد الأول للسلسلة المحددة في المثيل الحالي. تحدد المعلمات موضع بدء البحث في السلسلة الحالية ونوع البحث المراد استخدامه للسلسلة المحددة. |
| [IndexOf](../../aspose.note/richtext/indexof#indexof_6)(string, int, int, StringComparison) | إرجاع الفهرس الصفري للتواجد الأول للسلسلة المحددة في المثيل الحالي. |
| [Insert](../../aspose.note/richtext/insert#insert)(int, string) | لإدراج سلسلة محددة في موضع فهرس محدد في هذه الحالة. |
| [Insert](../../aspose.note/richtext/insert#insert_1)(int, string, TextStyle) | لإدراج سلسلة محددة بنمط محدد في موضع فهرس محدد في هذه الحالة. |
| [Remove](../../aspose.note/richtext/remove#remove)(int) | يزيل جميع الأحرف في المثال الحالي ، بدءًا من الموضع المحدد ويستمر حتى آخر موضع. |
| [Remove](../../aspose.note/richtext/remove#remove_1)(int, int) | يزيل عددًا محددًا من الأحرف في المثيل الحالي الذي يبدأ من الموضع المحدد. |
| [Replace](../../aspose.note/richtext/replace#replace)(char, char) | يستبدل جميع تكرارات حرف Unicode المحدد في هذه الحالة بحرف Unicode آخر محدد. |
| [Replace](../../aspose.note/richtext/replace#replace_1)(string, string) | يستبدل كل تكرارات سلسلة محددة في المثيل الحالي بسلسلة أخرى محددة. |
| [Replace](../../aspose.note/richtext/replace#replace_2)(string, string, TextStyle) | يستبدل كل تكرارات سلسلة محددة في المثيل الحالي بسلسلة أخرى محددة في النمط المحدد. |
| [Trim](../../aspose.note/richtext/trim#trim)() | يزيل كل أحرف المسافات البيضاء البادئة واللاحقة . |
| [Trim](../../aspose.note/richtext/trim#trim_1)(char) | يزيل كافة المثيلات السابقة والتابعة للحرف. |
| [Trim](../../aspose.note/richtext/trim#trim_2)(params char[]) | يزيل كل التكرارات السابقة والتالية لمجموعة من الأحرف المحددة في مصفوفة. |
| [TrimEnd](../../aspose.note/richtext/trimend#trimend)() | يزيل كل أحرف المسافات البيضاء اللاحقة. |
| [TrimEnd](../../aspose.note/richtext/trimend#trimend_1)(char) | يزيل كل التكرارات اللاحقة للحرف. |
| [TrimEnd](../../aspose.note/richtext/trimend#trimend_2)(params char[]) | يزيل كل التكرارات اللاحقة لمجموعة من الأحرف المحددة في مصفوفة. |
| [TrimStart](../../aspose.note/richtext/trimstart#trimstart)() | يزيل كافة أحرف المسافات البيضاء البادئة . |
| [TrimStart](../../aspose.note/richtext/trimstart#trimstart_1)(char) | يزيل جميع التكرارات البادئة للحرف المحدد. |
| [TrimStart](../../aspose.note/richtext/trimstart#trimstart_2)(params char[]) | يزيل كل التكرارات البادئة لمجموعة من الأحرف المحددة في مصفوفة. |

### أمثلة

يوضح كيفية الحصول على كل النص من المستند.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Text();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "Aspose.one");

// استرداد النص
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// طباعة النص على شاشة الإخراج
Console.WriteLine(text);
```

يوضح كيفية الحصول على كل النص من الصفحة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Text();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "Aspose.one");

// احصل على قائمة بعقد الصفحة
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // استرداد النص
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // طباعة النص على شاشة الإخراج
    Console.WriteLine(text);
}
```

دعنا نبرز عناوين الصفحة بين الرؤوس الأخرى عن طريق زيادة حجم الخط.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// قم بتحميل المستند في Aspose.
Document document = new Document(dataDir + "Aspose.one");

// تكرار من خلال عناوين الصفحة.
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

يوضح كيفية الحصول على نص من صف كل جدول.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tables();

// قم بتحميل المستند في Aspose.
Document document = new Document(dataDir + "Sample1.one");

// احصل على قائمة بعقد الجدول
IList<Table> nodes = document.GetChildNodes<Table>();

foreach (Table table in nodes)
{
    // التكرار خلال صفوف الجدول
    foreach (TableRow row in table)
    {
        // استرداد النص
        string text = string.Join(Environment.NewLine, row.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

        // طباعة النص على شاشة الإخراج
        Console.WriteLine(text);
    }
}
```

يوضح كيفية الحصول على نص من جدول.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tables();

// قم بتحميل المستند في Aspose.
Document document = new Document(dataDir + "Sample1.one");

// احصل على قائمة بعقد الجدول
IList<Table> nodes = document.GetChildNodes<Table>();

// تعيين عدد الجدول
int tblCount = 0;

foreach (Table table in nodes)
{
    tblCount++;
    Console.WriteLine("table # " + tblCount);

    // استرداد النص
    string text = string.Join(Environment.NewLine, table.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

    // طباعة النص على شاشة الإخراج
    Console.WriteLine(text);
}
```

دعنا نؤكد على التغييرات الأخيرة في النص من خلال التمييز.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// قم بتحميل المستند في Aspose.
Document document = new Document(dataDir + "Aspose.one");

// Get RichText عُدلت الأسبوع الماضي.
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

تعيين لغة التدقيق للنص.

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

التلاعب بتنسيق النص باستخدام نمط الفقرة.

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

يوضح كيفية الحصول على نص من خلايا الجدول.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tables();

// قم بتحميل المستند في Aspose.
Document document = new Document(dataDir + "Sample1.one");

// احصل على قائمة بعقد الجدول
IList<Table> nodes = document.GetChildNodes<Table>();        

foreach (Table table in nodes)
{
    // التكرار خلال صفوف الجدول
    foreach (TableRow row in table)
    {
        // احصل على قائمة بعقد TableCell
        // التكرار من خلال خلايا الجدول
        foreach (TableCell cell in row)
        {
            // استرداد النص
            string text = string.Join(Environment.NewLine, cell.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

            // طباعة النص على شاشة الإخراج
            Console.WriteLine(text);
        }
    }
}
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

يوضح كيفية إضافة فقرة جديدة بعلامة.

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
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
RichText text = new RichText(doc) { Text = "OneNote text.", ParagraphStyle = textStyle };
text.Tags.Add(NoteTag.CreateYellowStar());

// أضف عقدة نصية
outlineElem.AppendChildLast(text);

// إضافة عقدة عنصر المخطط التفصيلي
outline.AppendChildLast(outlineElem);

// إضافة عقدة المخطط التفصيلي
page.AppendChildLast(outline);

// إضافة عقدة الصفحة
doc.AppendChildLast(page);

// حفظ مستند OneNote
dataDir = dataDir + "AddTextNodeWithTag_out.one";
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

يوضح كيفية الوصول إلى تفاصيل العلامة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// قم بتحميل المستند في Aspose.
Document oneFile = new Document(dataDir + "TagFile.one");

// احصل على جميع عقد RichText
IList<RichText> nodes = oneFile.GetChildNodes<RichText>();

// كرر خلال كل عقدة
foreach (RichText richText in nodes)
{
    var tags = richText.Tags.OfType<NoteTag>();
    if (tags.Any())
    {
        Console.WriteLine($"Text: {richText.Text}");
        foreach (var noteTag in tags)
        {
            // استرداد الخصائص
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

يوضح كيفية تحضير قالب للاجتماع الأسبوعي.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// إنشاء كائن من فئة المستند
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

### أنظر أيضا

* class [Node](../node)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode)
* interface [ITaggable](../itaggable)
* مساحة الاسم [Aspose.Note](../../aspose.note)
* المجسم [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
