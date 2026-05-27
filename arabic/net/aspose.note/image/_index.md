---
title: "الفئة Image"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "الفئة Aspose.Note.Image. تمثل صورة."
type: docs
weight: 250
url: /ar/net/aspose.note/image/
---
## Image class

يمثل صورة.

```csharp
public sealed class Image : CompositeNode<Loop>, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [Image](image/#constructor)() | يُنشئ مثيلاً جديدًا للفئة `Image`. |
| [Image](image/#constructor_1)(string) | يُنشئ مثيلاً جديدًا للفئة `Image`. |
| [Image](image/#constructor_2)(string, Stream) | يُنشئ مثيلاً جديدًا للفئة `Image`. |
| [Image](image/#constructor_3)(string, string, string) | يُنشئ مثيلاً جديدًا للفئة `Image`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Alignment](../../aspose.note/image/alignment/) { get; set; } | يحصل أو يعيّن المحاذاة. |
| [AlternativeTextDescription](../../aspose.note/image/alternativetextdescription/) { get; set; } | يحصل أو يعيّن نصًا بديلًا للجسم للصورة. |
| [AlternativeTextTitle](../../aspose.note/image/alternativetexttitle/) { get; set; } | يحصل أو يعيّن عنوان النص البديل للصورة. |
| [Bytes](../../aspose.note/image/bytes/) { get; } | يحصل على مخزن بيانات الصورة. |
| [Document](../../aspose.note/node/document/) { get; } | يحصل على مستند العقدة. |
| [FileName](../../aspose.note/image/filename/) { get; } | يحصل على اسم الملف. |
| [FilePath](../../aspose.note/image/filepath/) { get; } | يحصل على المسار إلى ملف الصورة. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [Format](../../aspose.note/image/format/) { get; } | يحصل على تنسيق الصورة. |
| [Height](../../aspose.note/image/height/) { get; set; } | يحصل أو يعيّن الارتفاع. هذا هو الارتفاع الحقيقي للصورة في مستند MS OneNote. |
| [HorizontalOffset](../../aspose.note/image/horizontaloffset/) { get; set; } | يحصل أو يعيّن الإزاحة الأفقية. |
| [HyperlinkUrl](../../aspose.note/image/hyperlinkurl/) { get; set; } | يحصل أو يعيّن الرابط التشعبي المرتبط بالصورة. |
| [IsBackground](../../aspose.note/image/isbackground/) { get; set; } | يحصل على ما إذا كانت الصورة صورة خلفية. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [LastModifiedTime](../../aspose.note/image/lastmodifiedtime/) { get; set; } | يحصل أو يعيّن وقت التعديل الأخير. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | يحصل على العقدة التالية في نفس مستوى شجرة العقد. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | يحصل على نوع العقدة. |
| [OriginalHeight](../../aspose.note/image/originalheight/) { get; } | يحصل على الارتفاع الأصلي. هذا هو العرض الأصلي للصورة، قبل إعادة التحجيم. |
| [OriginalWidth](../../aspose.note/image/originalwidth/) { get; } | يحصل على العرض الأصلي. هذا هو العرض الأصلي للصورة، قبل إعادة التحجيم. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | يحصل على العقدة الأصلية. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | يحصل على العقدة السابقة في نفس مستوى شجرة العقد. |
| [Tags](../../aspose.note/image/tags/) { get; } | يحصل على قائمة جميع العلامات في الفقرة. |
| [VerticalOffset](../../aspose.note/image/verticaloffset/) { get; set; } | يحصل أو يضبط الإزاحة العمودية. |
| [Width](../../aspose.note/image/width/) { get; set; } | يحصل أو يعيّن العرض. هذا هو العرض الحقيقي للصورة في مستند MS OneNote. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Accept](../../aspose.note/image/accept/)(DocumentVisitor) | يقبل زائر العقدة. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;Loop&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params Loop[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |
| [Replace](../../aspose.note/image/replace/)(Image) | يستبدل بيانات الصورة الحالية بالبيانات من كائن Image المقدم. |

## أمثلة

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

### انظر أيضًا

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* class [Loop](../loop/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* interface [IPageChildNode](../ipagechildnode/)
* interface [ITaggable](../itaggable/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


