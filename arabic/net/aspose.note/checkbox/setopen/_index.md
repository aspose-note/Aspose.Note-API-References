---
title: CheckBox.SetOpen
second_title: Aspose.Note لمرجع NET API
description: CheckBox طريقة. يعين العلامة لفتح حالة .
type: docs
weight: 80
url: /ar/net/aspose.note/checkbox/setopen/
---
## CheckBox.SetOpen method

يعين العلامة لفتح حالة .

```csharp
public virtual void SetOpen()
```

### أمثلة

يوضح كيفية فتح جميع عناصر مربعات الاختيار المتعلقة بالمشروع ج.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// قم بتحميل المستند في Aspose.
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

### أنظر أيضا

* class [CheckBox](../)
* مساحة الاسم [Aspose.Note](../../checkbox/)
* المجسم [Aspose.Note](../../../)


