---
title: "NoteTask"
second_title: "Aspose.Note for Java API Referansı"
description: "Bir not görevini temsil eder."
type: docs
weight: 55
url: /tr/java/com.aspose.note/notetask/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended, [com.aspose.note.CheckBox](../../com.aspose.note/checkbox)
```
public final class NoteTask extends CheckBox
```

Bir not görevini temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [createCustomFollowUpDate(Date dueDate)](#createCustomFollowUpDate-java.util.Date-) | NoFollowUpDateFlag simgesi ve belirtilen son tarih ile yeni bir not görevi oluşturur. |
| [createFollowUpNextWeek()](#createFollowUpNextWeek--) | * FollowUpNextWeekFlag simgesi ile yeni bir not etiketi oluşturur. |
| [createFollowUpThisWeek()](#createFollowUpThisWeek--) | * FollowUpThisWeekFlag simgesi ile yeni bir not etiketi oluşturur. |
| [createFollowUpToday()](#createFollowUpToday--) | * FollowUpTodayFlag simgesi ile yeni bir not etiketi oluşturur. |
| [createFollowUpTomorrow()](#createFollowUpTomorrow--) | * FollowUpTomorrowFlag simgesi ile yeni bir not etiketi oluşturur. |
| [createNoFollowUpDate()](#createNoFollowUpDate--) | * NoFollowUpDateFlag simgesi ile yeni bir not etiketi oluşturur. |
| [equals(NoteTask other)](#equals-com.aspose.note.NoteTask-) | Belirtilen nesnenin mevcut nesneye eşit olup olmadığını belirler. |
| [equals(Object obj)](#equals-java.lang.Object-) | Belirtilen nesnenin mevcut nesneye eşit olup olmadığını belirler. |
| [getDueDate()](#getDueDate--) | Son tarihi alır veya ayarlar. |
| [getIcon()](#getIcon--) | Simgeyi alır veya ayarlar. |
| [getLabel()](#getLabel--) |  |
| [hashCode()](#hashCode--) | Tür için bir karma işlevi olarak hizmet verir. |
| [setDueDate(Date value)](#setDueDate-java.util.Date-) | Son tarihi alır veya ayarlar. |
| [setOpen()](#setOpen--) | Etiketi açık duruma ayarlar. |
### createCustomFollowUpDate(Date dueDate) {#createCustomFollowUpDate-java.util.Date-}
```
public static NoteTask createCustomFollowUpDate(Date dueDate)
```


NoFollowUpDateFlag simgesi ve belirtilen son tarih ile yeni bir not görevi oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dueDate | java.util.Date | Son Tarih. |

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpNextWeek() {#createFollowUpNextWeek--}
```
public static NoteTask createFollowUpNextWeek()
```


* FollowUpNextWeekFlag simgesi ile yeni bir not etiketi oluşturur.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpThisWeek() {#createFollowUpThisWeek--}
```
public static NoteTask createFollowUpThisWeek()
```


* FollowUpThisWeekFlag simgesi ile yeni bir not etiketi oluşturur.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpToday() {#createFollowUpToday--}
```
public static NoteTask createFollowUpToday()
```


* FollowUpTodayFlag simgesi ile yeni bir not etiketi oluşturur.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpTomorrow() {#createFollowUpTomorrow--}
```
public static NoteTask createFollowUpTomorrow()
```


* FollowUpTomorrowFlag simgesi ile yeni bir not etiketi oluşturur.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createNoFollowUpDate() {#createNoFollowUpDate--}
```
public static NoteTask createNoFollowUpDate()
```


* NoFollowUpDateFlag simgesi ile yeni bir not etiketi oluşturur.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### equals(NoteTask other) {#equals-com.aspose.note.NoteTask-}
```
public boolean equals(NoteTask other)
```


Belirtilen nesnenin mevcut nesneye eşit olup olmadığını belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | [NoteTask](../../com.aspose.note/notetask) | Nesne. |

**Returns:**
boolean - Bu `bool`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Belirtilen nesnenin mevcut nesneye eşit olup olmadığını belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object | Nesne. |

**Returns:**
boolean - Bu `bool`.
### getDueDate() {#getDueDate--}
```
public Date getDueDate()
```


Son tarihi alır veya ayarlar.

Değer: `DateTime`.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public int getIcon()
```


Simgeyi alır veya ayarlar.

Değer: [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getLabel() {#getLabel--}
```
public String getLabel()
```




**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public int hashCode()
```


Tür için bir karma işlevi olarak hizmet verir.

**Returns:**
int - Bu `int`.
### setDueDate(Date value) {#setDueDate-java.util.Date-}
```
public void setDueDate(Date value)
```


Son tarihi alır veya ayarlar.

Değer: `DateTime`.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


Etiketi açık duruma ayarlar.

