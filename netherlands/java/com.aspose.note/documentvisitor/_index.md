---
title: "DocumentVisitor"
second_title: "Aspose.Note for Java API-referentie"
description: "De abstracte klasse voor het itereren door een subboom met wortel op het opgegeven knooppunt."
type: docs
weight: 22
url: /nl/java/com.aspose.note/documentvisitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class DocumentVisitor
```

De abstracte klasse voor het itereren door een subboom met wortel op het opgegeven knooppunt.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [DocumentVisitor()](#DocumentVisitor--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [visitAttachedFileEnd(AttachedFile attachedFile)](#visitAttachedFileEnd-com.aspose.note.AttachedFile-) | Einde om het `AttachedFile`-knooppunt te bezoeken. |
| [visitAttachedFileStart(AttachedFile attachedFile)](#visitAttachedFileStart-com.aspose.note.AttachedFile-) | Start met het bezoeken van de `AttachedFile` node. |
| [visitDocumentEnd(Document document)](#visitDocumentEnd-com.aspose.note.Document-) | Einde van het bezoeken van de `Document` node. |
| [visitDocumentStart(Document document)](#visitDocumentStart-com.aspose.note.Document-) | Start met het bezoeken van de `Document` node. |
| [visitImageEnd(Image image)](#visitImageEnd-com.aspose.note.Image-) | Einde van het bezoeken van de `Image` node. |
| [visitImageStart(Image image)](#visitImageStart-com.aspose.note.Image-) | Start met het bezoeken van de `Image` node. |
| [visitInkDrawingEnd(InkDrawing inkDrawing)](#visitInkDrawingEnd-com.aspose.note.InkDrawing-) | Einde van het bezoeken van de [InkDrawing](../../com.aspose.note/inkdrawing) node. |
| [visitInkDrawingStart(InkDrawing inkDrawing)](#visitInkDrawingStart-com.aspose.note.InkDrawing-) | Start met het bezoeken van de [InkDrawing](../../com.aspose.note/inkdrawing) node. |
| [visitInkParagraphEnd(InkParagraph inkParagraph)](#visitInkParagraphEnd-com.aspose.note.InkParagraph-) | Einde van het bezoeken van de [InkParagraph](../../com.aspose.note/inkparagraph) node. |
| [visitInkParagraphStart(InkParagraph inkParagraph)](#visitInkParagraphStart-com.aspose.note.InkParagraph-) | Start met het bezoeken van de [InkParagraph](../../com.aspose.note/inkparagraph) node. |
| [visitInkWordEnd(InkWord inkWord)](#visitInkWordEnd-com.aspose.note.InkWord-) | Einde van het bezoeken van de [InkWord](../../com.aspose.note/inkword) node. |
| [visitInkWordStart(InkWord inkWord)](#visitInkWordStart-com.aspose.note.InkWord-) | Start met het bezoeken van de [InkWord](../../com.aspose.note/inkword) node. |
| [visitLoopEnd(Loop loop)](#visitLoopEnd-com.aspose.note.Loop-) | Einde van het bezoeken van de [Loop](../../com.aspose.note/loop) node. |
| [visitLoopStart(Loop loop)](#visitLoopStart-com.aspose.note.Loop-) | Start met het bezoeken van de [Loop](../../com.aspose.note/loop) node. |
| [visitOutlineElementEnd(OutlineElement outlineElement)](#visitOutlineElementEnd-com.aspose.note.OutlineElement-) | Einde van het bezoeken van de `OutlineElement` node. |
| [visitOutlineElementStart(OutlineElement outlineElement)](#visitOutlineElementStart-com.aspose.note.OutlineElement-) | Start met het bezoeken van de `OutlineElement` node. |
| [visitOutlineEnd(Outline outline)](#visitOutlineEnd-com.aspose.note.Outline-) | Einde van het bezoeken van de `Outline` node. |
| [visitOutlineGroupEnd(OutlineGroup outlineGroup)](#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-) | Einde van het bezoeken van de `OutlineGroup` node. |
| [visitOutlineGroupStart(OutlineGroup outlineGroup)](#visitOutlineGroupStart-com.aspose.note.OutlineGroup-) | Start met het bezoeken van de `OutlineGroup` node. |
| [visitOutlineStart(Outline outline)](#visitOutlineStart-com.aspose.note.Outline-) | Start met het bezoeken van de `Outline` node. |
| [visitPageEnd(Page page)](#visitPageEnd-com.aspose.note.Page-) | Einde van het bezoeken van de `Page` node. |
| [visitPageStart(Page page)](#visitPageStart-com.aspose.note.Page-) | Start met het bezoeken van de `Page` node. |
| [visitRichTextEnd(RichText richText)](#visitRichTextEnd-com.aspose.note.RichText-) | Einde van het bezoeken van de `RichText` node. |
| [visitRichTextStart(RichText richText)](#visitRichTextStart-com.aspose.note.RichText-) | Start met het bezoeken van de `RichText` node. |
| [visitTableCellEnd(TableCell tableCell)](#visitTableCellEnd-com.aspose.note.TableCell-) | Einde van het bezoeken van de `TableCell` node. |
| [visitTableCellStart(TableCell tableCell)](#visitTableCellStart-com.aspose.note.TableCell-) | Start met het bezoeken van de `TableCell` node. |
| [visitTableEnd(Table table)](#visitTableEnd-com.aspose.note.Table-) | Einde om de `Table` node te bezoeken. |
| [visitTableRowEnd(TableRow tableRow)](#visitTableRowEnd-com.aspose.note.TableRow-) | Einde om de `TableRow` node te bezoeken. |
| [visitTableRowStart(TableRow tableRow)](#visitTableRowStart-com.aspose.note.TableRow-) | Begin om de `TableRow` node te bezoeken. |
| [visitTableStart(Table table)](#visitTableStart-com.aspose.note.Table-) | Begin om de `Table` node te bezoeken. |
| [visitTitleEnd(Title title)](#visitTitleEnd-com.aspose.note.Title-) | Einde om de `Title` node te bezoeken. |
| [visitTitleStart(Title title)](#visitTitleStart-com.aspose.note.Title-) | Begin om de `Title` node te bezoeken. |
### DocumentVisitor() {#DocumentVisitor--}
```
public DocumentVisitor()
```


### visitAttachedFileEnd(AttachedFile attachedFile) {#visitAttachedFileEnd-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileEnd(AttachedFile attachedFile)
```


