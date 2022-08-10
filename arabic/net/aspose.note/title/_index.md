---
title: Title
second_title: Aspose.Note لمرجع NET API
description: يمثل عنوانًا .
type: docs
weight: 950
url: /ar/net/aspose.note/title/
---
## Title class

يمثل عنوانًا .

```csharp
public sealed class Title : CompositeNodeBase, ICompositeNode<RichText>, IPageChildNode
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [Title](title#constructor)() | يقوم بتهيئة مثيل جديد لملف[`Title`](../title) فئة . |

## الخصائص

| اسم | وصف |
| --- | --- |
| [Document](../../aspose.note/node/document) { get; } | يحصل على مستند العقدة . |
| [HorizontalOffset](../../aspose.note/title/horizontaloffset) { get; set; } | الحصول على أو تعيين الإزاحة الأفقية. |
| override [IsComposite](../../aspose.note/title/iscomposite) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه العقدة مركبة. إذا كان هذا صحيحًا ، يمكن أن تحتوي العقدة على عقد فرعية. |
| [LastModifiedTime](../../aspose.note/title/lastmodifiedtime) { get; set; } | الحصول على أو تعيين وقت آخر تعديل. |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | الحصول على العقدة التالية على نفس مستوى شجرة العقدة. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | يحصل على نوع العقدة . |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | يحصل على العقدة الأصلية . |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | الحصول على العقدة السابقة على نفس مستوى شجرة العقدة. |
| [TitleDate](../../aspose.note/title/titledate) { get; set; } | الحصول على أو تعيين سلسلة تمثيل التاريخ في العنوان. |
| [TitleText](../../aspose.note/title/titletext) { get; set; } | الحصول على نص العنوان أو تحديده. |
| [TitleTime](../../aspose.note/title/titletime) { get; set; } | الحصول على أو تعيين سلسلة تمثيل للوقت في العنوان. |
| [VerticalOffset](../../aspose.note/title/verticaloffset) { get; set; } | الحصول على أو تعيين الإزاحة الرأسية . |

## طُرق

| اسم | وصف |
| --- | --- |
| override [Accept](../../aspose.note/title/accept)(DocumentVisitor) | يقبل زائر العقدة . |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/title/getchildnodes#getchildnodes_1)() | احصل على جميع العقد الفرعية حسب نوع العقدة . |
| [GetEnumerator](../../aspose.note/title/getenumerator)() | إرجاع العداد الذي يتكرر خلال العقد التابعة لملف[`Title`](../title) . |

### أمثلة

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

### أنظر أيضا

* class [CompositeNodeBase](../compositenodebase)
* interface [ICompositeNode&lt;T&gt;](../icompositenode-1)
* class [RichText](../richtext)
* interface [IPageChildNode](../ipagechildnode)
* مساحة الاسم [Aspose.Note](../../aspose.note)
* المجسم [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
