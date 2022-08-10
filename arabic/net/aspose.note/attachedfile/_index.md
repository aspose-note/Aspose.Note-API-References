---
title: AttachedFile
second_title: Aspose.Note لمرجع NET API
description: يمثل ملف مرفق.
type: docs
weight: 10
url: /ar/net/aspose.note/attachedfile/
---
## AttachedFile class

يمثل ملف مرفق.

```csharp
public class AttachedFile : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [AttachedFile](attachedfile#constructor)() | يقوم بتهيئة مثيل جديد لملف[`AttachedFile`](../attachedfile) فئة . |
| [AttachedFile](attachedfile#constructor_6)(string, Stream) | يقوم بتهيئة مثيل جديد لملف[`AttachedFile`](../attachedfile) فئة . |
| [AttachedFile](attachedfile#constructor_7)(string, Stream, ImageFormat) | يقوم بتهيئة مثيل جديد لملف[`AttachedFile`](../attachedfile) فئة . |
| [AttachedFile](attachedfile#constructor_8)(string, Stream, Stream, ImageFormat) | يقوم بتهيئة مثيل جديد لملف[`AttachedFile`](../attachedfile) فئة . |

## الخصائص

| اسم | وصف |
| --- | --- |
| [Alignment](../../aspose.note/attachedfile/alignment) { get; set; } | الحصول على المحاذاة أو تعيينها. |
| [AlternativeTextDescription](../../aspose.note/attachedfile/alternativetextdescription) { get; set; } | الحصول على نص بديل لأيقونة الملف المرفق أو تعيينه. |
| [AlternativeTextTitle](../../aspose.note/attachedfile/alternativetexttitle) { get; set; } | الحصول على أو تحديد عنوان نص بديل لرمز الملف المرفق. |
| [Bytes](../../aspose.note/attachedfile/bytes) { get; } | يحصل على البيانات الثنائية لملف مضمن. |
| [Document](../../aspose.note/node/document) { get; } | يحصل على مستند العقدة . |
| [Extension](../../aspose.note/attachedfile/extension) { get; } | يحصل على امتداد الملف المضمن. |
| [FileName](../../aspose.note/attachedfile/filename) { get; } | يحصل على اسم الملف المضمن. |
| [FilePath](../../aspose.note/attachedfile/filepath) { get; } | يحصل على المسار للملف الأصلي. |
| [Height](../../aspose.note/attachedfile/height) { get; } | الحصول على الارتفاع الأصلي لرمز الملف المضمن. |
| [HorizontalOffset](../../aspose.note/attachedfile/horizontaloffset) { get; set; } | الحصول على أو تعيين الإزاحة الأفقية. |
| [Icon](../../aspose.note/attachedfile/icon) { get; } | الحصول على البيانات الثنائية للرمز المرتبط بالملف المضمن. |
| [IconExtension](../../aspose.note/attachedfile/iconextension) { get; } | يحصل على امتداد الأيقونة . |
| virtual [IsComposite](../../aspose.note/node/iscomposite) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه العقدة مركبة. إذا كان هذا صحيحًا ، يمكن أن تحتوي العقدة على عقد فرعية. |
| [IsPrintout](../../aspose.note/attachedfile/isprintout) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان عرض الملف مطبوعًا. |
| [IsSizeSetByUser](../../aspose.note/attachedfile/issizesetbyuser) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا تم تحديث قيمة حجم الرمز بشكل صريح من قبل المستخدم. |
| [LastModifiedTime](../../aspose.note/attachedfile/lastmodifiedtime) { get; set; } | الحصول على أو تعيين وقت آخر تعديل. |
| [MaxHeight](../../aspose.note/attachedfile/maxheight) { get; set; } | الحصول على أو تعيين أقصى ارتفاع لعرض رمز الملف المضمن. |
| [MaxWidth](../../aspose.note/attachedfile/maxwidth) { get; set; } | الحصول على أو تعيين الحد الأقصى للعرض لعرض رمز الملف المضمن. |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | الحصول على العقدة التالية على نفس مستوى شجرة العقدة. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | يحصل على نوع العقدة . |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | يحصل على العقدة الأصلية . |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | الحصول على العقدة السابقة على نفس مستوى شجرة العقدة. |
| [Tags](../../aspose.note/attachedfile/tags) { get; } | يحصل على قائمة بكافة علامات الفقرة . |
| [Text](../../aspose.note/attachedfile/text) { get; set; } | الحصول على أو تعيين التمثيل النصي للملف المضمن. يجب ألا تحتوي السلسلة على أي أحرف بالقيمة 10 (تغذية السطر) أو 13 (إرجاع السطر) . |
| [VerticalOffset](../../aspose.note/attachedfile/verticaloffset) { get; set; } | الحصول على أو تعيين الإزاحة الرأسية . |
| [Width](../../aspose.note/attachedfile/width) { get; } | الحصول على العرض الأصلي لرمز الملف المضمن. |

## طُرق

| اسم | وصف |
| --- | --- |
| override [Accept](../../aspose.note/attachedfile/accept)(DocumentVisitor) | يقبل زائر العقدة . |

### أمثلة

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

### أنظر أيضا

* class [Node](../node)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode)
* interface [IPageChildNode](../ipagechildnode)
* interface [ITaggable](../itaggable)
* مساحة الاسم [Aspose.Note](../../aspose.note)
* المجسم [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