Einde om het `AttachedFile`-knooppunt te bezoeken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | De `AttachedFile` node. |

### visitAttachedFileStart(AttachedFile attachedFile) {#visitAttachedFileStart-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileStart(AttachedFile attachedFile)
```


Start met het bezoeken van de `AttachedFile` node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | De `AttachedFile` node. |

### visitDocumentEnd(Document document) {#visitDocumentEnd-com.aspose.note.Document-}
```
public void visitDocumentEnd(Document document)
```


Einde van het bezoeken van de `Document` node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | De `Document` node. |

### visitDocumentStart(Document document) {#visitDocumentStart-com.aspose.note.Document-}
```
public void visitDocumentStart(Document document)
```


Start met het bezoeken van de `Document` node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | De `Document` node. |

### visitImageEnd(Image image) {#visitImageEnd-com.aspose.note.Image-}
```
public void visitImageEnd(Image image)
```


Einde van het bezoeken van de `Image` node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | De `Image` node. |

### visitImageStart(Image image) {#visitImageStart-com.aspose.note.Image-}
```
public void visitImageStart(Image image)
```


Start met het bezoeken van de `Image` node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | De `Image` node. |

### visitInkDrawingEnd(InkDrawing inkDrawing) {#visitInkDrawingEnd-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingEnd(InkDrawing inkDrawing)
```


Einde van het bezoeken van de [InkDrawing](../../com.aspose.note/inkdrawing) node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | De [InkDrawing](../../com.aspose.note/inkdrawing) node. |

### visitInkDrawingStart(InkDrawing inkDrawing) {#visitInkDrawingStart-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingStart(InkDrawing inkDrawing)
```


Start met het bezoeken van de [InkDrawing](../../com.aspose.note/inkdrawing) node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | De [InkDrawing](../../com.aspose.note/inkdrawing) node. |

### visitInkParagraphEnd(InkParagraph inkParagraph) {#visitInkParagraphEnd-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphEnd(InkParagraph inkParagraph)
```


Einde van het bezoeken van de [InkParagraph](../../com.aspose.note/inkparagraph) node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | De [InkParagraph](../../com.aspose.note/inkparagraph) node. |

### visitInkParagraphStart(InkParagraph inkParagraph) {#visitInkParagraphStart-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphStart(InkParagraph inkParagraph)
```


Start met het bezoeken van de [InkParagraph](../../com.aspose.note/inkparagraph) node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | De [InkParagraph](../../com.aspose.note/inkparagraph) node. |

### visitInkWordEnd(InkWord inkWord) {#visitInkWordEnd-com.aspose.note.InkWord-}
```
public void visitInkWordEnd(InkWord inkWord)
```


Einde van het bezoeken van de [InkWord](../../com.aspose.note/inkword) node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | De [InkWord](../../com.aspose.note/inkword) node. |

### visitInkWordStart(InkWord inkWord) {#visitInkWordStart-com.aspose.note.InkWord-}
```
public void visitInkWordStart(InkWord inkWord)
```


Start met het bezoeken van de [InkWord](../../com.aspose.note/inkword) node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | De [InkWord](../../com.aspose.note/inkword) node. |

### visitLoopEnd(Loop loop) {#visitLoopEnd-com.aspose.note.Loop-}
```
public void visitLoopEnd(Loop loop)
```


Einde van het bezoeken van de [Loop](../../com.aspose.note/loop) node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | De [Loop](../../com.aspose.note/loop) node. |

### visitLoopStart(Loop loop) {#visitLoopStart-com.aspose.note.Loop-}
```
public void visitLoopStart(Loop loop)
```


Start met het bezoeken van de [Loop](../../com.aspose.note/loop) node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | De [Loop](../../com.aspose.note/loop) node. |

### visitOutlineElementEnd(OutlineElement outlineElement) {#visitOutlineElementEnd-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementEnd(OutlineElement outlineElement)
```


