---
title: RichText.Replace
second_title: Aspose.Note untuk Referensi .NET API
description: RichText metode. Menggantikan semua kemunculan karakter Unicode tertentu dalam contoh ini dengan karakter Unicode lain yang ditentukan.
type: docs
weight: 200
url: /id/net/aspose.note/richtext/replace/
---
## Replace(char, char) {#replace}

Menggantikan semua kemunculan karakter Unicode tertentu dalam contoh ini dengan karakter Unicode lain yang ditentukan.

```csharp
public RichText Replace(char oldChar, char newChar)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| oldChar | Char | Karakter lama. |
| newChar | Char | Karakter baru. |

### Nilai Pengembalian

Itu[`RichText`](../) .

### Lihat juga

* class [RichText](../)
* ruang nama [Aspose.Note](../../richtext/)
* perakitan [Aspose.Note](../../../)

---

## Replace(string, string) {#replace_1}

Menggantikan semua kemunculan string tertentu dalam contoh saat ini dengan string lain yang ditentukan.

```csharp
public RichText Replace(string oldValue, string newValue)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| oldValue | String | Nilai lama. |
| newValue | String | Nilai baru. |

### Nilai Pengembalian

Itu[`RichText`](../) .

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### Contoh

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

Memperlihatkan cara membuat dokumen baru dengan mengganti potongan teks khusus dalam sebuah template.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

var D = new Dictionary<string, string>
            {
                { "Company", "Atlas Shrugged Ltd" },
                { "CandidateName", "John Galt" },
                { "JobTitle", "Chief Entrepreneur Officer" },
                { "Department", "Sales" },
                { "Salary", "123456 USD" },
                { "Vacation", "30" },
                { "StartDate", "29 Feb 2024" },
                { "YourName", "Ayn Rand" }
            };

// Muat dokumen template ke Aspose.Note.
var d = new Document(Path.Combine(dataDir, "JobOffer.one"));

// Ayo ganti semua kata template
foreach (var e in d.GetChildNodes<RichText>())
{
    foreach (var replace in D)
    {
        e.Replace($"${{{replace.Key}}}", replace.Value);
    }
}

d.Save(Path.Combine(dataDir, "JobOffer_out.one"));
```

### Lihat juga

* class [RichText](../)
* ruang nama [Aspose.Note](../../richtext/)
* perakitan [Aspose.Note](../../../)

---

## Replace(string, string, TextStyle) {#replace_2}

Menggantikan semua kemunculan string yang ditentukan dalam contoh saat ini dengan string lain yang ditentukan dalam gaya yang ditentukan.

```csharp
public RichText Replace(string oldValue, string newValue, TextStyle style)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| oldValue | String | Nilai lama. |
| newValue | String | Nilai baru. |
| style | TextStyle | Gaya nilai baru. |

### Nilai Pengembalian

Itu[`RichText`](../) .

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### Lihat juga

* class [TextStyle](../../textstyle/)
* class [RichText](../)
* ruang nama [Aspose.Note](../../richtext/)
* perakitan [Aspose.Note](../../../)


