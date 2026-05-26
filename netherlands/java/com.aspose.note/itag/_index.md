---
title: "ITag"
second_title: "Aspose.Note for Java API-referentie"
description: "De interface voor tags van alle soorten."
type: docs
weight: 109
url: /nl/java/com.aspose.note/itag/
---
```
public interface ITag
```

De interface voor tags van alle soorten.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getCompletedTime()](#getCompletedTime--) | Haalt de voltooidtijd op. |
| [getCreationTime()](#getCreationTime--) | Haalt de creatietijd op. |
| [getIcon()](#getIcon--) | Haalt het pictogram op. |
| [getLabel()](#getLabel--) | Haalt de labeltekst op. |
| [getStatus()](#getStatus--) | Haalt de status op. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Stelt de creatietijd in. |
### getCompletedTime() {#getCompletedTime--}
```
public abstract Date getCompletedTime()
```


Haalt de voltooidtijd op.

Waarde: De `Nullable{DateTime}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public abstract Date getCreationTime()
```


Haalt de creatietijd op.

Waarde: De java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


Haalt het pictogram op.

Waarde: De [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getLabel() {#getLabel--}
```
public abstract String getLabel()
```


Haalt de labeltekst op.

**Returns:**
java.lang.String
### getStatus() {#getStatus--}
```
public abstract int getStatus()
```


Haalt de status op.

Waarde: De [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public abstract void setCreationTime(Date value)
```


Stelt de creatietijd in.

Waarde: De java.util.Date.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date |  |

