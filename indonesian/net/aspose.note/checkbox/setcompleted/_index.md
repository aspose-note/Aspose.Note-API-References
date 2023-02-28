---
title: CheckBox.SetCompleted
second_title: Aspose.Note untuk Referensi .NET API
description: CheckBox metode. Menyetel tag ke status selesai.
type: docs
weight: 70
url: /id/net/aspose.note/checkbox/setcompleted/
---
## SetCompleted(DateTime) {#setcompleted_1}

Menyetel tag ke status selesai.

```csharp
public void SetCompleted(DateTime completedTime)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| completedTime | DateTime | Waktu selesai. |

### Lihat juga

* class [CheckBox](../)
* ruang nama [Aspose.Note](../../checkbox/)
* perakitan [Aspose.Note](../../../)

---

## SetCompleted() {#setcompleted}

Menyetel tag ke status selesai menggunakan waktu saat ini sebagai waktu selesai.

```csharp
public void SetCompleted()
```

### Contoh

Menunjukkan cara menyelesaikan semua item kotak centang yang terkait dengan 'Proyek C'.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Tags();

// Muat dokumen ke Aspose.Note.
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

### Lihat juga

* class [CheckBox](../)
* ruang nama [Aspose.Note](../../checkbox/)
* perakitan [Aspose.Note](../../../)


