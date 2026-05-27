---
title: "CheckBox.SetCompleted"
second_title: "مرجع API لـ Aspose.Note for .NET"
description: "طريقة CheckBox. تعيين العلامة إلى الحالة المكتملة"
type: docs
weight: 70
url: /ar/net/aspose.note/checkbox/setcompleted/
---
## SetCompleted(DateTime) {#setcompleted_1}

يضبط العلامة إلى حالة مكتملة.

```csharp
public void SetCompleted(DateTime completedTime)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| completedTime | DateTime | وقت الاكتمال. |

### انظر أيضًا

* class [CheckBox](../)
* namespace [Aspose.Note](../../checkbox/)
* assembly [Aspose.Note](../../../)

---

## SetCompleted() {#setcompleted}

يضبط العلامة إلى حالة مكتملة باستخدام الوقت الحالي كوقت إكمال.

```csharp
public void SetCompleted()
```

## أمثلة

يوضح كيفية إكمال جميع عناصر خانة الاختيار المتعلقة بـ 'Project C'.

```csharp
// المسار إلى دليل المستندات.
string dataDir = RunExamples.GetDataDir_Tags();

// حمّل المستند إلى Aspose.Note.
var oneFile = new Document(Path.Combine(dataDir, "ProjectNotes.one"));

foreach (var node in oneFile.GetChildNodes<ITaggable>())
{
    foreach (var checkBox in node.Tags.OfType<CheckBox>())
    {
        if (checkBox.Label.Contains("Project C") && !checkBox.Checked)
        {
            checkBox.SetCompleted();
        }
    }
}

oneFile.Save(Path.Combine(dataDir, ClosedProjectCNotesFileName));
```

### انظر أيضًا

* class [CheckBox](../)
* namespace [Aspose.Note](../../checkbox/)
* assembly [Aspose.Note](../../../)


