---
title: "Notebook.RemoveChild"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "طريقة Notebook. تُزيل العقدة الفرعية"
type: docs
weight: 140
url: /ar/net/aspose.note/notebook/removechild/
---
## Notebook.RemoveChild method

يزيل عقدة الطفل.

```csharp
public INotebookChildNode RemoveChild(INotebookChildNode oldChild)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| oldChild | INotebookChildNode | العقدة المراد إزالتها. |

### قيمة الإرجاع

العقدة التي تم إزالتها.

## أمثلة

يظهر كيفية الوصول إلى جميع الأقسام من دفتر ملاحظات.

```csharp
string inputFile = "notebook.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

Notebook rootNotebook = new Notebook(dataDir + inputFile);

IList<Document> allDocuments = rootNotebook.GetChildNodes<Document>();
foreach (Document document in allDocuments) 
{
    Console.WriteLine(document.DisplayName);
}
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

يظهر كيفية حفظ دفتر ملاحظات.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = false });

notebook.Save(dataDir + "notebook_out.onetoc2", new NotebookOneSaveOptions() { DeferredSaving = true});

if (notebook.Any())
{
    var childDocument0 = notebook[0] as Document;

    childDocument0.Save(dataDir + "Not Locked_out.one");

    var childDocument1 = notebook[1] as Document;

    childDocument1.Save(dataDir + "Locked Pass1_out.one", new OneSaveOptions() { DocumentPassword = "pass" });

    var childDocument2 = notebook[2] as Document;

    childDocument2.Save(dataDir + "Locked Pass2_out.one", new OneSaveOptions() { DocumentPassword = "pass2" });
}
```

### انظر أيضًا

* interface [INotebookChildNode](../../inotebookchildnode/)
* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)


