---
title: Document.Document
second_title: Aspose.Note untuk Referensi .NET API
description: Document konstruktor. Menginisialisasi instance baru dariDocument class. Membuat dokumen OneNote kosong.
type: docs
weight: 10
url: /id/net/aspose.note/document/document/
---
## Document() {#constructor}

Menginisialisasi instance baru dari[`Document`](../) class. Membuat dokumen OneNote kosong.

```csharp
public Document()
```

### Lihat juga

* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)

---

## Document(string) {#constructor_3}

Menginisialisasi instance baru dari[`Document`](../) class. Membuka dokumen OneNote yang sudah ada dari file.

```csharp
public Document(string filePath)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| filePath | String | Jalur file. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | Format dokumen tidak dikenal atau tidak didukung. |
| [FileCorruptedException](../../filecorruptedexception/) | Dokumen tampaknya rusak dan tidak dapat dimuat. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | Dokumen dienkripsi dan membutuhkan kata sandi untuk dibuka, tetapi Anda memberikan kata sandi yang salah. |
| InvalidOperationException | Ada masalah dengan dokumen tersebut dan harus dilaporkan ke pengembang Aspose.Note. |
| IOException | Ada pengecualian input/output. |

### Lihat juga

* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)

---

## Document(string, LoadOptions) {#constructor_4}

Menginisialisasi instance baru dari[`Document`](../)class. Membuka dokumen OneNote yang sudah ada dari file. Memungkinkan untuk menentukan opsi tambahan seperti kata sandi enkripsi.

```csharp
public Document(string filePath, LoadOptions loadOptions)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| filePath | String | Jalur file. |
| loadOptions | LoadOptions | Opsi yang digunakan untuk memuat dokumen. Bisa null. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | Format dokumen tidak dikenal atau tidak didukung. |
| [FileCorruptedException](../../filecorruptedexception/) | Dokumen tampaknya rusak dan tidak dapat dimuat. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | Dokumen dienkripsi dan membutuhkan kata sandi untuk dibuka, tetapi Anda memberikan kata sandi yang salah. |
| InvalidOperationException | Ada masalah dengan dokumen tersebut dan harus dilaporkan ke pengembang Aspose.Note. |
| IOException | Ada pengecualian input/output. |

### Lihat juga

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)

---

## Document(Stream) {#constructor_1}

Menginisialisasi instance baru dari[`Document`](../) class. Membuka dokumen OneNote yang sudah ada dari aliran.

```csharp
public Document(Stream inStream)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| inStream | Stream | Arus. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | Format dokumen tidak dikenal atau tidak didukung. |
| [FileCorruptedException](../../filecorruptedexception/) | Dokumen tampaknya rusak dan tidak dapat dimuat. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | Dokumen dienkripsi dan membutuhkan kata sandi untuk dibuka, tetapi Anda memberikan kata sandi yang salah. |
| InvalidOperationException | Ada masalah dengan dokumen tersebut dan harus dilaporkan ke pengembang Aspose.Note. |
| IOException | Ada pengecualian input/output. |
| ArgumentException | Aliran tidak mendukung pembacaan, nihil, atau sudah ditutup. |

### Lihat juga

* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)

---

## Document(Stream, LoadOptions) {#constructor_2}

Menginisialisasi instance baru dari[`Document`](../) class. Membuka dokumen OneNote yang sudah ada dari aliran. Memungkinkan untuk menentukan opsi tambahan seperti kata sandi enkripsi.

```csharp
public Document(Stream inStream, LoadOptions loadOptions)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| inStream | Stream | Arus. |
| loadOptions | LoadOptions | Opsi yang digunakan untuk memuat dokumen. Bisa null. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | Format dokumen tidak dikenal atau tidak didukung. |
| [FileCorruptedException](../../filecorruptedexception/) | Dokumen tampaknya rusak dan tidak dapat dimuat. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | Dokumen dienkripsi dan membutuhkan kata sandi untuk dibuka, tetapi Anda memberikan kata sandi yang salah. |
| InvalidOperationException | Ada masalah dengan dokumen tersebut dan harus dilaporkan ke pengembang Aspose.Note. |
| IOException | Ada pengecualian input/output. |
| ArgumentException | Aliran tidak mendukung pembacaan, nihil, atau sudah ditutup. |

### Lihat juga

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)


