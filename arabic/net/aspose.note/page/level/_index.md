---
title: Page.Level
second_title: Aspose.Note لمرجع NET API
description: Page ملكية. الحصول على المستوى أو تحديده .
type: docs
weight: 70
url: /ar/net/aspose.note/page/level/
---
## Page.Level property

الحصول على المستوى أو تحديده .

```csharp
public byte Level { get; set; }
```

### أمثلة

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

* class [Page](../)
* مساحة الاسم [Aspose.Note](../../page/)
* المجسم [Aspose.Note](../../../)


