---
title: SaveOptions
second_title: Aspose.Note for Java API Reference
description: An abstract base class which represents document saving options for a particular format.
type: docs
weight: 85
url: /java/com.aspose.note/saveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SaveOptions
```

An abstract base class which represents document saving options for a particular format.
## Methods

| Method | Description |
| --- | --- |
| [getFontsSubsystem()](#getFontsSubsystem--) | Gets or sets font's settings to be used while saving |
| [getPageCount()](#getPageCount--) | Gets or sets the number of pages to save. |
| [getPageIndex()](#getPageIndex--) | Gets or sets the index of the first page to save. |
| [getSaveFormat()](#getSaveFormat--) | Gets or sets the format in which the document is saved. |
| [setFontsSubsystem(FontsSubsystem value)](#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-) | Gets or sets font's settings to be used while saving |
| [setPageCount(int value)](#setPageCount-int-) | Gets or sets the number of pages to save. |
| [setPageIndex(int value)](#setPageIndex-int-) | Gets or sets the index of the first page to save. |
### getFontsSubsystem() {#getFontsSubsystem--}
```
public final FontsSubsystem getFontsSubsystem()
```


Gets or sets font's settings to be used while saving

**Returns:**
[FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Gets or sets the number of pages to save. By default is \{@link int\#Int32Extensions.MaxValue\} which means all pages of the document will be rendered.

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


Gets or sets the index of the first page to save. By default is 0.

**Returns:**
int
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Gets or sets the format in which the document is saved.

**Returns:**
int
### setFontsSubsystem(FontsSubsystem value) {#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-}
```
public final void setFontsSubsystem(FontsSubsystem value)
```


Gets or sets font's settings to be used while saving

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem) |  |

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


Gets or sets the number of pages to save. By default is \{@link int\#Int32Extensions.MaxValue\} which means all pages of the document will be rendered.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


Gets or sets the index of the first page to save. By default is 0.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

