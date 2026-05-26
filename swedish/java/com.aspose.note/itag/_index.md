---
title: "ITag"
second_title: "Aspose.Note for Java API-referens"
description: "Gränssnittet för taggar av alla slag."
type: docs
weight: 109
url: /sv/java/com.aspose.note/itag/
---
```
public interface ITag
```

Gränssnittet för taggar av alla slag.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getCompletedTime()](#getCompletedTime--) | Hämtar den slutförda tiden. |
| [getCreationTime()](#getCreationTime--) | Hämtar skapandetiden. |
| [getIcon()](#getIcon--) | Hämtar ikonen. |
| [getLabel()](#getLabel--) | Hämtar etiketttexten. |
| [getStatus()](#getStatus--) | Hämtar statusen. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Anger skapandetiden. |
### getCompletedTime() {#getCompletedTime--}
```
public abstract Date getCompletedTime()
```


Hämtar den slutförda tiden.

Värde: `Nullable\{DateTime\}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public abstract Date getCreationTime()
```


Hämtar skapandetiden.

Värde: java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


Hämtar ikonen.

Värde: [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getLabel() {#getLabel--}
```
public abstract String getLabel()
```


Hämtar etiketttexten.

**Returns:**
java.lang.String
### getStatus() {#getStatus--}
```
public abstract int getStatus()
```


Hämtar statusen.

Värde: [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public abstract void setCreationTime(Date value)
```


Anger skapandetiden.

Värde: java.util.Date.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date |  |

