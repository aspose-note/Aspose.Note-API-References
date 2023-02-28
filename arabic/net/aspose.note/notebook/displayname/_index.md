---
title: Notebook.DisplayName
second_title: Aspose.Note لمرجع NET API
description: Notebook ملكية. الحصول على أو تحديد اسم العرض .
type: docs
weight: 40
url: /ar/net/aspose.note/notebook/displayname/
---
## Notebook.DisplayName property

الحصول على أو تحديد اسم العرض .

```csharp
public string DisplayName { get; set; }
```

### أمثلة

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

### أنظر أيضا

* class [Notebook](../)
* مساحة الاسم [Aspose.Note](../../notebook/)
* المجسم [Aspose.Note](../../../)