Einde van het bezoeken van de `OutlineElement` node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | De `OutlineElement` node. |

### visitOutlineElementStart(OutlineElement outlineElement) {#visitOutlineElementStart-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementStart(OutlineElement outlineElement)
```


Start met het bezoeken van de `OutlineElement` node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | De `OutlineElement` node. |

### visitOutlineEnd(Outline outline) {#visitOutlineEnd-com.aspose.note.Outline-}
```
public void visitOutlineEnd(Outline outline)
```


Einde van het bezoeken van de `Outline` node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | De `Outline` node. |

### visitOutlineGroupEnd(OutlineGroup outlineGroup) {#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupEnd(OutlineGroup outlineGroup)
```


Einde van het bezoeken van de `OutlineGroup` node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | De `OutlineGroup` node. |

### visitOutlineGroupStart(OutlineGroup outlineGroup) {#visitOutlineGroupStart-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupStart(OutlineGroup outlineGroup)
```


Start met het bezoeken van de `OutlineGroup` node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | De `OutlineGroup` node. |

### visitOutlineStart(Outline outline) {#visitOutlineStart-com.aspose.note.Outline-}
```
public void visitOutlineStart(Outline outline)
```


Start met het bezoeken van de `Outline` node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | De `Outline` node. |

### visitPageEnd(Page page) {#visitPageEnd-com.aspose.note.Page-}
```
public void visitPageEnd(Page page)
```


Einde van het bezoeken van de `Page` node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | De `Page` node. |

### visitPageStart(Page page) {#visitPageStart-com.aspose.note.Page-}
```
public void visitPageStart(Page page)
```


Start met het bezoeken van de `Page` node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | De `Page` node. |

### visitRichTextEnd(RichText richText) {#visitRichTextEnd-com.aspose.note.RichText-}
```
public void visitRichTextEnd(RichText richText)
```


Einde van het bezoeken van de `RichText` node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | De `RichText` node. |

### visitRichTextStart(RichText richText) {#visitRichTextStart-com.aspose.note.RichText-}
```
public void visitRichTextStart(RichText richText)
```


Start met het bezoeken van de `RichText` node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | De `RichText` node. |

### visitTableCellEnd(TableCell tableCell) {#visitTableCellEnd-com.aspose.note.TableCell-}
```
public void visitTableCellEnd(TableCell tableCell)
```


Einde van het bezoeken van de `TableCell` node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | De `TableCell` node. |

### visitTableCellStart(TableCell tableCell) {#visitTableCellStart-com.aspose.note.TableCell-}
```
public void visitTableCellStart(TableCell tableCell)
```


Start met het bezoeken van de `TableCell` node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | De `TableCell` node. |

### visitTableEnd(Table table) {#visitTableEnd-com.aspose.note.Table-}
```
public void visitTableEnd(Table table)
```


Einde om de `Table` node te bezoeken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | De `Table` node. |

### visitTableRowEnd(TableRow tableRow) {#visitTableRowEnd-com.aspose.note.TableRow-}
```
public void visitTableRowEnd(TableRow tableRow)
```


Einde om de `TableRow` node te bezoeken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | De `TableRow` node. |

### visitTableRowStart(TableRow tableRow) {#visitTableRowStart-com.aspose.note.TableRow-}
```
public void visitTableRowStart(TableRow tableRow)
```


Begin om de `TableRow` node te bezoeken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | De `TableRow` node. |

### visitTableStart(Table table) {#visitTableStart-com.aspose.note.Table-}
```
public void visitTableStart(Table table)
```


Begin om de `Table` node te bezoeken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | De `Table` node. |

### visitTitleEnd(Title title) {#visitTitleEnd-com.aspose.note.Title-}
```
public void visitTitleEnd(Title title)
```


Einde om de `Title` node te bezoeken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | De `Title` node. |

### visitTitleStart(Title title) {#visitTitleStart-com.aspose.note.Title-}
```
public void visitTitleStart(Title title)
```


Begin om de `Title` node te bezoeken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | De `Title` node. |

