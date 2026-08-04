---
title: DocumentVisitor
second_title: Aspose.Note for Java API Reference
description: The abstract class for iterating through subtree with root at the specified node.
type: docs
weight: 22
url: /java/com.aspose.note/documentvisitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class DocumentVisitor
```

The abstract class for iterating through subtree with root at the specified node.
## Constructors

| Constructor | Description |
| --- | --- |
| [DocumentVisitor()](#DocumentVisitor--) |  |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [visitAttachedFileEnd(AttachedFile attachedFile)](#visitAttachedFileEnd-com.aspose.note.AttachedFile-) | End to visit the  AttachedFile  node. |
| [visitAttachedFileStart(AttachedFile attachedFile)](#visitAttachedFileStart-com.aspose.note.AttachedFile-) | Start to visit the  AttachedFile  node. |
| [visitDocumentEnd(Document document)](#visitDocumentEnd-com.aspose.note.Document-) | End to visit the  Document  node. |
| [visitDocumentStart(Document document)](#visitDocumentStart-com.aspose.note.Document-) | Start to visit the  Document  node. |
| [visitImageEnd(Image image)](#visitImageEnd-com.aspose.note.Image-) | End to visit the  Image  node. |
| [visitImageStart(Image image)](#visitImageStart-com.aspose.note.Image-) | Start to visit the  Image  node. |
| [visitInkDrawingEnd(InkDrawing inkDrawing)](#visitInkDrawingEnd-com.aspose.note.InkDrawing-) | End to visit the [InkDrawing](../../com.aspose.note/inkdrawing) node. |
| [visitInkDrawingStart(InkDrawing inkDrawing)](#visitInkDrawingStart-com.aspose.note.InkDrawing-) | Start to visit the [InkDrawing](../../com.aspose.note/inkdrawing) node. |
| [visitInkParagraphEnd(InkParagraph inkParagraph)](#visitInkParagraphEnd-com.aspose.note.InkParagraph-) | End to visit the [InkParagraph](../../com.aspose.note/inkparagraph) node. |
| [visitInkParagraphStart(InkParagraph inkParagraph)](#visitInkParagraphStart-com.aspose.note.InkParagraph-) | Start to visit the [InkParagraph](../../com.aspose.note/inkparagraph) node. |
| [visitInkWordEnd(InkWord inkWord)](#visitInkWordEnd-com.aspose.note.InkWord-) | End to visit the [InkWord](../../com.aspose.note/inkword) node. |
| [visitInkWordStart(InkWord inkWord)](#visitInkWordStart-com.aspose.note.InkWord-) | Start to visit the [InkWord](../../com.aspose.note/inkword) node. |
| [visitLoopEnd(Loop loop)](#visitLoopEnd-com.aspose.note.Loop-) | End to visit the [Loop](../../com.aspose.note/loop) node. |
| [visitLoopStart(Loop loop)](#visitLoopStart-com.aspose.note.Loop-) | Start to visit the [Loop](../../com.aspose.note/loop) node. |
| [visitOutlineElementEnd(OutlineElement outlineElement)](#visitOutlineElementEnd-com.aspose.note.OutlineElement-) | End to visit the  OutlineElement  node. |
| [visitOutlineElementStart(OutlineElement outlineElement)](#visitOutlineElementStart-com.aspose.note.OutlineElement-) | Start to visit the  OutlineElement  node. |
| [visitOutlineEnd(Outline outline)](#visitOutlineEnd-com.aspose.note.Outline-) | End to visit the  Outline  node. |
| [visitOutlineGroupEnd(OutlineGroup outlineGroup)](#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-) | End to visit the  OutlineGroup  node. |
| [visitOutlineGroupStart(OutlineGroup outlineGroup)](#visitOutlineGroupStart-com.aspose.note.OutlineGroup-) | Start to visit the  OutlineGroup  node. |
| [visitOutlineStart(Outline outline)](#visitOutlineStart-com.aspose.note.Outline-) | Start to visit the  Outline  node. |
| [visitPageEnd(Page page)](#visitPageEnd-com.aspose.note.Page-) | End to visit the  Page  node. |
| [visitPageStart(Page page)](#visitPageStart-com.aspose.note.Page-) | Start to visit the  Page  node. |
| [visitRichTextEnd(RichText richText)](#visitRichTextEnd-com.aspose.note.RichText-) | End to visit the  RichText  node. |
| [visitRichTextStart(RichText richText)](#visitRichTextStart-com.aspose.note.RichText-) | Start to visit the  RichText  node. |
| [visitTableCellEnd(TableCell tableCell)](#visitTableCellEnd-com.aspose.note.TableCell-) | End to visit the  TableCell  node. |
| [visitTableCellStart(TableCell tableCell)](#visitTableCellStart-com.aspose.note.TableCell-) | Start to visit the  TableCell  node. |
| [visitTableEnd(Table table)](#visitTableEnd-com.aspose.note.Table-) | End to visit the  Table  node. |
| [visitTableRowEnd(TableRow tableRow)](#visitTableRowEnd-com.aspose.note.TableRow-) | End to visit the  TableRow  node. |
| [visitTableRowStart(TableRow tableRow)](#visitTableRowStart-com.aspose.note.TableRow-) | Start to visit the  TableRow  node. |
| [visitTableStart(Table table)](#visitTableStart-com.aspose.note.Table-) | Start to visit the  Table  node. |
| [visitTitleEnd(Title title)](#visitTitleEnd-com.aspose.note.Title-) | End to visit the  Title  node. |
| [visitTitleStart(Title title)](#visitTitleStart-com.aspose.note.Title-) | Start to visit the  Title  node. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DocumentVisitor() {#DocumentVisitor--}
```
public DocumentVisitor()
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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




### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### visitAttachedFileEnd(AttachedFile attachedFile) {#visitAttachedFileEnd-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileEnd(AttachedFile attachedFile)
```


End to visit the  AttachedFile  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | The  AttachedFile  node. |

### visitAttachedFileStart(AttachedFile attachedFile) {#visitAttachedFileStart-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileStart(AttachedFile attachedFile)
```


Start to visit the  AttachedFile  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | The  AttachedFile  node. |

### visitDocumentEnd(Document document) {#visitDocumentEnd-com.aspose.note.Document-}
```
public void visitDocumentEnd(Document document)
```


End to visit the  Document  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | The  Document  node. |

### visitDocumentStart(Document document) {#visitDocumentStart-com.aspose.note.Document-}
```
public void visitDocumentStart(Document document)
```


Start to visit the  Document  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | The  Document  node. |

### visitImageEnd(Image image) {#visitImageEnd-com.aspose.note.Image-}
```
public void visitImageEnd(Image image)
```


End to visit the  Image  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | The  Image  node. |

### visitImageStart(Image image) {#visitImageStart-com.aspose.note.Image-}
```
public void visitImageStart(Image image)
```


Start to visit the  Image  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | The  Image  node. |

### visitInkDrawingEnd(InkDrawing inkDrawing) {#visitInkDrawingEnd-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingEnd(InkDrawing inkDrawing)
```


End to visit the [InkDrawing](../../com.aspose.note/inkdrawing) node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | The [InkDrawing](../../com.aspose.note/inkdrawing) node. |

### visitInkDrawingStart(InkDrawing inkDrawing) {#visitInkDrawingStart-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingStart(InkDrawing inkDrawing)
```


Start to visit the [InkDrawing](../../com.aspose.note/inkdrawing) node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | The [InkDrawing](../../com.aspose.note/inkdrawing) node. |

### visitInkParagraphEnd(InkParagraph inkParagraph) {#visitInkParagraphEnd-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphEnd(InkParagraph inkParagraph)
```


End to visit the [InkParagraph](../../com.aspose.note/inkparagraph) node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | The [InkParagraph](../../com.aspose.note/inkparagraph) node. |

### visitInkParagraphStart(InkParagraph inkParagraph) {#visitInkParagraphStart-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphStart(InkParagraph inkParagraph)
```


Start to visit the [InkParagraph](../../com.aspose.note/inkparagraph) node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | The [InkParagraph](../../com.aspose.note/inkparagraph) node. |

### visitInkWordEnd(InkWord inkWord) {#visitInkWordEnd-com.aspose.note.InkWord-}
```
public void visitInkWordEnd(InkWord inkWord)
```


End to visit the [InkWord](../../com.aspose.note/inkword) node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | The [InkWord](../../com.aspose.note/inkword) node. |

### visitInkWordStart(InkWord inkWord) {#visitInkWordStart-com.aspose.note.InkWord-}
```
public void visitInkWordStart(InkWord inkWord)
```


Start to visit the [InkWord](../../com.aspose.note/inkword) node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | The [InkWord](../../com.aspose.note/inkword) node. |

