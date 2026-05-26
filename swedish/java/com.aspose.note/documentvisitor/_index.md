---
title: "DocumentVisitor"
second_title: "Aspose.Note for Java API-referens"
description: "Den abstrakta klassen för att iterera genom ett delträd med rot i den angivna noden."
type: docs
weight: 22
url: /sv/java/com.aspose.note/documentvisitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class DocumentVisitor
```

Den abstrakta klassen för att iterera genom ett delträd med rot i den angivna noden.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [DocumentVisitor()](#DocumentVisitor--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [visitAttachedFileEnd(AttachedFile attachedFile)](#visitAttachedFileEnd-com.aspose.note.AttachedFile-) | Slut för att besöka `AttachedFile`-noden. |
| [visitAttachedFileStart(AttachedFile attachedFile)](#visitAttachedFileStart-com.aspose.note.AttachedFile-) | Starta besöket av `AttachedFile`-noden. |
| [visitDocumentEnd(Document document)](#visitDocumentEnd-com.aspose.note.Document-) | Avsluta besöket av `Document`-noden. |
| [visitDocumentStart(Document document)](#visitDocumentStart-com.aspose.note.Document-) | Starta besöket av `Document`-noden. |
| [visitImageEnd(Image image)](#visitImageEnd-com.aspose.note.Image-) | Avsluta besöket av `Image`-noden. |
| [visitImageStart(Image image)](#visitImageStart-com.aspose.note.Image-) | Starta besöket av `Image`-noden. |
| [visitInkDrawingEnd(InkDrawing inkDrawing)](#visitInkDrawingEnd-com.aspose.note.InkDrawing-) | Avsluta besöket av [InkDrawing](../../com.aspose.note/inkdrawing) noden. |
| [visitInkDrawingStart(InkDrawing inkDrawing)](#visitInkDrawingStart-com.aspose.note.InkDrawing-) | Starta besöket av [InkDrawing](../../com.aspose.note/inkdrawing) noden. |
| [visitInkParagraphEnd(InkParagraph inkParagraph)](#visitInkParagraphEnd-com.aspose.note.InkParagraph-) | Avsluta besöket av [InkParagraph](../../com.aspose.note/inkparagraph) noden. |
| [visitInkParagraphStart(InkParagraph inkParagraph)](#visitInkParagraphStart-com.aspose.note.InkParagraph-) | Starta besöket av [InkParagraph](../../com.aspose.note/inkparagraph) noden. |
| [visitInkWordEnd(InkWord inkWord)](#visitInkWordEnd-com.aspose.note.InkWord-) | Avsluta besöket av [InkWord](../../com.aspose.note/inkword) noden. |
| [visitInkWordStart(InkWord inkWord)](#visitInkWordStart-com.aspose.note.InkWord-) | Starta besöket av [InkWord](../../com.aspose.note/inkword) noden. |
| [visitLoopEnd(Loop loop)](#visitLoopEnd-com.aspose.note.Loop-) | Avsluta besöket av [Loop](../../com.aspose.note/loop) noden. |
| [visitLoopStart(Loop loop)](#visitLoopStart-com.aspose.note.Loop-) | Starta besöket av [Loop](../../com.aspose.note/loop) noden. |
| [visitOutlineElementEnd(OutlineElement outlineElement)](#visitOutlineElementEnd-com.aspose.note.OutlineElement-) | Avsluta besöket av `OutlineElement`-noden. |
| [visitOutlineElementStart(OutlineElement outlineElement)](#visitOutlineElementStart-com.aspose.note.OutlineElement-) | Starta besöket av `OutlineElement`-noden. |
| [visitOutlineEnd(Outline outline)](#visitOutlineEnd-com.aspose.note.Outline-) | Avsluta besöket av `Outline`-noden. |
| [visitOutlineGroupEnd(OutlineGroup outlineGroup)](#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-) | Avsluta besöket av `OutlineGroup`-noden. |
| [visitOutlineGroupStart(OutlineGroup outlineGroup)](#visitOutlineGroupStart-com.aspose.note.OutlineGroup-) | Starta besöket av `OutlineGroup`-noden. |
| [visitOutlineStart(Outline outline)](#visitOutlineStart-com.aspose.note.Outline-) | Starta besöket av `Outline`-noden. |
| [visitPageEnd(Page page)](#visitPageEnd-com.aspose.note.Page-) | Avsluta besöket av `Page`-noden. |
| [visitPageStart(Page page)](#visitPageStart-com.aspose.note.Page-) | Starta besöket av `Page`-noden. |
| [visitRichTextEnd(RichText richText)](#visitRichTextEnd-com.aspose.note.RichText-) | Avsluta besöket av `RichText`-noden. |
| [visitRichTextStart(RichText richText)](#visitRichTextStart-com.aspose.note.RichText-) | Starta besöket av `RichText`-noden. |
| [visitTableCellEnd(TableCell tableCell)](#visitTableCellEnd-com.aspose.note.TableCell-) | Avsluta besöket av `TableCell`-noden. |
| [visitTableCellStart(TableCell tableCell)](#visitTableCellStart-com.aspose.note.TableCell-) | Starta besöket av `TableCell`-noden. |
| [visitTableEnd(Table table)](#visitTableEnd-com.aspose.note.Table-) | Slut på att besöka `Table`-noden. |
| [visitTableRowEnd(TableRow tableRow)](#visitTableRowEnd-com.aspose.note.TableRow-) | Slut på att besöka `TableRow`-noden. |
| [visitTableRowStart(TableRow tableRow)](#visitTableRowStart-com.aspose.note.TableRow-) | Börja besöka `TableRow`-noden. |
| [visitTableStart(Table table)](#visitTableStart-com.aspose.note.Table-) | Börja besöka `Table`-noden. |
| [visitTitleEnd(Title title)](#visitTitleEnd-com.aspose.note.Title-) | Slut på att besöka `Title`-noden. |
| [visitTitleStart(Title title)](#visitTitleStart-com.aspose.note.Title-) | Börja besöka `Title`-noden. |
### DocumentVisitor() {#DocumentVisitor--}
```
public DocumentVisitor()
```


### visitAttachedFileEnd(AttachedFile attachedFile) {#visitAttachedFileEnd-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileEnd(AttachedFile attachedFile)
```


