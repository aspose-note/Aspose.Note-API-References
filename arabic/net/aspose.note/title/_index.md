---
title: "الفئة Title"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "الفئة Aspose.Note.Title. تمثل عنوانًا"
type: docs
weight: 1060
url: /ar/net/aspose.note/title/
---
## Title class

يمثل عنوانًا.

```csharp
public sealed class Title : CompositeNodeBase, ICompositeNode<RichText>, IPageChildNode
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [Title](title/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | يحصل على مستند العقدة. |
| [HorizontalOffset](../../aspose.note/title/horizontaloffset/) { get; set; } | يحصل أو يعيّن الإزاحة الأفقية. |
| override [IsComposite](../../aspose.note/title/iscomposite/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه العقدة مركبة. إذا كانت true يمكن للعقدة أن تحتوي على عقد فرعية. |
| [LastModifiedTime](../../aspose.note/title/lastmodifiedtime/) { get; set; } | يحصل أو يعيّن وقت آخر تعديل. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | يحصل على العقدة التالية في نفس مستوى شجرة العقد. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | يحصل على نوع العقدة. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | يحصل على العقدة الأصلية. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | يحصل على العقدة السابقة في نفس مستوى شجرة العقد. |
| [TitleDate](../../aspose.note/title/titledate/) { get; set; } | يحصل أو يعيّن تمثيلًا نصيًا للتاريخ في العنوان. |
| [TitleText](../../aspose.note/title/titletext/) { get; set; } | يحصل أو يعيّن نص العنوان. |
| [TitleTime](../../aspose.note/title/titletime/) { get; set; } | يحصل أو يعيّن تمثيلًا نصيًا للوقت في العنوان. |
| [VerticalOffset](../../aspose.note/title/verticaloffset/) { get; set; } | يحصل أو يضبط الإزاحة العمودية. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Accept](../../aspose.note/title/accept/)(DocumentVisitor) | يقبل زائر العقدة. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/title/getchildnodes/#getchildnodes_1)() | احصل على جميع عقد الطفل حسب نوع العقدة. |
| [GetEnumerator](../../aspose.note/title/getenumerator/)() | يعيد عدّادًا يتنقل عبر العقد الفرعية لـ `Title`. |

## أمثلة

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

### انظر أيضًا

* class [CompositeNodeBase](../compositenodebase/)
* interface [ICompositeNode&lt;T&gt;](../icompositenode-1/)
* class [RichText](../richtext/)
* interface [IPageChildNode](../ipagechildnode/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


