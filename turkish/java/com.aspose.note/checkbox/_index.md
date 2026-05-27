---
title: "CheckBox"
second_title: "Aspose.Note for Java API Referansı"
description: "Tamamlanmış ve tamamlanmamış durumlar arasında geçiş yapabilen etiketler için temel sınıf."
type: docs
weight: 13
url: /tr/java/com.aspose.note/checkbox/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended
```
public abstract class CheckBox extends TagExtended
```

Tamamlanmış ve tamamlanmamış durumlar arasında geçiş yapabilen etiketler için temel sınıf.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getChecked()](#getChecked--) | CheckBox'ın işaretli durumda olup olmadığını gösteren bir değeri alır. |
| [getCompletedTime()](#getCompletedTime--) | Tamamlanma zamanını alır veya ayarlar. |
| [getCreationTime()](#getCreationTime--) | Oluşturma zamanını alır veya ayarlar. |
| [getIcon()](#getIcon--) | Simgeyi alır veya ayarlar. |
| [getStatus()](#getStatus--) | Durumu alır veya ayarlar. |
| [setCompleted()](#setCompleted--) | Etiketi, tamamlanma zamanı olarak geçerli zamanı kullanarak tamamlanmış duruma ayarlar. |
| [setCompleted(Date completedTime)](#setCompleted-java.util.Date-) | Etiketi tamamlanmış duruma ayarlar. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Oluşturma zamanını alır veya ayarlar. |
| [setOpen()](#setOpen--) | Etiketi açık duruma ayarlar. |
### getChecked() {#getChecked--}
```
public final boolean getChecked()
```


CheckBox'ın işaretli durumda olup olmadığını gösteren bir değeri alır.

**Returns:**
boolean
### getCompletedTime() {#getCompletedTime--}
```
public final Date getCompletedTime()
```


Tamamlanma zamanını alır veya ayarlar.

Değer: `Nullable\{DateTime\}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Oluşturma zamanını alır veya ayarlar.

Değer: java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


Simgeyi alır veya ayarlar.

Değer: [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getStatus() {#getStatus--}
```
public final int getStatus()
```


Durumu alır veya ayarlar.

Değer: [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCompleted() {#setCompleted--}
```
public final void setCompleted()
```


Etiketi, tamamlanma zamanı olarak geçerli zamanı kullanarak tamamlanmış duruma ayarlar.

### setCompleted(Date completedTime) {#setCompleted-java.util.Date-}
```
public final void setCompleted(Date completedTime)
```


Etiketi tamamlanmış duruma ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| completedTime | java.util.Date | Tamamlanma zamanı. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public final void setCreationTime(Date value)
```


Oluşturma zamanını alır veya ayarlar.

Değer: java.util.Date.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


Etiketi açık duruma ayarlar.

