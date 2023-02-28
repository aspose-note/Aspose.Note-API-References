---
title: Class Metered
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.Metered kelas. Menyediakan metode untuk menyetel kunci terukur.
type: docs
weight: 350
url: /id/net/aspose.note/metered/
---
## Metered class

Menyediakan metode untuk menyetel kunci terukur.

```csharp
public class Metered
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [Metered](metered/)() | Konstruktor default. |

## Metode

| Nama | Keterangan |
| --- | --- |
| [ResetMeteredKey](../../aspose.note/metered/resetmeteredkey/)() | Menghapus lisensi penyiapan sebelumnya. |
| [SetMeteredKey](../../aspose.note/metered/setmeteredkey/)(string, string) | Menetapkan kunci publik dan pribadi terukur. |
| static [GetConsumptionCredit](../../aspose.note/metered/getconsumptioncredit/)() | Mendapat kredit konsumsi. |
| static [GetConsumptionQuantity](../../aspose.note/metered/getconsumptionquantity/)() | Mendapat ukuran file konsumsi. |

### Contoh

Dalam contoh ini, upaya akan dilakukan untuk menyetel kunci publik dan pribadi terukur

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

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

* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


