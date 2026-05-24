---
title: "ITag"
second_title: "Aspose.Note für Java API-Referenz"
description: "Die Schnittstelle für Tags aller Art."
type: docs
weight: 109
url: /de/java/com.aspose.note/itag/
---
```
public interface ITag
```

Die Schnittstelle für Tags aller Art.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getCompletedTime()](#getCompletedTime--) | Liest die Abschlusszeit. |
| [getCreationTime()](#getCreationTime--) | Liest die Erstellungszeit. |
| [getIcon()](#getIcon--) | Liest das Symbol. |
| [getLabel()](#getLabel--) | Liest den Etikettentext. |
| [getStatus()](#getStatus--) | Liest den Status. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Setzt die Erstellungszeit. |
### getCompletedTime() {#getCompletedTime--}
```
public abstract Date getCompletedTime()
```


Liest die Abschlusszeit.

Wert: Das `Nullable\{DateTime\}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public abstract Date getCreationTime()
```


Liest die Erstellungszeit.

Wert: Das java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


Liest das Symbol.

Wert: Das [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getLabel() {#getLabel--}
```
public abstract String getLabel()
```


Liest den Etikettentext.

**Returns:**
java.lang.String
### getStatus() {#getStatus--}
```
public abstract int getStatus()
```


Liest den Status.

Wert: Das [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public abstract void setCreationTime(Date value)
```


Setzt die Erstellungszeit.

Wert: Das java.util.Date.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date |  |

