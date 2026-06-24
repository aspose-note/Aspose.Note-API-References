---
title: "CheckBox.SetOpen"
second_title: "مرجع API لـ Aspose.Note لـ .NET"
description: "طريقة CheckBox. يضبط العلامة إلى الحالة المفتوحة"
type: docs
weight: 80
url: /ar/net/aspose.note/checkbox/setopen/
---
## CheckBox.SetOpen method

تعيين العلامة إلى حالة مفتوحة.

```csharp
public virtual void SetOpen()
```

## أمثلة

يوضح كيفية فتح جميع عناصر خانة الاختيار المرتبطة بـ 'Project C'.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// حمّل المستند إلى Aspose.Note.
var oneFile = new Document(Path.Combine(dataDir, ClosedProjectCNotesFileName));

foreach (var node in oneFile.GetChildNodes<ITaggable>())
{
    foreach (var checkBox in node.Tags.OfType<CheckBox>())
    {
        if (checkBox.Label.Contains("Project C") && checkBox.Checked)
        {
            checkBox.SetOpen();
        }
    }
}

oneFile.Save(Path.Combine(dataDir, "ProjectNoteWithOpenProjectC.one"));
```

### انظر أيضًا

* class [CheckBox](../)
* namespace [Aspose.Note](../../checkbox/)
* assembly [Aspose.Note](../../../)


