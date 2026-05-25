---
title: "NoteTask"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Rappresenta un'attività di nota."
type: docs
weight: 55
url: /it/java/com.aspose.note/notetask/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended, [com.aspose.note.CheckBox](../../com.aspose.note/checkbox)
```
public final class NoteTask extends CheckBox
```

Rappresenta un'attività di nota.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [createCustomFollowUpDate(Date dueDate)](#createCustomFollowUpDate-java.util.Date-) | Crea un nuovo compito nota con l'icona NoFollowUpDateFlag e la data di scadenza specificata. |
| [createFollowUpNextWeek()](#createFollowUpNextWeek--) | \* Crea un nuovo tag nota con l'icona FollowUpNextWeekFlag. |
| [createFollowUpThisWeek()](#createFollowUpThisWeek--) | \* Crea un nuovo tag nota con l'icona FollowUpThisWeekFlag. |
| [createFollowUpToday()](#createFollowUpToday--) | \* Crea un nuovo tag nota con l'icona FollowUpTodayFlag. |
| [createFollowUpTomorrow()](#createFollowUpTomorrow--) | \* Crea un nuovo tag nota con l'icona FollowUpTomorrowFlag. |
| [createNoFollowUpDate()](#createNoFollowUpDate--) | \* Crea un nuovo tag nota con l'icona NoFollowUpDateFlag. |
| [equals(NoteTask other)](#equals-com.aspose.note.NoteTask-) | Determina se l'oggetto specificato è uguale all'oggetto corrente. |
| [equals(Object obj)](#equals-java.lang.Object-) | Determina se l'oggetto specificato è uguale all'oggetto corrente. |
| [getDueDate()](#getDueDate--) | Ottiene o imposta la data di scadenza. |
| [getIcon()](#getIcon--) | Ottiene o imposta l'icona. |
| [getLabel()](#getLabel--) |  |
| [hashCode()](#hashCode--) | Funziona come funzione hash per il tipo. |
| [setDueDate(Date value)](#setDueDate-java.util.Date-) | Ottiene o imposta la data di scadenza. |
| [setOpen()](#setOpen--) | Imposta il tag in stato aperto. |
### createCustomFollowUpDate(Date dueDate) {#createCustomFollowUpDate-java.util.Date-}
```
public static NoteTask createCustomFollowUpDate(Date dueDate)
```


Crea un nuovo compito nota con l'icona NoFollowUpDateFlag e la data di scadenza specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dueDate | java.util.Date | La data di scadenza. |

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpNextWeek() {#createFollowUpNextWeek--}
```
public static NoteTask createFollowUpNextWeek()
```


\* Crea un nuovo tag nota con l'icona FollowUpNextWeekFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpThisWeek() {#createFollowUpThisWeek--}
```
public static NoteTask createFollowUpThisWeek()
```


\* Crea un nuovo tag nota con l'icona FollowUpThisWeekFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpToday() {#createFollowUpToday--}
```
public static NoteTask createFollowUpToday()
```


\* Crea un nuovo tag nota con l'icona FollowUpTodayFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpTomorrow() {#createFollowUpTomorrow--}
```
public static NoteTask createFollowUpTomorrow()
```


\* Crea un nuovo tag nota con l'icona FollowUpTomorrowFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createNoFollowUpDate() {#createNoFollowUpDate--}
```
public static NoteTask createNoFollowUpDate()
```


\* Crea un nuovo tag nota con l'icona NoFollowUpDateFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### equals(NoteTask other) {#equals-com.aspose.note.NoteTask-}
```
public boolean equals(NoteTask other)
```


Determina se l'oggetto specificato è uguale all'oggetto corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | [NoteTask](../../com.aspose.note/notetask) | L'oggetto. |

**Returns:**
boolean - Il `bool`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determina se l'oggetto specificato è uguale all'oggetto corrente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object | L'oggetto. |

**Returns:**
boolean - Il `bool`.
### getDueDate() {#getDueDate--}
```
public Date getDueDate()
```


Ottiene o imposta la data di scadenza.

Valore: il `DateTime`.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public int getIcon()
```


Ottiene o imposta l'icona.

Valore: Il [TagIcon](../../com.aspose.note.infrastructure/tagicon).

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


Funziona come funzione hash per il tipo.

**Returns:**
int - Il `int`.
### setDueDate(Date value) {#setDueDate-java.util.Date-}
```
public void setDueDate(Date value)
```


Ottiene o imposta la data di scadenza.

Valore: il `DateTime`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


Imposta il tag in stato aperto.

