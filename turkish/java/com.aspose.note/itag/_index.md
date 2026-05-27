---
title: "ITag"
second_title: "Aspose.Note for Java API Referansı"
description: "Her türlü etiket için arabirim."
type: docs
weight: 109
url: /tr/java/com.aspose.note/itag/
---
```
public interface ITag
```

Her türlü etiket için arabirim.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getCompletedTime()](#getCompletedTime--) | Tamamlanma zamanını alır. |
| [getCreationTime()](#getCreationTime--) | Oluşturulma zamanını alır. |
| [getIcon()](#getIcon--) | Simgeyi alır. |
| [getLabel()](#getLabel--) | Etiket metnini alır. |
| [getStatus()](#getStatus--) | Durumu alır. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Oluşturma zamanını ayarlar. |
### getCompletedTime() {#getCompletedTime--}
```
public abstract Date getCompletedTime()
```


Tamamlanma zamanını alır.

Değer: `Nullable\{DateTime\}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public abstract Date getCreationTime()
```


Oluşturulma zamanını alır.

Değer: java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


Simgeyi alır.

Değer: [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getLabel() {#getLabel--}
```
public abstract String getLabel()
```


Etiket metnini alır.

**Returns:**
java.lang.String
### getStatus() {#getStatus--}
```
public abstract int getStatus()
```


Durumu alır.

Değer: [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public abstract void setCreationTime(Date value)
```


Oluşturma zamanını ayarlar.

Değer: java.util.Date.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date |  |

