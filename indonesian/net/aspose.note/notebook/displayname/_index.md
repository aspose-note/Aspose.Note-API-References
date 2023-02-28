---
title: Notebook.DisplayName
second_title: Aspose.Note untuk Referensi .NET API
description: Notebook Properti. Mendapat atau menyetel nama tampilan.
type: docs
weight: 40
url: /id/net/aspose.note/notebook/displayname/
---
## Notebook.DisplayName property

Mendapat atau menyetel nama tampilan.

```csharp
public string DisplayName { get; set; }
```

### Contoh

Memperlihatkan cara menghapus bagian dari buku catatan.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Muat Buku Catatan OneNote
var notebook = new Notebook(dataDir + "test.onetoc2");

// Telusuri node anaknya untuk mencari item anak yang diinginkan
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // Hapus Item Anak dari Notebook
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// Simpan Buku Catatan
notebook.Save(dataDir);
```

### Lihat juga

* class [Notebook](../)
* ruang nama [Aspose.Note](../../notebook/)
* perakitan [Aspose.Note](../../../)


