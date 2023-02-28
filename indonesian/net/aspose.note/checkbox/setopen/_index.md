---
title: CheckBox.SetOpen
second_title: Aspose.Note untuk Referensi .NET API
description: CheckBox metode. Mengatur tag ke status terbuka.
type: docs
weight: 80
url: /id/net/aspose.note/checkbox/setopen/
---
## CheckBox.SetOpen method

Mengatur tag ke status terbuka.

```csharp
public virtual void SetOpen()
```

### Contoh

Menunjukkan cara membuka semua item kotak centang yang terkait dengan 'Project C'.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Tags();

// Muat dokumen ke Aspose.Note.
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

### Lihat juga

* class [CheckBox](../)
* ruang nama [Aspose.Note](../../checkbox/)
* perakitan [Aspose.Note](../../../)


