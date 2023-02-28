---
title: Page.GetChildNodes
second_title: Aspose.Note untuk Referensi .NET API
description: Page metode. Dapatkan semua node turunan halaman berdasarkan jenis node.
type: docs
weight: 150
url: /id/net/aspose.note/page/getchildnodes/
---
## Page.GetChildNodes&lt;T1&gt; method

Dapatkan semua node turunan halaman berdasarkan jenis node.

```csharp
public override List<T1> GetChildNodes<T1>()
    where T1 : class, INode
```

| Parameter | Keterangan |
| --- | --- |
| T1 | Jenis elemen dalam daftar yang dikembalikan. |

### Nilai Pengembalian

Daftar node anak.

### Contoh

Menunjukkan cara mendapatkan semua teks dari dokumen.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Text();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Mengambil teks
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// Cetak teks pada layar keluaran
Console.WriteLine(text);
```

Menunjukkan cara mendapatkan semua teks dari halaman.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Text();

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Dapatkan daftar node halaman
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // Mengambil teks
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // Cetak teks pada layar keluaran
    Console.WriteLine(text);
}
```

Menunjukkan cara melewati semua halaman dan membuat penggantian dalam teks.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Dapatkan semua node RichText
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Ganti teks bentuk
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// Simpan ke format file apa pun yang didukung
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Menunjukkan cara melewati teks halaman dan membuat pengganti.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// Muat dokumen ke Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// Dapatkan semua node RichText
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Ganti teks bentuk
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// Simpan ke format file apa pun yang didukung
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

### Lihat juga

* interface [INode](../../inode/)
* class [Page](../)
* ruang nama [Aspose.Note](../../page/)
* perakitan [Aspose.Note](../../../)


