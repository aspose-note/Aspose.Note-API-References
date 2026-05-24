---
title: "NotebookSaveOptions"
second_title: "Aspose.Note für Java API-Referenz"
description: "Eine abstrakte Basisklasse, die Notizbuch-Speicheroptionen für ein bestimmtes Format darstellt."
type: docs
weight: 61
url: /de/java/com.aspose.note/notebooksaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class NotebookSaveOptions
```

Eine abstrakte Basisklasse, die Notizbuch-Speicheroptionen für ein bestimmtes Format darstellt.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getDeferredSaving()](#getDeferredSaving--) | Liest oder setzt einen Wert, der angibt, ob Kinddokumente explizit gespeichert werden sollen. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | Ermittelt die Speicheroptionen für alle Kinddokumente des Notizbuchs. |
| [getFlatten()](#getFlatten--) | Liest oder setzt einen Wert, der angibt, ob die Kindhierarchie des Notizbuchs flach gespeichert wird. |
| [getSaveFormat()](#getSaveFormat--) | Ermittelt das Format, in dem das Notizbuch gespeichert wird. |
| [setDeferredSaving(boolean value)](#setDeferredSaving-boolean-) | Liest oder setzt einen Wert, der angibt, ob Kinddokumente explizit gespeichert werden sollen. |
| [setFlatten(boolean value)](#setFlatten-boolean-) | Liest oder setzt einen Wert, der angibt, ob die Kindhierarchie des Notizbuchs flach gespeichert wird. |
### getDeferredSaving() {#getDeferredSaving--}
```
public boolean getDeferredSaving()
```


Liest oder setzt einen Wert, der angibt, ob Kinddokumente explizit gespeichert werden sollen.

--------------------

Der Standardwert ist `false`, sodass Kinddokumente implizit gespeichert werden. Der Wert `true` bedeutet, dass der Benutzer jeden Kindknoten des Notizbuchs explizit speichern soll. Wenn das Notizbuch in einen Stream gespeichert wird, ist der Wert immer `true`, obwohl er vom Benutzer ausdrücklich auf `false` gesetzt wurde.

**Returns:**
boolean
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public abstract SaveOptions getDocumentSaveOptionsInternal()
```


Ermittelt die Speicheroptionen für alle Kinddokumente des Notizbuchs.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getFlatten() {#getFlatten--}
```
public boolean getFlatten()
```


Liest oder setzt einen Wert, der angibt, ob die Kindhierarchie des Notizbuchs flach gespeichert wird.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public abstract int getSaveFormat()
```


Ermittelt das Format, in dem das Notizbuch gespeichert wird.

**Returns:**
int
### setDeferredSaving(boolean value) {#setDeferredSaving-boolean-}
```
public void setDeferredSaving(boolean value)
```


Liest oder setzt einen Wert, der angibt, ob Kinddokumente explizit gespeichert werden sollen.

--------------------

Der Standardwert ist `false`, sodass Kinddokumente implizit gespeichert werden. Der Wert `true` bedeutet, dass der Benutzer jeden Kindknoten des Notizbuchs explizit speichern soll. Wenn das Notizbuch in einen Stream gespeichert wird, ist der Wert immer `true`, obwohl er vom Benutzer ausdrücklich auf `false` gesetzt wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFlatten(boolean value) {#setFlatten-boolean-}
```
public void setFlatten(boolean value)
```


Liest oder setzt einen Wert, der angibt, ob die Kindhierarchie des Notizbuchs flach gespeichert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

