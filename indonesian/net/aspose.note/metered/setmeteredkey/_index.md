---
title: Metered.SetMeteredKey
second_title: Aspose.Note untuk Referensi .NET API
description: Metered metode. Menetapkan kunci publik dan pribadi terukur.
type: docs
weight: 30
url: /id/net/aspose.note/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Menetapkan kunci publik dan pribadi terukur.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| publicKey | String | Kunci publik. |
| privateKey | String | Kunci pribadi. |

### Perkataan

Jika Anda membeli lisensi terukur, API ini harus dipanggil saat startup aplikasi, biasanya, ini sudah cukup. Namun, jika terukur gagal mengunggah data konsumsi selama periode 24 jam, lisensi akan ditetapkan ke status evaluasi. Untuk menghindari kasus seperti itu, Anda harus secara teratur memeriksa status lisensi. Jika status evaluasi, panggil API ini lagi.

### Contoh

Menunjukkan cara menyetel lisensi terukur.

```csharp
Metered metered = new Metered();
metered.SetMeteredKey("MyPublicKey", "MyPrivateKey");

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");

// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_Pages();

// Muat dokumen OneNote dan dapatkan anak pertama           
Document document = new Document(Path.Combine(dataDir, "Aspose.one"));

document.Save(Path.Combine(dataDir, "MeteredLicense.pdf"));

Console.WriteLine($"Credit before operation: {Metered.GetConsumptionCredit():F2}");
Console.WriteLine($"Consumption quantity before operation: {Metered.GetConsumptionQuantity():F2}");
```

### Lihat juga

* class [Metered](../)
* ruang nama [Aspose.Note](../../metered/)
* perakitan [Aspose.Note](../../../)


