---
title: "CheckBox"
second_title: "Aspose.Note for Java API-referentie"
description: "De basisklasse voor tags die hun status kunnen schakelen tussen voltooid en onvoltooid."
type: docs
weight: 13
url: /nl/java/com.aspose.note/checkbox/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended
```
public abstract class CheckBox extends TagExtended
```

De basisklasse voor tags die hun status kunnen schakelen tussen voltooid en onvoltooid.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getChecked()](#getChecked--) | Haalt een waarde op die aangeeft of de CheckBox zich in de aangevinkte toestand bevindt. |
| [getCompletedTime()](#getCompletedTime--) | Haalt het voltooid tijdstip op of stelt het in. |
| [getCreationTime()](#getCreationTime--) | Haalt het aanmaaktijdstip op of stelt het in. |
| [getIcon()](#getIcon--) | Haalt het pictogram op of stelt dit in. |
| [getStatus()](#getStatus--) | Haalt de status op of stelt deze in. |
| [setCompleted()](#setCompleted--) | Stelt de tag in op de voltooide status met gebruik van de huidige tijd als voltooid tijdstip. |
| [setCompleted(Date completedTime)](#setCompleted-java.util.Date-) | Stelt de tag in op de voltooide status. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Haalt het aanmaaktijdstip op of stelt het in. |
| [setOpen()](#setOpen--) | Stelt de tag in op open status. |
### getChecked() {#getChecked--}
```
public final boolean getChecked()
```


Haalt een waarde op die aangeeft of de CheckBox zich in de aangevinkte toestand bevindt.

**Returns:**
boolean
### getCompletedTime() {#getCompletedTime--}
```
public final Date getCompletedTime()
```


Haalt het voltooid tijdstip op of stelt het in.

Waarde: De `Nullable{DateTime}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Haalt het aanmaaktijdstip op of stelt het in.

Waarde: De java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


Haalt het pictogram op of stelt dit in.

Waarde: De [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getStatus() {#getStatus--}
```
public final int getStatus()
```


Haalt de status op of stelt deze in.

Waarde: De [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCompleted() {#setCompleted--}
```
public final void setCompleted()
```


Stelt de tag in op de voltooide status met gebruik van de huidige tijd als voltooid tijdstip.

### setCompleted(Date completedTime) {#setCompleted-java.util.Date-}
```
public final void setCompleted(Date completedTime)
```


Stelt de tag in op de voltooide status.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| completedTime | java.util.Date | De voltooide tijd. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public final void setCreationTime(Date value)
```


Haalt het aanmaaktijdstip op of stelt het in.

Waarde: De java.util.Date.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


Stelt de tag in op open status.