### visitLoopEnd(Loop loop) {#visitLoopEnd-com.aspose.note.Loop-}
```
public void visitLoopEnd(Loop loop)
```


End to visit the [Loop](../../com.aspose.note/loop) node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | The [Loop](../../com.aspose.note/loop) node. |

### visitLoopStart(Loop loop) {#visitLoopStart-com.aspose.note.Loop-}
```
public void visitLoopStart(Loop loop)
```


Start to visit the [Loop](../../com.aspose.note/loop) node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | The [Loop](../../com.aspose.note/loop) node. |

### visitOutlineElementEnd(OutlineElement outlineElement) {#visitOutlineElementEnd-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementEnd(OutlineElement outlineElement)
```


End to visit the  OutlineElement  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | The  OutlineElement  node. |

### visitOutlineElementStart(OutlineElement outlineElement) {#visitOutlineElementStart-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementStart(OutlineElement outlineElement)
```


Start to visit the  OutlineElement  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | The  OutlineElement  node. |

### visitOutlineEnd(Outline outline) {#visitOutlineEnd-com.aspose.note.Outline-}
```
public void visitOutlineEnd(Outline outline)
```


End to visit the  Outline  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | The  Outline  node. |

### visitOutlineGroupEnd(OutlineGroup outlineGroup) {#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupEnd(OutlineGroup outlineGroup)
```


End to visit the  OutlineGroup  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | The  OutlineGroup  node. |

### visitOutlineGroupStart(OutlineGroup outlineGroup) {#visitOutlineGroupStart-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupStart(OutlineGroup outlineGroup)
```


Start to visit the  OutlineGroup  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | The  OutlineGroup  node. |

### visitOutlineStart(Outline outline) {#visitOutlineStart-com.aspose.note.Outline-}
```
public void visitOutlineStart(Outline outline)
```


Start to visit the  Outline  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | The  Outline  node. |

### visitPageEnd(Page page) {#visitPageEnd-com.aspose.note.Page-}
```
public void visitPageEnd(Page page)
```


End to visit the  Page  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | The  Page  node. |

### visitPageStart(Page page) {#visitPageStart-com.aspose.note.Page-}
```
public void visitPageStart(Page page)
```


Start to visit the  Page  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | The  Page  node. |

### visitRichTextEnd(RichText richText) {#visitRichTextEnd-com.aspose.note.RichText-}
```
public void visitRichTextEnd(RichText richText)
```


End to visit the  RichText  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | The  RichText  node. |

### visitRichTextStart(RichText richText) {#visitRichTextStart-com.aspose.note.RichText-}
```
public void visitRichTextStart(RichText richText)
```


Start to visit the  RichText  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | The  RichText  node. |

### visitTableCellEnd(TableCell tableCell) {#visitTableCellEnd-com.aspose.note.TableCell-}
```
public void visitTableCellEnd(TableCell tableCell)
```


End to visit the  TableCell  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | The  TableCell  node. |

### visitTableCellStart(TableCell tableCell) {#visitTableCellStart-com.aspose.note.TableCell-}
```
public void visitTableCellStart(TableCell tableCell)
```


Start to visit the  TableCell  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | The  TableCell  node. |

### visitTableEnd(Table table) {#visitTableEnd-com.aspose.note.Table-}
```
public void visitTableEnd(Table table)
```


End to visit the  Table  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | The  Table  node. |

### visitTableRowEnd(TableRow tableRow) {#visitTableRowEnd-com.aspose.note.TableRow-}
```
public void visitTableRowEnd(TableRow tableRow)
```


End to visit the  TableRow  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | The  TableRow  node. |

### visitTableRowStart(TableRow tableRow) {#visitTableRowStart-com.aspose.note.TableRow-}
```
public void visitTableRowStart(TableRow tableRow)
```


Start to visit the  TableRow  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | The  TableRow  node. |

### visitTableStart(Table table) {#visitTableStart-com.aspose.note.Table-}
```
public void visitTableStart(Table table)
```


Start to visit the  Table  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | The  Table  node. |

### visitTitleEnd(Title title) {#visitTitleEnd-com.aspose.note.Title-}
```
public void visitTitleEnd(Title title)
```


End to visit the  Title  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | The  Title  node. |

### visitTitleStart(Title title) {#visitTitleStart-com.aspose.note.Title-}
```
public void visitTitleStart(Title title)
```


Start to visit the  Title  node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | The  Title  node. |

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

