---
title: "ITag"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Antarmuka untuk tag dari semua jenis."
type: docs
weight: 109
url: /id/java/com.aspose.note/itag/
---
```
public interface ITag
```

Antarmuka untuk tag dari semua jenis.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getCompletedTime()](#getCompletedTime--) | Mendapatkan waktu selesai. |
| [getCreationTime()](#getCreationTime--) | Mendapatkan waktu pembuatan. |
| [getIcon()](#getIcon--) | Mendapatkan ikon. |
| [getLabel()](#getLabel--) | Mendapatkan teks label. |
| [getStatus()](#getStatus--) | Mendapatkan status. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Mengatur waktu pembuatan. |
### getCompletedTime() {#getCompletedTime--}
```
public abstract Date getCompletedTime()
```


Mendapatkan waktu selesai.

Value: `Nullable\{DateTime\}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public abstract Date getCreationTime()
```


Mendapatkan waktu pembuatan.

Value: java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


Mendapatkan ikon.

Value: [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getLabel() {#getLabel--}
```
public abstract String getLabel()
```


Mendapatkan teks label.

**Returns:**
java.lang.String
### getStatus() {#getStatus--}
```
public abstract int getStatus()
```


Mendapatkan status.

Value: [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public abstract void setCreationTime(Date value)
```


Mengatur waktu pembuatan.

Value: java.util.Date.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date |  |

