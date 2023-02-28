---
title: Notebook.DisplayName
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Notebook संपत्त. प्रदर्शन नम प्रप्त य सेट करत है
type: docs
weight: 40
url: /hi/net/aspose.note/notebook/displayname/
---
## Notebook.DisplayName property

प्रदर्शन नाम प्राप्त या सेट करता है।

```csharp
public string DisplayName { get; set; }
```

### उदाहरण

दिखाता है कि किसी नोटबुक से किसी अनुभाग को कैसे निकालना है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
string dataDir = RunExamples.GetDataDir_NoteBook();

// एक OneNote नोटबुक लोड करें
var notebook = new Notebook(dataDir + "test.onetoc2");

// वांछित चाइल्ड आइटम को खोजने के लिए उसके चाइल्ड नोड के माध्यम से ट्रैवर्स करें
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // चाइल्ड आइटम को नोटबुक से निकालें
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// नोटबुक को सेव करें
notebook.Save(dataDir);
```

### यह सभी देखें

* class [Notebook](../)
* नाम स्थान [Aspose.Note](../../notebook/)
* सभा [Aspose.Note](../../../)


