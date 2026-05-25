---
title: "CheckBox"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Kelas dasar untuk tag yang dapat mengubah statusnya antara lengkap dan tidak lengkap."
type: docs
weight: 13
url: /id/java/com.aspose.note/checkbox/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended
```
public abstract class CheckBox extends TagExtended
```

Kelas dasar untuk tag yang dapat mengubah statusnya antara lengkap dan tidak lengkap.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getChecked()](#getChecked--) | Mendapatkan nilai yang menunjukkan apakah CheckBox berada dalam keadaan tercentang. |
| [getCompletedTime()](#getCompletedTime--) | Mendapatkan atau mengatur waktu selesai. |
| [getCreationTime()](#getCreationTime--) | Mendapatkan atau mengatur waktu pembuatan. |
| [getIcon()](#getIcon--) | Mendapatkan atau mengatur ikon. |
| [getStatus()](#getStatus--) | Mendapatkan atau mengatur status. |
| [setCompleted()](#setCompleted--) | Mengatur tag ke status selesai menggunakan waktu saat ini sebagai waktu selesai. |
| [setCompleted(Date completedTime)](#setCompleted-java.util.Date-) | Mengatur tag ke status selesai. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Mendapatkan atau mengatur waktu pembuatan. |
| [setOpen()](#setOpen--) | Mengatur tag ke keadaan terbuka. |
### getChecked() {#getChecked--}
```
public final boolean getChecked()
```


Mendapatkan nilai yang menunjukkan apakah CheckBox berada dalam keadaan tercentang.

**Returns:**
boolean
### getCompletedTime() {#getCompletedTime--}
```
public final Date getCompletedTime()
```


Mendapatkan atau mengatur waktu selesai.

Value: `Nullable\{DateTime\}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Mendapatkan atau mengatur waktu pembuatan.

Value: java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


Mendapatkan atau mengatur ikon.

Value: [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getStatus() {#getStatus--}
```
public final int getStatus()
```


Mendapatkan atau mengatur status.

Value: [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCompleted() {#setCompleted--}
```
public final void setCompleted()
```


Mengatur tag ke status selesai menggunakan waktu saat ini sebagai waktu selesai.

### setCompleted(Date completedTime) {#setCompleted-java.util.Date-}
```
public final void setCompleted(Date completedTime)
```


Mengatur tag ke status selesai.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| completedTime | java.util.Date | Waktu selesai. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public final void setCreationTime(Date value)
```


Mendapatkan atau mengatur waktu pembuatan.

Value: java.util.Date.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


Mengatur tag ke keadaan terbuka.

