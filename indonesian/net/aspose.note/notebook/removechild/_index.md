---
title: Notebook.RemoveChild
second_title: Aspose.Note untuk Referensi .NET API
description: Notebook metode. Menghapus simpul anak.
type: docs
weight: 140
url: /id/net/aspose.note/notebook/removechild/
---
## Notebook.RemoveChild method

Menghapus simpul anak.

```csharp
public INotebookChildNode RemoveChild(INotebookChildNode oldChild)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| oldChild | INotebookChildNode | Simpul yang akan dihapus. |

### Nilai Pengembalian

Node yang dihapus.

### Contoh

Memperlihatkan cara mengakses semua bagian dari buku catatan.

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

Menunjukkan cara menyimpan buku catatan.

```csharp
// Jalur ke direktori dokumen.
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

### Lihat juga

* interface [INotebookChildNode](../../inotebookchildnode/)
* class [Notebook](../)
* ruang nama [Aspose.Note](../../notebook/)
* perakitan [Aspose.Note](../../../)


