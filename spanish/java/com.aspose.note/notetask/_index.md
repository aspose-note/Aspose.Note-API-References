---
title: "NoteTask"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Representa una tarea de nota."
type: docs
weight: 55
url: /es/java/com.aspose.note/notetask/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended, [com.aspose.note.CheckBox](../../com.aspose.note/checkbox)
```
public final class NoteTask extends CheckBox
```

Representa una tarea de nota.
## Métodos

| Método | Descripción |
| --- | --- |
| [createCustomFollowUpDate(Date dueDate)](#createCustomFollowUpDate-java.util.Date-) | Crea una nueva tarea de nota con el icono NoFollowUpDateFlag y la fecha de vencimiento especificada. |
| [createFollowUpNextWeek()](#createFollowUpNextWeek--) | \* Crea una nueva etiqueta de nota con el icono FollowUpNextWeekFlag. |
| [createFollowUpThisWeek()](#createFollowUpThisWeek--) | \* Crea una nueva etiqueta de nota con el icono FollowUpThisWeekFlag. |
| [createFollowUpToday()](#createFollowUpToday--) | \* Crea una nueva etiqueta de nota con el icono FollowUpTodayFlag. |
| [createFollowUpTomorrow()](#createFollowUpTomorrow--) | \* Crea una nueva etiqueta de nota con el icono FollowUpTomorrowFlag. |
| [createNoFollowUpDate()](#createNoFollowUpDate--) | \* Crea una nueva etiqueta de nota con el icono NoFollowUpDateFlag. |
| [equals(NoteTask other)](#equals-com.aspose.note.NoteTask-) | Determina si el objeto especificado es igual al objeto actual. |
| [equals(Object obj)](#equals-java.lang.Object-) | Determina si el objeto especificado es igual al objeto actual. |
| [getDueDate()](#getDueDate--) | Obtiene o establece la fecha de vencimiento. |
| [getIcon()](#getIcon--) | Obtiene o establece el ícono. |
| [getLabel()](#getLabel--) |  |
| [hashCode()](#hashCode--) | Funciona como una función hash para el tipo. |
| [setDueDate(Date value)](#setDueDate-java.util.Date-) | Obtiene o establece la fecha de vencimiento. |
| [setOpen()](#setOpen--) | Establece la etiqueta en estado abierto. |
### createCustomFollowUpDate(Date dueDate) {#createCustomFollowUpDate-java.util.Date-}
```
public static NoteTask createCustomFollowUpDate(Date dueDate)
```


Crea una nueva tarea de nota con el icono NoFollowUpDateFlag y la fecha de vencimiento especificada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dueDate | java.util.Date | La fecha de vencimiento. |

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpNextWeek() {#createFollowUpNextWeek--}
```
public static NoteTask createFollowUpNextWeek()
```


\* Crea una nueva etiqueta de nota con el icono FollowUpNextWeekFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpThisWeek() {#createFollowUpThisWeek--}
```
public static NoteTask createFollowUpThisWeek()
```


\* Crea una nueva etiqueta de nota con el icono FollowUpThisWeekFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpToday() {#createFollowUpToday--}
```
public static NoteTask createFollowUpToday()
```


\* Crea una nueva etiqueta de nota con el icono FollowUpTodayFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpTomorrow() {#createFollowUpTomorrow--}
```
public static NoteTask createFollowUpTomorrow()
```


\* Crea una nueva etiqueta de nota con el icono FollowUpTomorrowFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createNoFollowUpDate() {#createNoFollowUpDate--}
```
public static NoteTask createNoFollowUpDate()
```


\* Crea una nueva etiqueta de nota con el icono NoFollowUpDateFlag.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### equals(NoteTask other) {#equals-com.aspose.note.NoteTask-}
```
public boolean equals(NoteTask other)
```


Determina si el objeto especificado es igual al objeto actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | [NoteTask](../../com.aspose.note/notetask) | El objeto. |

**Returns:**
boolean - El `bool`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determina si el objeto especificado es igual al objeto actual.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | java.lang.Object | El objeto. |

**Returns:**
boolean - El `bool`.
### getDueDate() {#getDueDate--}
```
public Date getDueDate()
```


Obtiene o establece la fecha de vencimiento.

Valor: El `DateTime`.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public int getIcon()
```


Obtiene o establece el ícono.

Valor: El [TagIcon](../../com.aspose.note.infrastructure/tagicon).

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


Funciona como una función hash para el tipo.

**Returns:**
int - El `int`.
### setDueDate(Date value) {#setDueDate-java.util.Date-}
```
public void setDueDate(Date value)
```


Obtiene o establece la fecha de vencimiento.

Valor: El `DateTime`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


Establece la etiqueta en estado abierto.

