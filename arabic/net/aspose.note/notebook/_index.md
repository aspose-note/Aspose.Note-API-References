---
title: Notebook
second_title: Aspose.Note لمرجع NET API
description: يمثل Aspose.Note note .
type: docs
weight: 390
url: /ar/net/aspose.note/notebook/
---
## Notebook class

يمثل Aspose.Note note .

```csharp
public class Notebook : IEnumerable<INotebookChildNode>, INotebookChildNode
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [Notebook](notebook#constructor)() | يقوم بتهيئة مثيل جديد لملف[`Notebook`](../notebook) فئة . |
| [Notebook](notebook#constructor_1)(Stream) | يقوم بتهيئة مثيل جديد لملف[`Notebook`](../notebook) class. فتح دفتر ملاحظات OneNote موجود من دفق. |
| [Notebook](notebook#constructor_3)(string) | يقوم بتهيئة مثيل جديد لملف[`Notebook`](../notebook) class. فتح دفتر ملاحظات OneNote موجود من ملف. |
| [Notebook](notebook#constructor_2)(Stream, NotebookLoadOptions) | يقوم بتهيئة مثيل جديد لملف[`Notebook`](../notebook) class. يفتح دفتر ملاحظات OneNote موجود من دفق. يسمح بتحديد خيارات تحميل إضافية. |
| [Notebook](notebook#constructor_4)(string, NotebookLoadOptions) | يقوم بتهيئة مثيل جديد لملف[`Notebook`](../notebook)class. يفتح دفتر ملاحظات OneNote من ملف. يسمح بتحديد خيارات إضافية مثل استراتيجية تحميل الأطفال ("كسول" / فوري) . |

## الخصائص

| اسم | وصف |
| --- | --- |
| [Color](../../aspose.note/notebook/color) { get; set; } | الحصول على اللون أو تحديده . |
| [Count](../../aspose.note/notebook/count) { get; } | الحصول على عدد العناصر الموجودة في ملف[`Notebook`](../notebook) . |
| [DisplayName](../../aspose.note/notebook/displayname) { get; set; } | الحصول على أو تحديد اسم العرض . |
| [FileFormat](../../aspose.note/notebook/fileformat) { get; } | الحصول على تنسيق الملف (OneNote 2010 ، OneNote Online) . |
| [Guid](../../aspose.note/notebook/guid) { get; } | يحصل على معرف الكائن الفريد عالميًا . |
| [IsHistoryEnabled](../../aspose.note/notebook/ishistoryenabled) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان السجل ممكّنًا أم لا. |
| [Item](../../aspose.note/notebook/item) { get; } | يحصل على العقدة الفرعية للمفكرة بواسطة الفهرس المحدد. |

## طُرق

| اسم | وصف |
| --- | --- |
| [AppendChild](../../aspose.note/notebook/appendchild)(INotebookChildNode) | يضيف العقدة إلى نهاية القائمة. |
| [GetChildNodes&lt;T1&gt;](../../aspose.note/notebook/getchildnodes)() | احصل على جميع العقد الفرعية حسب نوع العقدة . |
| [GetEnumerator](../../aspose.note/notebook/getenumerator)() | إرجاع العداد الذي يتكرر خلال العقد التابعة لملف[`Notebook`](../notebook) . |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument)(Stream) | يضيف عقدة مستند فرعية . يفتح مستند OneNote موجود من دفق . |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_2)(string) | يضيف عقدة مستند فرعية . يفتح مستند OneNote موجود من ملف . |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_1)(Stream, LoadOptions) | يضيف عقدة مستند فرعية . يفتح مستند OneNote موجود من دفق. يسمح بتحديد خيارات تحميل إضافية. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_3)(string, LoadOptions) | يضيف عقدة مستند فرعية . يفتح مستند OneNote موجود من ملف. يسمح بتحديد خيارات تحميل إضافية. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook)(Stream) | إضافة عقدة دفتر ملاحظات فرعية . فتح دفتر ملاحظات OneNote موجود من دفق . |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_2)(string) | إضافة عقدة دفتر ملاحظات فرعية . فتح دفتر ملاحظات OneNote موجود من ملف. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_1)(Stream, NotebookLoadOptions) | يضيف عقدة دفتر ملاحظات فرعية . يفتح دفتر ملاحظات OneNote موجود من دفق. يسمح بتحديد خيارات تحميل إضافية. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_3)(string, NotebookLoadOptions) | إضافة عقدة دفتر ملاحظات فرعية . فتح دفتر ملاحظات OneNote موجود من ملف. يسمح بتحديد خيارات تحميل إضافية. |
| [RemoveChild](../../aspose.note/notebook/removechild)(INotebookChildNode) | يزيل العقدة الفرعية . |
| [Save](../../aspose.note/notebook/save#save)(Stream) | يحفظ مستند OneNote في دفق. |
| [Save](../../aspose.note/notebook/save#save_3)(string) | يحفظ مستند OneNote في ملف. |
| [Save](../../aspose.note/notebook/save#save_2)(Stream, NotebookSaveOptions) | يحفظ مستند OneNote في دفق باستخدام خيارات الحفظ المحددة. |
| [Save](../../aspose.note/notebook/save#save_1)(Stream, SaveFormat) | يحفظ مستند OneNote في دفق بالتنسيق المحدد. |
| [Save](../../aspose.note/notebook/save#save_5)(string, NotebookSaveOptions) | يحفظ مستند OneNote في ملف باستخدام خيارات الحفظ المحددة. |
| [Save](../../aspose.note/notebook/save#save_4)(string, SaveFormat) | يحفظ مستند OneNote في ملف بالتنسيق المحدد. |

### أمثلة

يوضح كيفية حفظ دفتر الملاحظات.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook();

dataDir = dataDir + "test_out.onetoc2";

// حفظ دفتر الملاحظات
notebook.Save(dataDir);
```

