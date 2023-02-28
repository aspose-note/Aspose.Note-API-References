---
title: License.SetLicense
second_title: Aspose.Note untuk Referensi .NET API
description: License metode. Lisensi komponen.
type: docs
weight: 20
url: /id/net/aspose.note/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Lisensi komponen.

```csharp
public void SetLicense(string licenseName)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| licenseName | String | Dapat berupa nama file lengkap atau pendek atau nama sumber daya tersemat. Gunakan string kosong untuk beralih ke mode evaluasi. |

### Perkataan

Mencoba menemukan lisensi di lokasi berikut:

1. Jalur eksplisit.

2. Folder yang berisi rakitan komponen Aspose.

3. Folder yang berisi rakitan panggilan klien.

4. Folder yang berisi rakitan entri (startup).

5. Sumber daya tertanam dalam perakitan panggilan klien.

**Catatan:**Di .NET Compact Framework, mencoba menemukan lisensi hanya di lokasi berikut:

1. Jalur eksplisit.

2. Sumber daya tertanam dalam perakitan panggilan klien.

### Contoh

Menunjukkan cara memuat lisensi untuk Aspose.Note dari file.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
license.SetLicense("Aspose.Note.lic");
```

Menunjukkan cara memuat lisensi untuk Aspose.Note dari sumber file tersemat.

```csharp
// Instansiasi kelas Lisensi
Aspose.Note.License license = new Aspose.Note.License();

// Berikan hanya nama file lisensi yang disematkan di rakitan
license.SetLicense("Aspose.Note.lic");
```

### Lihat juga

* class [License](../)
* ruang nama [Aspose.Note](../../license/)
* perakitan [Aspose.Note](../../../)

---

## SetLicense(Stream) {#setlicense}

Lisensi komponen.

```csharp
public void SetLicense(Stream stream)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| stream | Stream | Aliran yang berisi lisensi. |

### Perkataan

Gunakan metode ini untuk memuat lisensi dari aliran.

### Contoh

Menunjukkan cara memuat lisensi untuk Aspose.Note dari aliran.

```csharp
Aspose.Note.License license = new Aspose.Note.License();
using (FileStream myStream = new FileStream("Aspose.Note.lic", FileMode.Open))
{
    license.SetLicense(myStream);
}
```

### Lihat juga

* class [License](../)
* ruang nama [Aspose.Note](../../license/)
* perakitan [Aspose.Note](../../../)


