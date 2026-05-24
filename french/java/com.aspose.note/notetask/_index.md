---
title: "NoteTask"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Représente une tâche de note."
type: docs
weight: 55
url: /fr/java/com.aspose.note/notetask/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended, [com.aspose.note.CheckBox](../../com.aspose.note/checkbox)
```
public final class NoteTask extends CheckBox
```

Représente une tâche de note.
## Méthodes

| Méthode | Description |
| --- | --- |
| [createCustomFollowUpDate(Date dueDate)](#createCustomFollowUpDate-java.util.Date-) | Crée une nouvelle tâche de note avec l'icône NoFollowUpDateFlag et la date d'échéance spécifiée. |
| [createFollowUpNextWeek()](#createFollowUpNextWeek--) | * Crée une nouvelle étiquette de note avec l'icône FollowUpNextWeekFlag. |
| [createFollowUpThisWeek()](#createFollowUpThisWeek--) | * Crée une nouvelle étiquette de note avec l'icône FollowUpThisWeekFlag. |
| [createFollowUpToday()](#createFollowUpToday--) | * Crée une nouvelle étiquette de note avec l'icône FollowUpTodayFlag. |
| [createFollowUpTomorrow()](#createFollowUpTomorrow--) | * Crée une nouvelle étiquette de note avec l'icône FollowUpTomorrowFlag. |
| [createNoFollowUpDate()](#createNoFollowUpDate--) | * Crée une nouvelle étiquette de note avec l'icône NoFollowUpDateFlag. |
| [equals(NoteTask other)](#equals-com.aspose.note.NoteTask-) | Détermine si l'objet spécifié est égal à l'objet actuel. |
| [equals(Object obj)](#equals-java.lang.Object-) | Détermine si l'objet spécifié est égal à l'objet actuel. |
| [getDueDate()](#getDueDate--) | Obtient ou définit la date d'échéance. |
| [getIcon()](#getIcon--) | Obtient ou définit l'icône. |
| [getLabel()](#getLabel--) |  |
| [hashCode()](#hashCode--) | Servit de fonction de hachage pour le type. |
| [setDueDate(Date value)](#setDueDate-java.util.Date-) | Obtient ou définit la date d'échéance. |
| [setOpen()](#setOpen--) | Définit l'étiquette à l'état ouvert. |
### createCustomFollowUpDate(Date dueDate) {#createCustomFollowUpDate-java.util.Date-}
```
public static NoteTask createCustomFollowUpDate(Date dueDate)
```


Crée une nouvelle tâche de note avec l'icône NoFollowUpDateFlag et la date d'échéance spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| dueDate | java.util.Date | La date d'échéance. |

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpNextWeek() {#createFollowUpNextWeek--}
```
public static NoteTask createFollowUpNextWeek()
```


* Crée une nouvelle étiquette de note avec l'icône FollowUpNextWeekFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpThisWeek() {#createFollowUpThisWeek--}
```
public static NoteTask createFollowUpThisWeek()
```


* Crée une nouvelle étiquette de note avec l'icône FollowUpThisWeekFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpToday() {#createFollowUpToday--}
```
public static NoteTask createFollowUpToday()
```


* Crée une nouvelle étiquette de note avec l'icône FollowUpTodayFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpTomorrow() {#createFollowUpTomorrow--}
```
public static NoteTask createFollowUpTomorrow()
```


* Crée une nouvelle étiquette de note avec l'icône FollowUpTomorrowFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createNoFollowUpDate() {#createNoFollowUpDate--}
```
public static NoteTask createNoFollowUpDate()
```


* Crée une nouvelle étiquette de note avec l'icône NoFollowUpDateFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### equals(NoteTask other) {#equals-com.aspose.note.NoteTask-}
```
public boolean equals(NoteTask other)
```


Détermine si l'objet spécifié est égal à l'objet actuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| other | [NoteTask](../../com.aspose.note/notetask) | L'objet. |

**Returns:**
booléen - Le `bool`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Détermine si l'objet spécifié est égal à l'objet actuel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | L'objet. |

**Returns:**
booléen - Le `bool`.
### getDueDate() {#getDueDate--}
```
public Date getDueDate()
```


Obtient ou définit la date d'échéance.

Valeur: le `DateTime`.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public int getIcon()
```


Obtient ou définit l'icône.

Valeur : Le [TagIcon](../../com.aspose.note.infrastructure/tagicon).

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


Servit de fonction de hachage pour le type.

**Returns:**
int - Le `int`.
### setDueDate(Date value) {#setDueDate-java.util.Date-}
```
public void setDueDate(Date value)
```


Obtient ou définit la date d'échéance.

Valeur: le `DateTime`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


Définit l'étiquette à l'état ouvert.

