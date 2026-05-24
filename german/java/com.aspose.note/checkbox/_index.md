---
title: "CheckBox"
second_title: "Aspose.Note für Java API-Referenz"
description: "Die Basisklasse für Tags, die ihren Zustand zwischen vollständig und unvollständig umschalten können."
type: docs
weight: 13
url: /de/java/com.aspose.note/checkbox/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended
```
public abstract class CheckBox extends TagExtended
```

Die Basisklasse für Tags, die ihren Zustand zwischen vollständig und unvollständig umschalten können.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getChecked()](#getChecked--) | Gibt einen Wert zurück, der angibt, ob das CheckBox im aktivierten Zustand ist. |
| [getCompletedTime()](#getCompletedTime--) | Liest oder setzt die Abschlusszeit. |
| [getCreationTime()](#getCreationTime--) | Liest oder setzt die Erstellungszeit. |
| [getIcon()](#getIcon--) | Liest oder setzt das Icon. |
| [getStatus()](#getStatus--) | Liest oder setzt den Status. |
| [setCompleted()](#setCompleted--) | Setzt das Tag auf den abgeschlossenen Zustand und verwendet die aktuelle Zeit als Abschlusszeit. |
| [setCompleted(Date completedTime)](#setCompleted-java.util.Date-) | Setzt das Tag auf den abgeschlossenen Zustand. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Liest oder setzt die Erstellungszeit. |
| [setOpen()](#setOpen--) | Setzt das Tag auf den offenen Zustand. |
### getChecked() {#getChecked--}
```
public final boolean getChecked()
```


Gibt einen Wert zurück, der angibt, ob das CheckBox im aktivierten Zustand ist.

**Returns:**
boolean
### getCompletedTime() {#getCompletedTime--}
```
public final Date getCompletedTime()
```


Liest oder setzt die Abschlusszeit.

Wert: Das `Nullable\{DateTime\}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Liest oder setzt die Erstellungszeit.

Wert: Das java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


Liest oder setzt das Icon.

Wert: Das [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getStatus() {#getStatus--}
```
public final int getStatus()
```


Liest oder setzt den Status.

Wert: Das [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCompleted() {#setCompleted--}
```
public final void setCompleted()
```


Setzt das Tag auf den abgeschlossenen Zustand und verwendet die aktuelle Zeit als Abschlusszeit.

### setCompleted(Date completedTime) {#setCompleted-java.util.Date-}
```
public final void setCompleted(Date completedTime)
```


Setzt das Tag auf den abgeschlossenen Zustand.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| completedTime | java.util.Date | Die Abschlusszeit. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public final void setCreationTime(Date value)
```


Liest oder setzt die Erstellungszeit.

Wert: Das java.util.Date.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


Setzt das Tag auf den offenen Zustand.

