---
title: CheckBox.SetCompleted
second_title: Aspose.Note .NET API संदर्भ के लिए
description: CheckBox तरक. टैग क पूर्ण स्थत पर सेट करत है
type: docs
weight: 70
url: /hi/net/aspose.note/checkbox/setcompleted/
---
## SetCompleted(DateTime) {#setcompleted_1}

टैग को पूर्ण स्थिति पर सेट करता है।

```csharp
public void SetCompleted(DateTime completedTime)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| completedTime | DateTime | पूर्ण समय. |

### यह सभी देखें

* class [CheckBox](../)
* नाम स्थान [Aspose.Note](../../checkbox/)
* सभा [Aspose.Note](../../../)

---

## SetCompleted() {#setcompleted}

वर्तमान समय को पूर्ण समय के रूप में उपयोग करके पूर्ण स्थिति में टैग सेट करता है।

```csharp
public void SetCompleted()
```

### उदाहरण

दिखाता है कि 'प्रोजेक्ट सी' से संबंधित सभी चेकबॉक्स आइटम को कैसे पूरा किया जाए।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tags();

// दस्तावेज़ को Aspose.Note में लोड करें।
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

### यह सभी देखें

* class [CheckBox](../)
* नाम स्थान [Aspose.Note](../../checkbox/)
* सभा [Aspose.Note](../../../)


