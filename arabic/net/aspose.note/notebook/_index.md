---
title: "فئة Notebook"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "فئة Aspose.Note.Notebook. تمثل دفتر ملاحظات Aspose.Note"
type: docs
weight: 480
url: /ar/net/aspose.note/notebook/
---
## Notebook class

يمثل دفتر ملاحظات Aspose.Note.

```csharp
public class Notebook : IEnumerable<INotebookChildNode>, INotebookChildNode
```

## المُنشئات

| الاسم | الوصف |
| --- | --- |
| [Notebook](notebook/#constructor)() | تهيئ نسخة جديدة من الفئة `Notebook`. |
| [Notebook](notebook/#constructor_1)(Stream) | تهيئ نسخة جديدة من الفئة `Notebook`. يفتح دفتر ملاحظات OneNote موجود من تدفق. |
| [Notebook](notebook/#constructor_3)(string) | تهيئ نسخة جديدة من الفئة `Notebook`. يفتح دفتر ملاحظات OneNote موجود من ملف. |
| [Notebook](notebook/#constructor_2)(Stream, NotebookLoadOptions) | تهيئ نسخة جديدة من الفئة `Notebook`. يفتح دفتر ملاحظات OneNote موجود من تدفق. يسمح بتحديد خيارات تحميل إضافية. |
| [Notebook](notebook/#constructor_4)(string, NotebookLoadOptions) | تهيئ نسخة جديدة من الفئة `Notebook`. يفتح دفتر ملاحظات OneNote موجود من ملف. يسمح بتحديد خيارات إضافية مثل استراتيجية تحميل العناصر الفرعية ("lazy"/instant). |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Color](../../aspose.note/notebook/color/) { get; set; } | يحصل أو يعيّن اللون. |
| [Count](../../aspose.note/notebook/count/) { get; } | يحصل على عدد العناصر الموجودة في `Notebook`. |
| [DisplayName](../../aspose.note/notebook/displayname/) { get; set; } | يحصل أو يضبط اسم العرض. |
| [FileFormat](../../aspose.note/notebook/fileformat/) { get; } | يحصل على تنسيق الملف (OneNote 2010، OneNote Online). |
| [Guid](../../aspose.note/notebook/guid/) { get; } | يحصل على المعرف الفريد عالميًا للكائن. |
| [IsHistoryEnabled](../../aspose.note/notebook/ishistoryenabled/) { get; set; } | يحصل أو يضبط قيمة تشير إلى ما إذا كان السجل مفعلاً. |
| [Item](../../aspose.note/notebook/item/) { get; } | يحصل على عقدة الطفل للمفكرة بالترتيب المحدد. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AppendChild](../../aspose.note/notebook/appendchild/)(INotebookChildNode) | يضيف العقدة إلى نهاية القائمة. |
| [GetChildNodes&lt;T1&gt;](../../aspose.note/notebook/getchildnodes/)() | احصل على جميع عقد الطفل حسب نوع العقدة. |
| [GetEnumerator](../../aspose.note/notebook/getenumerator/)() | يرجع عدّادًا يتنقل عبر عقد الطفل في `Notebook`. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument)(Stream) | يضيف عقدة مستند طفل. يفتح مستند OneNote موجود من تدفق. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_2)(string) | يضيف عقدة مستند طفل. يفتح مستند OneNote موجود من ملف. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_1)(Stream, LoadOptions) | يضيف عقدة مستند طفل. يفتح مستند OneNote موجود من تدفق. يسمح بتحديد خيارات تحميل إضافية. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_3)(string, LoadOptions) | يضيف عقدة مستند طفل. يفتح مستند OneNote موجود من ملف. يسمح بتحديد خيارات تحميل إضافية. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook)(Stream) | يضيف عقدة مفكرة طفل. يفتح مفكرة OneNote موجودة من تدفق. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_2)(string) | يضيف عقدة مفكرة طفل. يفتح مفكرة OneNote موجودة من ملف. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_1)(Stream, NotebookLoadOptions) | يضيف عقدة مفكرة طفل. يفتح مفكرة OneNote موجودة من تدفق. يسمح بتحديد خيارات تحميل إضافية. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_3)(string, NotebookLoadOptions) | يضيف عقدة مفكرة طفل. يفتح مفكرة OneNote موجودة من ملف. يسمح بتحديد خيارات تحميل إضافية. |
| [RemoveChild](../../aspose.note/notebook/removechild/)(INotebookChildNode) | يزيل عقدة الطفل. |
| [Save](../../aspose.note/notebook/save/#save)(Stream) | يحفظ مستند OneNote إلى تدفق. |
| [Save](../../aspose.note/notebook/save/#save_3)(string) | يحفظ مستند OneNote إلى ملف. |
| [Save](../../aspose.note/notebook/save/#save_2)(Stream, NotebookSaveOptions) | يحفظ مستند OneNote إلى تدفق باستخدام خيارات الحفظ المحددة. |
| [Save](../../aspose.note/notebook/save/#save_1)(Stream, SaveFormat) | يحفظ مستند OneNote إلى تدفق بالتنسيق المحدد. |
| [Save](../../aspose.note/notebook/save/#save_5)(string, NotebookSaveOptions) | يحفظ مستند OneNote إلى ملف باستخدام خيارات الحفظ المحددة. |
| [Save](../../aspose.note/notebook/save/#save_4)(string, SaveFormat) | يحفظ مستند OneNote إلى ملف بالتنسيق المحدد. |

## أمثلة

يعرض كيفية حفظ المفكرة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook();

dataDir = dataDir + "test_out.onetoc2";

// احفظ الدفتر
notebook.Save(dataDir);
```

يوضح كيفية حفظ الدفتر بصيغة PDF.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر OneNote
var notebook = new Notebook(dataDir + "Notebook.onetoc2");

dataDir = dataDir + "ConvertToPDF_out.pdf";

// احفظ الدفتر
notebook.Save(dataDir);
```

يوضح كيفية حفظ الدفتر كصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر OneNote
var notebook = new Notebook(dataDir + "Notebook.onetoc2");

dataDir = dataDir + "ConvertToImage_out.png";

// احفظ الدفتر
notebook.Save(dataDir);
```

يوضح كيفية استخراج كل النص من الدفتر.

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

يوضح كيفية حفظ الدفتر المسطح بصيغة PDF.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر OneNote
var notebook = new Notebook(dataDir + "Notebook.onetoc2");

// احفظ الدفتر
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

يوضح كيفية التنقل عبر مستندات الدفتر وتحميلها بشكل كسول.

```csharp
string inputFile = "Notebook.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

// بشكل افتراضي، تحميل العناصر الفرعية هو "lazy".
Notebook notebook = new Notebook(dataDir + inputFile);

foreach (var notebookChildNode in notebook.OfType<Document>()) 
{
    // يتم التحميل الفعلي للمستند الفرعي هنا فقط.
    // قم بعمل شيء مع المستند الفرعي
}
```

يوضح كيفية إضافة قسم جديد إلى الدفتر.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر OneNote
var notebook = new Notebook(dataDir + "Notebook.onetoc2");

// إلحاق عنصر فرعي جديد إلى الدفتر
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// احفظ الدفتر
notebook.Save(dataDir);
```

يوضح كيفية تحميل الدفتر من تدفق.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notebook.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

يوضح كيفية التعامل مع دفتر مشفر.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

يوضح كيفية حفظ الدفتر كصورة مع الخيارات المحددة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر OneNote
var notebook = new Notebook(dataDir + "Notebook.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// احفظ الدفتر
notebook.Save(dataDir, notebookSaveOptions);
```

يوضح كيفية حفظ الدفتر المسطح كصورة.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر OneNote
var notebook = new Notebook(dataDir + "Notebook.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// احفظ الدفتر
notebook.Save(dataDir, notebookSaveOptions);
```

يوضح كيفية إزالة قسم من الدفتر.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

// تحميل دفتر OneNote
var notebook = new Notebook(dataDir + "test.onetoc2");

// التنقل عبر العقد الفرعية للبحث عن العنصر الفرعي المطلوب
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // إزالة العنصر الفرعي من الدفتر
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// احفظ الدفتر
notebook.Save(dataDir);
```

يوضح كيفية التنقل عبر المستندات المحملة مسبقًا للدفتر.

```csharp
// بشكل افتراضي، تحميل العناصر الفرعية هو "lazy".
// لذلك، تم حدوث التحميل الفوري،
// من الضروري ضبط علامة NotebookLoadOptions.InstantLoading.
NotebookLoadOptions loadOptions = new NotebookLoadOptions { InstantLoading = true };

String inputFile = "Notebook.onetoc2";
String dataDir = RunExamples.GetDataDir_NoteBook();
Notebook notebook = new Notebook(dataDir + inputFile, loadOptions);

// جميع المستندات الفرعية تم تحميلها بالفعل.
foreach (INotebookChildNode notebookChildNode in notebook.OfType<Document>()) 
{
   // قم بعمل شيء مع المستند الفرعي
}
```

يوضح كيفية المرور عبر محتوى الدفتر.

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
            // قم بعمل شيء مع المستند الفرعي
        }
        else if (notebookChildNode is Notebook)
        {
            // قم بعمل شيء مع دفتر فرعي
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

### انظر أيضًا

* interface [INotebookChildNode](../inotebookchildnode/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