Slut för att besöka `AttachedFile`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | Den `AttachedFile`-noden. |

### visitAttachedFileStart(AttachedFile attachedFile) {#visitAttachedFileStart-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileStart(AttachedFile attachedFile)
```


Starta besöket av `AttachedFile`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | Den `AttachedFile`-noden. |

### visitDocumentEnd(Document document) {#visitDocumentEnd-com.aspose.note.Document-}
```
public void visitDocumentEnd(Document document)
```


Avsluta besöket av `Document`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | Den `Document`-noden. |

### visitDocumentStart(Document document) {#visitDocumentStart-com.aspose.note.Document-}
```
public void visitDocumentStart(Document document)
```


Starta besöket av `Document`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | Den `Document`-noden. |

### visitImageEnd(Image image) {#visitImageEnd-com.aspose.note.Image-}
```
public void visitImageEnd(Image image)
```


Avsluta besöket av `Image`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | Den `Image`-noden. |

### visitImageStart(Image image) {#visitImageStart-com.aspose.note.Image-}
```
public void visitImageStart(Image image)
```


Starta besöket av `Image`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | Den `Image`-noden. |

### visitInkDrawingEnd(InkDrawing inkDrawing) {#visitInkDrawingEnd-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingEnd(InkDrawing inkDrawing)
```


Avsluta besöket av [InkDrawing](../../com.aspose.note/inkdrawing) noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | Den [InkDrawing](../../com.aspose.note/inkdrawing) noden. |

### visitInkDrawingStart(InkDrawing inkDrawing) {#visitInkDrawingStart-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingStart(InkDrawing inkDrawing)
```


Starta besöket av [InkDrawing](../../com.aspose.note/inkdrawing) noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | Den [InkDrawing](../../com.aspose.note/inkdrawing) noden. |

### visitInkParagraphEnd(InkParagraph inkParagraph) {#visitInkParagraphEnd-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphEnd(InkParagraph inkParagraph)
```


Avsluta besöket av [InkParagraph](../../com.aspose.note/inkparagraph) noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | Den [InkParagraph](../../com.aspose.note/inkparagraph) noden. |

### visitInkParagraphStart(InkParagraph inkParagraph) {#visitInkParagraphStart-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphStart(InkParagraph inkParagraph)
```


Starta besöket av [InkParagraph](../../com.aspose.note/inkparagraph) noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | Den [InkParagraph](../../com.aspose.note/inkparagraph) noden. |

### visitInkWordEnd(InkWord inkWord) {#visitInkWordEnd-com.aspose.note.InkWord-}
```
public void visitInkWordEnd(InkWord inkWord)
```


Avsluta besöket av [InkWord](../../com.aspose.note/inkword) noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | Den [InkWord](../../com.aspose.note/inkword) noden. |

### visitInkWordStart(InkWord inkWord) {#visitInkWordStart-com.aspose.note.InkWord-}
```
public void visitInkWordStart(InkWord inkWord)
```


Starta besöket av [InkWord](../../com.aspose.note/inkword) noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | Den [InkWord](../../com.aspose.note/inkword) noden. |

### visitLoopEnd(Loop loop) {#visitLoopEnd-com.aspose.note.Loop-}
```
public void visitLoopEnd(Loop loop)
```


Avsluta besöket av [Loop](../../com.aspose.note/loop) noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | Den [Loop](../../com.aspose.note/loop) noden. |

### visitLoopStart(Loop loop) {#visitLoopStart-com.aspose.note.Loop-}
```
public void visitLoopStart(Loop loop)
```


Starta besöket av [Loop](../../com.aspose.note/loop) noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | Den [Loop](../../com.aspose.note/loop) noden. |

### visitOutlineElementEnd(OutlineElement outlineElement) {#visitOutlineElementEnd-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementEnd(OutlineElement outlineElement)
```


