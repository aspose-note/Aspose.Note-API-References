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
| [ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)](#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-) | Initializes a new instance of the `ExtendedApsPage` class. |
## Methods

| Method | Description |
| --- | --- |
| [getContentSize()](#getContentSize--) | Gets the page size excluding margins. |
| [getMargin()](#getMargin--) | Gets margin of this page. |
| [getPageEndInNotePage()](#getPageEndInNotePage--) | Gets the position of the page end, in the MS OneNote page, when one MS OneNote page is divided into several aps Pages. |
| [getPageSize()](#getPageSize--) | Gets the final page size. |
| [getPageStartInNotePage()](#getPageStartInNotePage--) | Gets the position of the page start in the MS OneNote page, when one MS OneNote page is divided into several aps Pages. |
| [iterator()](#iterator--) | Returns the enumerator that iterates through the all nodes from this page. |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) | The get enumerator. |
### ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin) {#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-}
```
public ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)
```


Initializes a new instance of the `ExtendedApsPage` class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageSize | com.aspose.ms.System.Drawing.SizeF | The page size. |
| pageStartInNotePage | float | The page start in the original MS OneNote page. |
| margin | com.aspose.foundation.layout.Margin | The extended page margin. |

### getContentSize() {#getContentSize--}
```
public System.Drawing.SizeF getContentSize()
```


Gets the page size excluding margins.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
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
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsNode> iterator()
```


Returns the enumerator that iterates through the all nodes from this page.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsNode&gt; - The `IEnumerator`.
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```


The get enumerator.

**Returns:**
com.aspose.ms.System.Collections.IEnumerator - The `IEnumerator`.
