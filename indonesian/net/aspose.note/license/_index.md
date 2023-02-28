---
title: Class License
second_title: Aspose.Note untuk Referensi .NET API
description: Aspose.Note.License kelas. Menyediakan metode untuk melisensikan komponen.
type: docs
weight: 310
url: /id/net/aspose.note/license/
---
## License class

Menyediakan metode untuk melisensikan komponen.

```csharp
public class License
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [License](license/)() | Konstruktor default. |

## Metode

| Nama | Keterangan |
| --- | --- |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense)(Stream) | Lisensi komponen. |
| [SetLicense](../../aspose.note/license/setlicense/#setlicense_1)(string) | Lisensi komponen. |

### Contoh

Menunjukkan cara memuat lisensi untuk Aspose.Note dari file.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

Menunjukkan cara memuat lisensi untuk Aspose.Note dari aliran.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

Menunjukkan cara memuat lisensi untuk Aspose.Note dari sumber file tersemat.

```csharp
// Instansiasi kelas Lisensi
Aspose.Note.License license = new Aspose.Note.License();

// Berikan hanya nama file lisensi yang disematkan di rakitan
license.SetLicense("Aspose.Note.lic");
```

### Lihat juga

* ruang nama [Aspose.Note](../../aspose.note/)
* perakitan [Aspose.Note](../../)