يوضح كيفية حفظ دفتر الملاحظات بتنسيق pdf.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر ملاحظات OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToPDF_out.pdf";

// حفظ دفتر الملاحظات
notebook.Save(dataDir);
```

يوضح كيفية حفظ دفتر الملاحظات كصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر ملاحظات OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToImage_out.png";

// حفظ دفتر الملاحظات
notebook.Save(dataDir);
```

يوضح كيفية الحصول على كل النص من دفتر ملاحظات.

```csharp
string inputFile = "notebook.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

Notebook rootNotebook = new Notebook(dataDir + inputFile);

IList<RichText> allRichTextNodes = rootNotebook.GetChildNodes<RichText>();
foreach (RichText richTextNode in allRichTextNodes)
{
    Console.WriteLine(richTextNode.Text);
}
```

يوضح كيفية حفظ دفتر ملاحظات مسطح بتنسيق pdf.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر ملاحظات OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// حفظ دفتر الملاحظات
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

يوضح كيفية التكرار من خلال مستندات جهاز كمبيوتر محمول يتم تحميلها بتكاسل.

```csharp
string inputFile = "Notizbuch öffnen.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

// افتراضيًا يتم تحميل الأطفال "كسول".
Notebook notebook = new Notebook(dataDir + inputFile);

foreach (var notebookChildNode in notebook.OfType<Document>()) 
{
    // التحميل الفعلي للمستند الفرعي يحدث هنا فقط.
    // افعل شيئًا مع المستند الفرعي
}
```

يوضح كيفية إضافة قسم جديد إلى دفتر ملاحظات.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر ملاحظات OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// إلحاق طفل جديد بدفتر الملاحظات
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// حفظ دفتر الملاحظات
notebook.Save(dataDir);
```

يوضح كيفية تحميل دفتر الملاحظات من دفق.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

يوضح كيفية عمل دفتر ملاحظات مشفر.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

يوضح كيفية حفظ دفتر الملاحظات كصورة بخيارات محددة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر ملاحظات OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// حفظ دفتر الملاحظات
notebook.Save(dataDir, notebookSaveOptions);
```

يوضح كيفية حفظ دفتر الملاحظات المسطح كصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر ملاحظات OneNote
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// حفظ دفتر الملاحظات
notebook.Save(dataDir, notebookSaveOptions);
```

يوضح كيفية إزالة قسم من دفتر ملاحظات.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر ملاحظات OneNote
var notebook = new Notebook(dataDir + "test.onetoc2");

// اجتياز العقد الفرعية للبحث عن العنصر الفرعي المطلوب
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // إزالة العنصر الفرعي من دفتر الملاحظات
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// حفظ دفتر الملاحظات
notebook.Save(dataDir);
```

يوضح كيفية التكرار من خلال المستندات المحملة مسبقًا لدفتر ملاحظات.

```csharp
// افتراضيًا يتم تحميل الأطفال "كسول".
// لذلك حدث التحميل الفوري ،
// من الضروري تعيين علامة NotebookLoadOptions.InstantLoading.
NotebookLoadOptions loadOptions = new NotebookLoadOptions { InstantLoading = true };

String inputFile = "Notizbuch öffnen.onetoc2";
String dataDir = RunExamples.GetDataDir_NoteBook();
Notebook notebook = new Notebook(dataDir + inputFile, loadOptions);

// تم تحميل كافة المستندات التابعة بالفعل.
foreach (INotebookChildNode notebookChildNode in notebook.OfType<Document>()) 
{
   // افعل شيئًا مع المستند الفرعي
}
```

يوضح كيفية المرور عبر محتوى دفتر ملاحظات.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = "Open Notebook.onetoc2";
try
{
    var notebook = new Notebook(dataDir + fileName);
    foreach (var notebookChildNode in notebook)
    {
        Console.WriteLine(notebookChildNode.DisplayName);
        if (notebookChildNode is Document)
        {
            // افعل شيئًا مع المستند الفرعي
        }
        else if (notebookChildNode is Notebook)
        {
            // افعل شيئًا باستخدام دفتر ملاحظات الأطفال
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

### أنظر أيضا

* interface [INotebookChildNode](../inotebookchildnode)
* مساحة الاسم [Aspose.Note](../../aspose.note)
* المجسم [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
