---
title: "CheckBox"
second_title: "Aspose.Note for Java API-referens"
description: "Bas-klassen för taggar som kan växla sitt tillstånd mellan komplett och ofullständig."
type: docs
weight: 13
url: /sv/java/com.aspose.note/checkbox/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended
```
public abstract class CheckBox extends TagExtended
```

Bas-klassen för taggar som kan växla sitt tillstånd mellan komplett och ofullständig.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getChecked()](#getChecked--) | Hämtar ett värde som indikerar om CheckBox är i markerat tillstånd. |
| [getCompletedTime()](#getCompletedTime--) | Hämtar eller anger den slutförda tiden. |
| [getCreationTime()](#getCreationTime--) | Hämtar eller anger skapningstiden. |
| [getIcon()](#getIcon--) | Hämtar eller anger ikonen. |
| [getStatus()](#getStatus--) | Hämtar eller anger statusen. |
| [setCompleted()](#setCompleted--) | Ställer in taggen till slutfört tillstånd med aktuell tid som slutfört tid. |
| [setCompleted(Date completedTime)](#setCompleted-java.util.Date-) | Ställer in taggen till slutfört tillstånd. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Hämtar eller anger skapningstiden. |
| [setOpen()](#setOpen--) | Sätter taggen till öppet läge. |
### getChecked() {#getChecked--}
```
public final boolean getChecked()
```


Hämtar ett värde som indikerar om CheckBox är i markerat tillstånd.

**Returns:**
boolean
### getCompletedTime() {#getCompletedTime--}
```
public final Date getCompletedTime()
```


Hämtar eller anger den slutförda tiden.

Värde: `Nullable\{DateTime\}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Hämtar eller anger skapningstiden.

Värde: java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


Hämtar eller anger ikonen.

Värde: [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getStatus() {#getStatus--}
```
public final int getStatus()
```


Hämtar eller anger statusen.

Värde: [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCompleted() {#setCompleted--}
```
public final void setCompleted()
```


Ställer in taggen till slutfört tillstånd med aktuell tid som slutfört tid.

### setCompleted(Date completedTime) {#setCompleted-java.util.Date-}
```
public final void setCompleted(Date completedTime)
```


Ställer in taggen till slutfört tillstånd.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| completedTime | java.util.Date | Den slutförda tiden. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public final void setCreationTime(Date value)
```


Hämtar eller anger skapningstiden.

Värde: java.util.Date.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


Sätter taggen till öppet läge.

