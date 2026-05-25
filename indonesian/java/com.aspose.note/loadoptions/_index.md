---
title: "LoadOptions"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Opsi yang digunakan untuk memuat dokumen."
type: docs
weight: 46
url: /id/java/com.aspose.note/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Opsi yang digunakan untuk memuat dokumen.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | Menginisialisasi instance baru dari kelas `LoadOptions`. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getDocumentPassword()](#getDocumentPassword--) | Mendapatkan atau mengatur kata sandi untuk konten dokumen yang dienkripsi. |
| [getLoadHistory()](#getLoadHistory--) | Mendapatkan atau mengatur nilai yang menunjukkan apakah pemuat dokumen harus mengabaikan riwayat. |
| [setDocumentPassword(String value)](#setDocumentPassword-java.lang.String-) | Mendapatkan atau mengatur kata sandi untuk konten dokumen yang dienkripsi. |
| [setLoadHistory(boolean value)](#setLoadHistory-boolean-) | Mendapatkan atau mengatur nilai yang menunjukkan apakah pemuat dokumen harus mengabaikan riwayat. |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Menginisialisasi instance baru dari kelas `LoadOptions`.

### getDocumentPassword() {#getDocumentPassword--}
```
public String getDocumentPassword()
```


Mendapatkan atau mengatur kata sandi untuk konten dokumen yang dienkripsi. Nilai diabaikan jika dokumen tidak dilindungi kata sandi.

**Returns:**
java.lang.String
### getLoadHistory() {#getLoadHistory--}
```
public boolean getLoadHistory()
```


Mendapatkan atau mengatur nilai yang menunjukkan apakah pemuat dokumen harus mengabaikan riwayat. Gunakan opsi ini untuk mengurangi penggunaan memori dan CPU. Nilai default adalah `true`.

**Returns:**
boolean
### setDocumentPassword(String value) {#setDocumentPassword-java.lang.String-}
```
public void setDocumentPassword(String value)
```


Mendapatkan atau mengatur kata sandi untuk konten dokumen yang dienkripsi. Nilai diabaikan jika dokumen tidak dilindungi kata sandi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String |  |

### setLoadHistory(boolean value) {#setLoadHistory-boolean-}
```
public void setLoadHistory(boolean value)
```


Mendapatkan atau mengatur nilai yang menunjukkan apakah pemuat dokumen harus mengabaikan riwayat. Gunakan opsi ini untuk mengurangi penggunaan memori dan CPU. Nilai default adalah `true`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean |  |

