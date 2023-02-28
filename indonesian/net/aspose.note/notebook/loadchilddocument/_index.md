---
title: Notebook.LoadChildDocument
second_title: Aspose.Note untuk Referensi .NET API
description: Notebook metode. Menambahkan simpul dokumen anak. Membuka dokumen OneNote yang sudah ada dari file.
type: docs
weight: 120
url: /id/net/aspose.note/notebook/loadchilddocument/
---
## LoadChildDocument(string) {#loadchilddocument_2}

Menambahkan simpul dokumen anak. Membuka dokumen OneNote yang sudah ada dari file.

```csharp
public void LoadChildDocument(string filePath)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| filePath | String | Jalur file. |

### Contoh

Menunjukkan cara memuat notebook dari aliran.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

### Lihat juga

* class [Notebook](../)
* ruang nama [Aspose.Note](../../notebook/)
* perakitan [Aspose.Note](../../../)

---

## LoadChildDocument(string, LoadOptions) {#loadchilddocument_3}

Menambahkan simpul dokumen anak. Membuka dokumen OneNote yang sudah ada dari file. Memungkinkan untuk menentukan opsi pemuatan tambahan.

```csharp
public void LoadChildDocument(string filePath, LoadOptions loadOptions)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| filePath | String | Jalur file. |
| loadOptions | LoadOptions | Opsi pemuatan. |

### Lihat juga

* class [LoadOptions](../../loadoptions/)
* class [Notebook](../)
* ruang nama [Aspose.Note](../../notebook/)
* perakitan [Aspose.Note](../../../)

---

## LoadChildDocument(Stream) {#loadchilddocument}

Menambahkan simpul dokumen anak. Membuka dokumen OneNote yang sudah ada dari aliran.

```csharp
public void LoadChildDocument(Stream stream)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| stream | Stream | Arus. |

### Contoh

Menunjukkan cara memuat notebook dari aliran.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

### Lihat juga

* class [Notebook](../)
* ruang nama [Aspose.Note](../../notebook/)
* perakitan [Aspose.Note](../../../)

---

## LoadChildDocument(Stream, LoadOptions) {#loadchilddocument_1}

Menambahkan simpul dokumen anak. Membuka dokumen OneNote yang sudah ada dari aliran. Memungkinkan untuk menentukan opsi pemuatan tambahan.

```csharp
public void LoadChildDocument(Stream stream, LoadOptions loadOptions)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| stream | Stream | Arus. |
| loadOptions | LoadOptions | Opsi pemuatan. |

### Lihat juga

* class [LoadOptions](../../loadoptions/)
* class [Notebook](../)
* ruang nama [Aspose.Note](../../notebook/)
* perakitan [Aspose.Note](../../../)


