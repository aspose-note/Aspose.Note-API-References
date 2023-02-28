---
title: Document.IsEncrypted
second_title: Aspose.Note untuk Referensi .NET API
description: Document metode. Memeriksa apakah dokumen dari aliran dienkripsi. Untuk memeriksanya kita perlu memuat dokumen ini sepenuhnya. Jadi metode ini dapat menyebabkan penalti kinerja.
type: docs
weight: 150
url: /id/net/aspose.note/document/isencrypted/
---
## IsEncrypted(Stream, LoadOptions, out Document) {#isencrypted_1}

Memeriksa apakah dokumen dari aliran dienkripsi. Untuk memeriksanya, kita perlu memuat dokumen ini sepenuhnya. Jadi metode ini dapat menyebabkan penalti kinerja.

```csharp
public static bool IsEncrypted(Stream stream, LoadOptions options, out Document document)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| stream | Stream | Arus. |
| options | LoadOptions | Opsi pemuatan. |
| document | Document& | Dokumen yang dimuat. |

### Nilai Pengembalian

Mengembalikan true jika dokumen dienkripsi sebaliknya false.

### Contoh

Menunjukkan cara memeriksa apakah dokumen dilindungi kata sandi.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Menunjukkan cara memeriksa apakah dokumen dilindungi kata sandi dengan kata sandi tertentu.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Lihat juga

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)

---

## IsEncrypted(Stream, string, out Document) {#isencrypted_2}

Memeriksa apakah dokumen dari aliran dienkripsi. Untuk memeriksanya, kita perlu memuat dokumen ini sepenuhnya. Jadi metode ini dapat menyebabkan penalti kinerja.

```csharp
public static bool IsEncrypted(Stream stream, string password, out Document document)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| stream | Stream | Arus. |
| password | String | Kata sandi untuk mendekripsi dokumen. |
| document | Document& | Dokumen yang dimuat. |

### Nilai Pengembalian

Mengembalikan true jika dokumen dienkripsi sebaliknya false.

### Contoh

Menunjukkan cara memeriksa apakah dokumen dilindungi kata sandi.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Menunjukkan cara memeriksa apakah dokumen dilindungi kata sandi dengan kata sandi tertentu.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Lihat juga

* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)

---

## IsEncrypted(Stream, out Document) {#isencrypted}

Memeriksa apakah dokumen dari aliran dienkripsi. Untuk memeriksanya, kita perlu memuat dokumen ini sepenuhnya. Jadi metode ini dapat menyebabkan penalti kinerja.

```csharp
public static bool IsEncrypted(Stream stream, out Document document)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| stream | Stream | Arus. |
| document | Document& | Dokumen yang dimuat. |

### Nilai Pengembalian

Mengembalikan true jika dokumen dienkripsi sebaliknya false.

### Contoh

Menunjukkan cara memeriksa apakah dokumen dilindungi kata sandi.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Menunjukkan cara memeriksa apakah dokumen dilindungi kata sandi dengan kata sandi tertentu.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Lihat juga

* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)

---

## IsEncrypted(string, LoadOptions, out Document) {#isencrypted_4}

Memeriksa apakah dokumen dari file dienkripsi. Untuk memeriksanya, kita perlu memuat dokumen ini sepenuhnya. Jadi metode ini dapat menyebabkan penalti kinerja.

```csharp
public static bool IsEncrypted(string filePath, LoadOptions options, out Document document)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| filePath | String | Jalur file. |
| options | LoadOptions | Opsi pemuatan. |
| document | Document& | Dokumen yang dimuat. |

### Nilai Pengembalian

Mengembalikan true jika dokumen dienkripsi sebaliknya false.

### Contoh

Menunjukkan cara memeriksa apakah dokumen dilindungi kata sandi.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Menunjukkan cara memeriksa apakah dokumen dilindungi kata sandi dengan kata sandi tertentu.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Lihat juga

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)

---

## IsEncrypted(string, out Document) {#isencrypted_3}

Memeriksa apakah dokumen dari file dienkripsi. Untuk memeriksanya, kita perlu memuat dokumen ini sepenuhnya. Jadi metode ini dapat menyebabkan penalti kinerja.

```csharp
public static bool IsEncrypted(string filePath, out Document document)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| filePath | String | Jalur file. |
| document | Document& | Dokumen yang dimuat. |

### Nilai Pengembalian

Mengembalikan true jika dokumen dienkripsi sebaliknya false.

### Contoh

Menunjukkan cara memeriksa apakah dokumen dilindungi kata sandi.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Menunjukkan cara memeriksa apakah dokumen dilindungi kata sandi dengan kata sandi tertentu.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Lihat juga

* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)

---

## IsEncrypted(string, string, out Document) {#isencrypted_5}

Memeriksa apakah dokumen dari file dienkripsi. Untuk memeriksanya, kita perlu memuat dokumen ini sepenuhnya. Jadi metode ini dapat menyebabkan penalti kinerja.

```csharp
public static bool IsEncrypted(string filePath, string password, out Document document)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| filePath | String | Jalur file. |
| password | String | Kata sandi untuk mendekripsi dokumen. |
| document | Document& | Dokumen yang dimuat. |

### Nilai Pengembalian

Mengembalikan true jika dokumen dienkripsi sebaliknya false.

### Contoh

Menunjukkan cara memeriksa apakah dokumen dilindungi kata sandi.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Menunjukkan cara memeriksa apakah dokumen dilindungi kata sandi dengan kata sandi tertentu.

```csharp
// Jalur ke direktori dokumen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Lihat juga

* class [Document](../)
* ruang nama [Aspose.Note](../../document/)
* perakitan [Aspose.Note](../../../)


