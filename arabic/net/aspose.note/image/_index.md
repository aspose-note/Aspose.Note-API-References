---
title: Class Image
second_title: Aspose.Note لمرجع NET API
description: Aspose.Note.Image فصل. يمثل صورة .
type: docs
weight: 250
url: /ar/net/aspose.note/image/
---
## Image class

يمثل صورة .

```csharp
public sealed class Image : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [Image](image/#constructor)() | يقوم بتهيئة مثيل جديد لملف`Image` فئة . |
| [Image](image/#constructor_4)(string, Stream) | يقوم بتهيئة مثيل جديد لملف`Image` فئة . |
| [Image](image/#constructor_5)(string, string, string) | يقوم بتهيئة مثيل جديد لملف`Image` فئة . |

## الخصائص

| اسم | وصف |
| --- | --- |
| [Alignment](../../aspose.note/image/alignment/) { get; set; } | الحصول على المحاذاة أو تعيينها. |
| [AlternativeTextDescription](../../aspose.note/image/alternativetextdescription/) { get; set; } | الحصول على نص بديل للصورة أو تعيينه. |
| [AlternativeTextTitle](../../aspose.note/image/alternativetexttitle/) { get; set; } | الحصول على عنوان نص بديل للصورة أو تعيينه. |
| [Bytes](../../aspose.note/image/bytes/) { get; } | يحصل على مخزن بيانات الصورة. |
| [Document](../../aspose.note/node/document/) { get; } | يحصل على وثيقة العقدة . |
| [FileName](../../aspose.note/image/filename/) { get; } | يحصل على اسم الملف. |
| [FilePath](../../aspose.note/image/filepath/) { get; } | يحصل على المسار لملف الصورة. |
| [Format](../../aspose.note/image/format/) { get; } | الحصول على تنسيق الصورة. |
| [Height](../../aspose.note/image/height/) { get; set; } | الحصول على الارتفاع أو تحديده. هذا هو الارتفاع الحقيقي للصورة في مستند MS OneNote . |
| [HorizontalOffset](../../aspose.note/image/horizontaloffset/) { get; set; } | الحصول على أو تعيين الإزاحة الأفقية. |
| [HyperlinkUrl](../../aspose.note/image/hyperlinkurl/) { get; set; } | الحصول على أو تعيين الارتباط التشعبي المرتبط بالصورة. |
| [IsBackground](../../aspose.note/image/isbackground/) { get; set; } | تحديد ما إذا كانت الصورة صورة خلفية . |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه العقدة مركبة. إذا كان هذا صحيحًا ، يمكن أن تحتوي العقدة على عقد فرعية. |
| [LastModifiedTime](../../aspose.note/image/lastmodifiedtime/) { get; set; } | الحصول على أو تعيين وقت آخر تعديل. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | الحصول على العقدة التالية على نفس مستوى شجرة العقدة. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | يحصل على نوع العقدة . |
| [OriginalHeight](../../aspose.note/image/originalheight/) { get; } | الحصول على الارتفاع الأصلي. هذا هو العرض الأصلي للصورة قبل تغيير الحجم. |
| [OriginalWidth](../../aspose.note/image/originalwidth/) { get; } | يحصل على العرض الأصلي. هذا هو العرض الأصلي للصورة قبل تغيير الحجم. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | يحصل على العقدة الأصلية . |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | الحصول على العقدة السابقة على نفس مستوى شجرة العقدة. |
| [Tags](../../aspose.note/image/tags/) { get; } | يحصل على قائمة بكافة علامات الفقرة . |
| [VerticalOffset](../../aspose.note/image/verticaloffset/) { get; set; } | الحصول على أو تعيين الإزاحة الرأسية . |
| [Width](../../aspose.note/image/width/) { get; set; } | الحصول على العرض أو تحديده. هذا هو العرض الحقيقي للصورة في مستند MS OneNote. |

## طُرق

| اسم | وصف |
| --- | --- |
| override [Accept](../../aspose.note/image/accept/)(DocumentVisitor) | يقبل زائر العقدة . |

### أمثلة

يوضح كيفية ربط ارتباط تشعبي بصورة ما.

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

يوضح كيفية الحصول على معلومات التعريف الخاصة بالصورة.

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

يوضح كيفية إضافة صورة من ملف إلى مستند بخصائص يحددها المستخدم.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Images();

// تحميل المستند من الدفق.
Document doc = new Document(dataDir + "Aspose.one");

// احصل على الصفحة الأولى من المستند.
Aspose.Note.Page page = doc.FirstChild;

// تحميل صورة من الملف.
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

### أنظر أيضا

* class [Node](../node/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* interface [ITaggable](../itaggable/)
* مساحة الاسم [Aspose.Note](../../aspose.note/)
* المجسم [Aspose.Note](../../)


