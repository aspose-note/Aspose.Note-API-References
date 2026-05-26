---
title: "SaveOptions"
second_title: "Aspose.Note for Java API-referens"
description: "En abstrakt basklass som representerar alternativ för dokumentlagring för ett specifikt format."
type: docs
weight: 85
url: /sv/java/com.aspose.note/saveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SaveOptions
```

En abstrakt basklass som representerar alternativ för dokumentlagring för ett specifikt format.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getFontsSubsystem()](#getFontsSubsystem--) | Hämtar eller anger teckensnittets inställningar som ska användas vid sparande |
| [getPageCount()](#getPageCount--) | Hämtar eller anger antalet sidor som ska sparas. |
| [getPageIndex()](#getPageIndex--) | Hämtar eller anger index för den första sidan som ska sparas. |
| [getSaveFormat()](#getSaveFormat--) | Hämtar eller anger formatet som dokumentet sparas i. |
| [setFontsSubsystem(FontsSubsystem value)](#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-) | Hämtar eller anger teckensnittets inställningar som ska användas vid sparande |
| [setPageCount(int value)](#setPageCount-int-) | Hämtar eller anger antalet sidor som ska sparas. |
| [setPageIndex(int value)](#setPageIndex-int-) | Hämtar eller anger index för den första sidan som ska sparas. |
### getFontsSubsystem() {#getFontsSubsystem--}
```
public final FontsSubsystem getFontsSubsystem()
```


Hämtar eller anger teckensnittets inställningar som ska användas vid sparande

**Returns:**
[FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Hämtar eller anger antalet sidor som ska sparas. Standardvärdet är \{@link int\#Int32Extensions.MaxValue\} vilket betyder att alla sidor i dokumentet kommer att renderas.

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


Hämtar eller anger index för den första sidan som ska sparas. Standardvärdet är 0.

**Returns:**
int
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Hämtar eller anger formatet som dokumentet sparas i.

**Returns:**
int
### setFontsSubsystem(FontsSubsystem value) {#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-}
```
public final void setFontsSubsystem(FontsSubsystem value)
```


Hämtar eller anger teckensnittets inställningar som ska användas vid sparande

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem) |  |

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


Hämtar eller anger antalet sidor som ska sparas. Standardvärdet är \{@link int\#Int32Extensions.MaxValue\} vilket betyder att alla sidor i dokumentet kommer att renderas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


Hämtar eller anger index för den första sidan som ska sparas. Standardvärdet är 0.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

