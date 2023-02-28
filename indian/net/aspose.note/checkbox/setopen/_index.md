---
title: CheckBox.SetOpen
second_title: Aspose.Note .NET API संदर्भ के लिए
description: CheckBox तरक. टैग क ओपन स्टेट पर सेट करत है
type: docs
weight: 80
url: /hi/net/aspose.note/checkbox/setopen/
---
## CheckBox.SetOpen method

टैग को ओपन स्टेट पर सेट करता है।

```csharp
public virtual void SetOpen()
```

### उदाहरण

दिखाता है कि 'प्रोजेक्ट सी' से संबंधित सभी चेकबॉक्स आइटम कैसे खोलें।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_Tags();

// दस्तावेज़ को Aspose.Note में लोड करें।
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

### यह सभी देखें

* class [CheckBox](../)
* नाम स्थान [Aspose.Note](../../checkbox/)
* सभा [Aspose.Note](../../../)


