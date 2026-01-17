---
title: ExtendedApsPage
second_title: Aspose.Note for Java API Reference
description: Represents a wrapper for the standard ApsGlyphs which extends some of the drawing behavior.
type: docs
weight: 27
url: /java/com.aspose.note/extendedapspage/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode, com.aspose.foundation.rendering.ApsCompositeNode, com.aspose.foundation.rendering.ApsPage

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsPage extends ApsPage implements System.Collections.Generic.IGenericEnumerable<ApsNode>
```

Represents a wrapper for the standard ApsGlyphs, which extends some of the drawing behavior.
## Constructors

| Constructor | Description |
| --- | --- |
| [ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)](#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-) | Initializes a new instance of the  ExtendedApsPage  class. |
## Methods

| Method | Description |
| --- | --- |
| [accept(ApsDocumentVisitor arg0)](#accept-com.aspose.foundation.rendering.ApsDocumentVisitor-) |  |
| [add(ApsNode arg0)](#add-com.aspose.foundation.rendering.ApsNode-) |  |
| [addRange(ApsNode[] arg0)](#addRange-com.aspose.foundation.rendering.ApsNode---) |  |
| [clear()](#clear--) |  |
| [disposeIt()](#disposeIt--) |  |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAttributes()](#getAttributes--) |  |
| [getClass()](#getClass--) |  |
| [getContentSize()](#getContentSize--) | Gets the page size excluding margins. |
| [getCount()](#getCount--) |  |
| [getHeight()](#getHeight--) |  |
| [getHeightPixels()](#getHeightPixels--) |  |
| [getId()](#getId--) |  |
| [getMargin()](#getMargin--) | Gets margin of this page. |
| [getPageEndInNotePage()](#getPageEndInNotePage--) | Gets the position of the page end, in the MS OneNote page, when one MS OneNote page is divided into several aps Pages. |
| [getPageSize()](#getPageSize--) | Gets the final page size. |
| [getPageStartInNotePage()](#getPageStartInNotePage--) | Gets the position of the page start in the MS OneNote page, when one MS OneNote page is divided into several aps Pages. |
| [getPaperTray()](#getPaperTray--) |  |
| [getParent()](#getParent--) |  |
| [getSize()](#getSize--) |  |
| [getWidth()](#getWidth--) |  |
| [getWidthPixels()](#getWidthPixels--) |  |
| [get_Item(int arg0)](#get-Item-int-) |  |
| [hashCode()](#hashCode--) |  |
| [insert(int arg0, ApsNode arg1)](#insert-int-com.aspose.foundation.rendering.ApsNode-) |  |
| [isEndPage()](#isEndPage--) |  |
| [iterator()](#iterator--) | Returns the enumerator that iterates through the all nodes from this page. |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) | The get enumerator. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(ApsNode arg0)](#remove-com.aspose.foundation.rendering.ApsNode-) |  |
| [setEndPage(boolean arg0)](#setEndPage-boolean-) |  |
| [setId(String arg0)](#setId-java.lang.String-) |  |
| [setParent(ApsNode arg0)](#setParent-com.aspose.foundation.rendering.ApsNode-) |  |
| [setSize(System.Drawing.SizeF arg0)](#setSize-com.aspose.ms.System.Drawing.SizeF-) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin) {#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-}
```
public ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)
```


Initializes a new instance of the  ExtendedApsPage  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageSize | com.aspose.ms.System.Drawing.SizeF | The page size. |
| pageStartInNotePage | float | The page start in the original MS OneNote page. |
| margin | com.aspose.foundation.layout.Margin | The extended page margin. |

### accept(ApsDocumentVisitor arg0) {#accept-com.aspose.foundation.rendering.ApsDocumentVisitor-}
```
public void accept(ApsDocumentVisitor arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | com.aspose.foundation.rendering.ApsDocumentVisitor |  |

### add(ApsNode arg0) {#add-com.aspose.foundation.rendering.ApsNode-}
```
public void add(ApsNode arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | com.aspose.foundation.rendering.ApsNode |  |

### addRange(ApsNode[] arg0) {#addRange-com.aspose.foundation.rendering.ApsNode---}
```
public void addRange(ApsNode[] arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | com.aspose.foundation.rendering.ApsNode[] |  |

### clear() {#clear--}
```
public void clear()
```




### disposeIt() {#disposeIt--}
```
public void disposeIt()
```




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
### getAttributes() {#getAttributes--}
```
public ApsNodeAttributes getAttributes()
```




**Returns:**
com.aspose.foundation.rendering.ApsNodeAttributes
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getContentSize() {#getContentSize--}
```
public System.Drawing.SizeF getContentSize()
```


Gets the page size excluding margins.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getCount() {#getCount--}
```
public int getCount()
```




**Returns:**
int
### getHeight() {#getHeight--}
```
public float getHeight()
```




**Returns:**
float
### getHeightPixels() {#getHeightPixels--}
```
public int getHeightPixels()
```




**Returns:**
int
### getId() {#getId--}
```
public String getId()
```




**Returns:**
java.lang.String
### getMargin() {#getMargin--}
```
public Margin getMargin()
```


Gets margin of this page.

**Returns:**
com.aspose.foundation.layout.Margin
### getPageEndInNotePage() {#getPageEndInNotePage--}
```
public float getPageEndInNotePage()
```


Gets the position of the page end, in the MS OneNote page, when one MS OneNote page is divided into several aps Pages.

**Returns:**
float
### getPageSize() {#getPageSize--}
```
public System.Drawing.SizeF getPageSize()
```


Gets the final page size.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getPageStartInNotePage() {#getPageStartInNotePage--}
```
public float getPageStartInNotePage()
```


Gets the position of the page start in the MS OneNote page, when one MS OneNote page is divided into several aps Pages.

**Returns:**
float
### getPaperTray() {#getPaperTray--}
```
public int getPaperTray()
```




**Returns:**
int
### getParent() {#getParent--}
```
public ApsNode getParent()
```




**Returns:**
com.aspose.foundation.rendering.ApsNode
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```




**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getWidth() {#getWidth--}
```
public float getWidth()
```




**Returns:**
float
### getWidthPixels() {#getWidthPixels--}
```
public int getWidthPixels()
```




**Returns:**
int
### get_Item(int arg0) {#get-Item-int-}
```
public ApsNode get_Item(int arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | int |  |

**Returns:**
com.aspose.foundation.rendering.ApsNode
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### insert(int arg0, ApsNode arg1) {#insert-int-com.aspose.foundation.rendering.ApsNode-}
```
public void insert(int arg0, ApsNode arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | int |  |
| arg1 | com.aspose.foundation.rendering.ApsNode |  |

### isEndPage() {#isEndPage--}
```
public boolean isEndPage()
```




**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsNode> iterator()
```


Returns the enumerator that iterates through the all nodes from this page.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator<com.aspose.foundation.rendering.ApsNode> - The  IEnumerator .
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```


The get enumerator.

**Returns:**
com.aspose.ms.System.Collections.IEnumerator - The  IEnumerator .
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(ApsNode arg0) {#remove-com.aspose.foundation.rendering.ApsNode-}
```
public void remove(ApsNode arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | com.aspose.foundation.rendering.ApsNode |  |

### setEndPage(boolean arg0) {#setEndPage-boolean-}
```
public void setEndPage(boolean arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | boolean |  |

### setId(String arg0) {#setId-java.lang.String-}
```
public void setId(String arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.String |  |

### setParent(ApsNode arg0) {#setParent-com.aspose.foundation.rendering.ApsNode-}
```
public void setParent(ApsNode arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | com.aspose.foundation.rendering.ApsNode |  |

### setSize(System.Drawing.SizeF arg0) {#setSize-com.aspose.ms.System.Drawing.SizeF-}
```
public void setSize(System.Drawing.SizeF arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | com.aspose.ms.System.Drawing.SizeF |  |

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

