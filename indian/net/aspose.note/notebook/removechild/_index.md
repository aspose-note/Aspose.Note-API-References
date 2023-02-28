---
title: Notebook.RemoveChild
second_title: Aspose.Note .NET API संदर्भ के लिए
description: Notebook तरक. चइल्ड नड नकलत है.
type: docs
weight: 140
url: /hi/net/aspose.note/notebook/removechild/
---
## Notebook.RemoveChild method

चाइल्ड नोड निकालता है.

```csharp
public INotebookChildNode RemoveChild(INotebookChildNode oldChild)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| oldChild | INotebookChildNode | निकालने के लिए नोड. |

### प्रतिलाभ की मात्रा

हटाया गया नोड.

### उदाहरण

दिखाता है कि किसी नोटबुक से सभी अनुभागों तक कैसे पहुँचें।

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

दिखाता है कि नोटबुक को कैसे सहेजना है।

```csharp
// दस्तावेज़ निर्देशिका का पथ।
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

### यह सभी देखें

* interface [INotebookChildNode](../../inotebookchildnode/)
* class [Notebook](../)
* नाम स्थान [Aspose.Note](../../notebook/)
* सभा [Aspose.Note](../../../)


