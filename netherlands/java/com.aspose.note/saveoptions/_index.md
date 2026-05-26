---
title: "SaveOptions"
second_title: "Aspose.Note for Java API-referentie"
description: "Een abstracte basisklasse die documentopslagopties voor een bepaald formaat voorstelt."
type: docs
weight: 85
url: /nl/java/com.aspose.note/saveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SaveOptions
```

Een abstracte basisklasse die documentopslagopties voor een bepaald formaat voorstelt.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getFontsSubsystem()](#getFontsSubsystem--) | Haalt de lettertype-instellingen op die tijdens het opslaan worden gebruikt of stelt deze in. |
| [getPageCount()](#getPageCount--) | Haalt het aantal pagina's op dat moet worden opgeslagen of stelt dit in. |
| [getPageIndex()](#getPageIndex--) | Haalt de index van de eerste pagina die moet worden opgeslagen op of stelt deze in. |
| [getSaveFormat()](#getSaveFormat--) | Haalt het formaat op waarin het document wordt opgeslagen of stelt dit in. |
| [setFontsSubsystem(FontsSubsystem value)](#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-) | Haalt de lettertype-instellingen op die tijdens het opslaan worden gebruikt of stelt deze in. |
| [setPageCount(int value)](#setPageCount-int-) | Haalt het aantal pagina's op dat moet worden opgeslagen of stelt dit in. |
| [setPageIndex(int value)](#setPageIndex-int-) | Haalt de index van de eerste pagina die moet worden opgeslagen op of stelt deze in. |
### getFontsSubsystem() {#getFontsSubsystem--}
```
public final FontsSubsystem getFontsSubsystem()
```


Haalt de lettertype-instellingen op die tijdens het opslaan worden gebruikt of stelt deze in.

**Returns:**
[FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Haalt het aantal pagina's op dat moet worden opgeslagen of stelt dit in. Standaard is \{@link int\#Int32Extensions.MaxValue\} wat betekent dat alle pagina's van het document worden gerenderd.

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


Haalt de index van de eerste pagina die moet worden opgeslagen op of stelt deze in. Standaard is 0.

**Returns:**
int
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Haalt het formaat op waarin het document wordt opgeslagen of stelt dit in.

**Returns:**
int
### setFontsSubsystem(FontsSubsystem value) {#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-}
```
public final void setFontsSubsystem(FontsSubsystem value)
```


Haalt de lettertype-instellingen op die tijdens het opslaan worden gebruikt of stelt deze in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem) |  |

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


Haalt het aantal pagina's op dat moet worden opgeslagen of stelt dit in. Standaard is \{@link int\#Int32Extensions.MaxValue\} wat betekent dat alle pagina's van het document worden gerenderd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


Haalt de index van de eerste pagina die moet worden opgeslagen op of stelt deze in. Standaard is 0.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int |  |

