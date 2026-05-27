---
title: "Notebook.DisplayName"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "خاصية Notebook. تحصل أو تعين اسم العرض"
type: docs
weight: 40
url: /ar/net/aspose.note/notebook/displayname/
---
## Notebook.DisplayName property

يحصل أو يضبط اسم العرض.

```csharp
public string DisplayName { get; set; }
```

## أمثلة

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

### انظر أيضًا

* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)