Avsluta besöket av `OutlineElement`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | Den `OutlineElement`-noden. |

### visitOutlineElementStart(OutlineElement outlineElement) {#visitOutlineElementStart-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementStart(OutlineElement outlineElement)
```


Starta besöket av `OutlineElement`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | Den `OutlineElement`-noden. |

### visitOutlineEnd(Outline outline) {#visitOutlineEnd-com.aspose.note.Outline-}
```
public void visitOutlineEnd(Outline outline)
```


Avsluta besöket av `Outline`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | Den `Outline`-noden. |

### visitOutlineGroupEnd(OutlineGroup outlineGroup) {#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupEnd(OutlineGroup outlineGroup)
```


Avsluta besöket av `OutlineGroup`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | Den `OutlineGroup`-noden. |

### visitOutlineGroupStart(OutlineGroup outlineGroup) {#visitOutlineGroupStart-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupStart(OutlineGroup outlineGroup)
```


Starta besöket av `OutlineGroup`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | Den `OutlineGroup`-noden. |

### visitOutlineStart(Outline outline) {#visitOutlineStart-com.aspose.note.Outline-}
```
public void visitOutlineStart(Outline outline)
```


Starta besöket av `Outline`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | Den `Outline`-noden. |

### visitPageEnd(Page page) {#visitPageEnd-com.aspose.note.Page-}
```
public void visitPageEnd(Page page)
```


Avsluta besöket av `Page`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Den `Page`-noden. |

### visitPageStart(Page page) {#visitPageStart-com.aspose.note.Page-}
```
public void visitPageStart(Page page)
```


Starta besöket av `Page`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Den `Page`-noden. |

### visitRichTextEnd(RichText richText) {#visitRichTextEnd-com.aspose.note.RichText-}
```
public void visitRichTextEnd(RichText richText)
```


Avsluta besöket av `RichText`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | Den `RichText`-noden. |

### visitRichTextStart(RichText richText) {#visitRichTextStart-com.aspose.note.RichText-}
```
public void visitRichTextStart(RichText richText)
```


Starta besöket av `RichText`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | Den `RichText`-noden. |

### visitTableCellEnd(TableCell tableCell) {#visitTableCellEnd-com.aspose.note.TableCell-}
```
public void visitTableCellEnd(TableCell tableCell)
```


Avsluta besöket av `TableCell`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | Den `TableCell`-noden. |

### visitTableCellStart(TableCell tableCell) {#visitTableCellStart-com.aspose.note.TableCell-}
```
public void visitTableCellStart(TableCell tableCell)
```


Starta besöket av `TableCell`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | Den `TableCell`-noden. |

### visitTableEnd(Table table) {#visitTableEnd-com.aspose.note.Table-}
```
public void visitTableEnd(Table table)
```


Slut på att besöka `Table`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | Den `Table`-noden. |

### visitTableRowEnd(TableRow tableRow) {#visitTableRowEnd-com.aspose.note.TableRow-}
```
public void visitTableRowEnd(TableRow tableRow)
```


Slut på att besöka `TableRow`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | Den `TableRow`-noden. |

### visitTableRowStart(TableRow tableRow) {#visitTableRowStart-com.aspose.note.TableRow-}
```
public void visitTableRowStart(TableRow tableRow)
```


Börja besöka `TableRow`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | Den `TableRow`-noden. |

### visitTableStart(Table table) {#visitTableStart-com.aspose.note.Table-}
```
public void visitTableStart(Table table)
```


Börja besöka `Table`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | Den `Table`-noden. |

### visitTitleEnd(Title title) {#visitTitleEnd-com.aspose.note.Title-}
```
public void visitTitleEnd(Title title)
```


Slut på att besöka `Title`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | Den `Title`-noden. |

### visitTitleStart(Title title) {#visitTitleStart-com.aspose.note.Title-}
```
public void visitTitleStart(Title title)
```


Börja besöka `Title`-noden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | Den `Title`-noden. |

