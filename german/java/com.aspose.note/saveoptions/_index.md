---
title: "SaveOptions"
second_title: "Aspose.Note für Java API-Referenz"
description: "Eine abstrakte Basisklasse, die Dokumentspeicheroptionen für ein bestimmtes Format darstellt."
type: docs
weight: 85
url: /de/java/com.aspose.note/saveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SaveOptions
```

Eine abstrakte Basisklasse, die Dokumentspeicheroptionen für ein bestimmtes Format darstellt.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getFontsSubsystem()](#getFontsSubsystem--) | Ruft die Schriftarteinstellungen ab, die beim Speichern verwendet werden, oder legt sie fest. |
| [getPageCount()](#getPageCount--) | Ruft die Anzahl der zu speichernden Seiten ab oder legt sie fest. |
| [getPageIndex()](#getPageIndex--) | Ruft den Index der ersten zu speichernden Seite ab oder legt ihn fest. |
| [getSaveFormat()](#getSaveFormat--) | Ruft das Format ab, in dem das Dokument gespeichert wird, oder legt es fest. |
| [setFontsSubsystem(FontsSubsystem value)](#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-) | Ruft die Schriftarteinstellungen ab, die beim Speichern verwendet werden, oder legt sie fest. |
| [setPageCount(int value)](#setPageCount-int-) | Ruft die Anzahl der zu speichernden Seiten ab oder legt sie fest. |
| [setPageIndex(int value)](#setPageIndex-int-) | Ruft den Index der ersten zu speichernden Seite ab oder legt ihn fest. |
### getFontsSubsystem() {#getFontsSubsystem--}
```
public final FontsSubsystem getFontsSubsystem()
```


Ruft die Schriftarteinstellungen ab, die beim Speichern verwendet werden, oder legt sie fest.

**Returns:**
[FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Ruft die Anzahl der zu speichernden Seiten ab oder legt sie fest. Standardmäßig ist \{@link int\#Int32Extensions.MaxValue\}, was bedeutet, dass alle Seiten des Dokuments gerendert werden.

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


Ruft den Index der ersten zu speichernden Seite ab oder legt ihn fest. Standardmäßig ist 0.

**Returns:**
int
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Ruft das Format ab, in dem das Dokument gespeichert wird, oder legt es fest.

**Returns:**
int
### setFontsSubsystem(FontsSubsystem value) {#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-}
```
public final void setFontsSubsystem(FontsSubsystem value)
```


Ruft die Schriftarteinstellungen ab, die beim Speichern verwendet werden, oder legt sie fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem) |  |

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


Ruft die Anzahl der zu speichernden Seiten ab oder legt sie fest. Standardmäßig ist \{@link int\#Int32Extensions.MaxValue\}, was bedeutet, dass alle Seiten des Dokuments gerendert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


Ruft den Index der ersten zu speichernden Seite ab oder legt ihn fest. Standardmäßig ist 0.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

