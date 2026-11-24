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
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFontsSubsystem()](#getFontsSubsystem--) | Gets or sets font's settings to be used while saving |
| [getPageCount()](#getPageCount--) | Gets or sets the number of pages to save. |
| [getPageIndex()](#getPageIndex--) | Gets or sets the index of the first page to save. |
| [getSaveFormat()](#getSaveFormat--) | Gets or sets the format in which the document is saved. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFontsSubsystem(FontsSubsystem value)](#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-) | Gets or sets font's settings to be used while saving |
| [setPageCount(int value)](#setPageCount-int-) | Gets or sets the number of pages to save. |
| [setPageIndex(int value)](#setPageIndex-int-) | Gets or sets the index of the first page to save. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




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

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final void wait(long arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

