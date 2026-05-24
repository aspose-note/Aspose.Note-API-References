---
title: "DocumentVisitor"
second_title: "Aspose.Note für Java API-Referenz"
description: "Die abstrakte Klasse zum Durchlaufen eines Teilbaums mit Wurzel am angegebenen Knoten."
type: docs
weight: 22
url: /de/java/com.aspose.note/documentvisitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class DocumentVisitor
```

Die abstrakte Klasse zum Durchlaufen eines Teilbaums mit Wurzel am angegebenen Knoten.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [DocumentVisitor()](#DocumentVisitor--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [visitAttachedFileEnd(AttachedFile attachedFile)](#visitAttachedFileEnd-com.aspose.note.AttachedFile-) | Ende, um den `AttachedFile`-Knoten zu besuchen. |
| [visitAttachedFileStart(AttachedFile attachedFile)](#visitAttachedFileStart-com.aspose.note.AttachedFile-) | Starten Sie den Besuch des Knotens `AttachedFile`. |
| [visitDocumentEnd(Document document)](#visitDocumentEnd-com.aspose.note.Document-) | Beenden Sie den Besuch des Knotens `Document`. |
| [visitDocumentStart(Document document)](#visitDocumentStart-com.aspose.note.Document-) | Starten Sie den Besuch des Knotens `Document`. |
| [visitImageEnd(Image image)](#visitImageEnd-com.aspose.note.Image-) | Beenden Sie den Besuch des Knotens `Image`. |
| [visitImageStart(Image image)](#visitImageStart-com.aspose.note.Image-) | Starten Sie den Besuch des Knotens `Image`. |
| [visitInkDrawingEnd(InkDrawing inkDrawing)](#visitInkDrawingEnd-com.aspose.note.InkDrawing-) | Beenden Sie den Besuch des Knotens [InkDrawing](../../com.aspose.note/inkdrawing). |
| [visitInkDrawingStart(InkDrawing inkDrawing)](#visitInkDrawingStart-com.aspose.note.InkDrawing-) | Starten Sie den Besuch des Knotens [InkDrawing](../../com.aspose.note/inkdrawing). |
| [visitInkParagraphEnd(InkParagraph inkParagraph)](#visitInkParagraphEnd-com.aspose.note.InkParagraph-) | Beenden Sie den Besuch des Knotens [InkParagraph](../../com.aspose.note/inkparagraph). |
| [visitInkParagraphStart(InkParagraph inkParagraph)](#visitInkParagraphStart-com.aspose.note.InkParagraph-) | Starten Sie den Besuch des Knotens [InkParagraph](../../com.aspose.note/inkparagraph). |
| [visitInkWordEnd(InkWord inkWord)](#visitInkWordEnd-com.aspose.note.InkWord-) | Beenden Sie den Besuch des Knotens [InkWord](../../com.aspose.note/inkword). |
| [visitInkWordStart(InkWord inkWord)](#visitInkWordStart-com.aspose.note.InkWord-) | Starten Sie den Besuch des Knotens [InkWord](../../com.aspose.note/inkword). |
| [visitLoopEnd(Loop loop)](#visitLoopEnd-com.aspose.note.Loop-) | Beenden Sie den Besuch des Knotens [Loop](../../com.aspose.note/loop). |
| [visitLoopStart(Loop loop)](#visitLoopStart-com.aspose.note.Loop-) | Starten Sie den Besuch des Knotens [Loop](../../com.aspose.note/loop). |
| [visitOutlineElementEnd(OutlineElement outlineElement)](#visitOutlineElementEnd-com.aspose.note.OutlineElement-) | Beenden Sie den Besuch des Knotens `OutlineElement`. |
| [visitOutlineElementStart(OutlineElement outlineElement)](#visitOutlineElementStart-com.aspose.note.OutlineElement-) | Starten Sie den Besuch des Knotens `OutlineElement`. |
| [visitOutlineEnd(Outline outline)](#visitOutlineEnd-com.aspose.note.Outline-) | Beenden Sie den Besuch des Knotens `Outline`. |
| [visitOutlineGroupEnd(OutlineGroup outlineGroup)](#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-) | Beenden Sie den Besuch des Knotens `OutlineGroup`. |
| [visitOutlineGroupStart(OutlineGroup outlineGroup)](#visitOutlineGroupStart-com.aspose.note.OutlineGroup-) | Starten Sie den Besuch des Knotens `OutlineGroup`. |
| [visitOutlineStart(Outline outline)](#visitOutlineStart-com.aspose.note.Outline-) | Starten Sie den Besuch des Knotens `Outline`. |
| [visitPageEnd(Page page)](#visitPageEnd-com.aspose.note.Page-) | Beenden Sie den Besuch des Knotens `Page`. |
| [visitPageStart(Page page)](#visitPageStart-com.aspose.note.Page-) | Starten Sie den Besuch des Knotens `Page`. |
| [visitRichTextEnd(RichText richText)](#visitRichTextEnd-com.aspose.note.RichText-) | Beenden Sie den Besuch des Knotens `RichText`. |
| [visitRichTextStart(RichText richText)](#visitRichTextStart-com.aspose.note.RichText-) | Starten Sie den Besuch des Knotens `RichText`. |
| [visitTableCellEnd(TableCell tableCell)](#visitTableCellEnd-com.aspose.note.TableCell-) | Beenden Sie den Besuch des Knotens `TableCell`. |
| [visitTableCellStart(TableCell tableCell)](#visitTableCellStart-com.aspose.note.TableCell-) | Starten Sie den Besuch des Knotens `TableCell`. |
| [visitTableEnd(Table table)](#visitTableEnd-com.aspose.note.Table-) | Ende beim Besuch des `Table` Knotens. |
| [visitTableRowEnd(TableRow tableRow)](#visitTableRowEnd-com.aspose.note.TableRow-) | Ende beim Besuch des `TableRow` Knotens. |
| [visitTableRowStart(TableRow tableRow)](#visitTableRowStart-com.aspose.note.TableRow-) | Start beim Besuch des `TableRow` Knotens. |
| [visitTableStart(Table table)](#visitTableStart-com.aspose.note.Table-) | Start beim Besuch des `Table` Knotens. |
| [visitTitleEnd(Title title)](#visitTitleEnd-com.aspose.note.Title-) | Ende beim Besuch des `Title` Knotens. |
| [visitTitleStart(Title title)](#visitTitleStart-com.aspose.note.Title-) | Start beim Besuch des `Title` Knotens. |
### DocumentVisitor() {#DocumentVisitor--}
```
public DocumentVisitor()
```


### visitAttachedFileEnd(AttachedFile attachedFile) {#visitAttachedFileEnd-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileEnd(AttachedFile attachedFile)
```


Ende, um den `AttachedFile`-Knoten zu besuchen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | Der `AttachedFile` Knoten. |

### visitAttachedFileStart(AttachedFile attachedFile) {#visitAttachedFileStart-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileStart(AttachedFile attachedFile)
```


Starten Sie den Besuch des Knotens `AttachedFile`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | Der `AttachedFile` Knoten. |

### visitDocumentEnd(Document document) {#visitDocumentEnd-com.aspose.note.Document-}
```
public void visitDocumentEnd(Document document)
```


Beenden Sie den Besuch des Knotens `Document`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | Der `Document` Knoten. |

### visitDocumentStart(Document document) {#visitDocumentStart-com.aspose.note.Document-}
```
public void visitDocumentStart(Document document)
```


Starten Sie den Besuch des Knotens `Document`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | Der `Document` Knoten. |

### visitImageEnd(Image image) {#visitImageEnd-com.aspose.note.Image-}
```
public void visitImageEnd(Image image)
```


Beenden Sie den Besuch des Knotens `Image`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | Der `Image` Knoten. |

### visitImageStart(Image image) {#visitImageStart-com.aspose.note.Image-}
```
public void visitImageStart(Image image)
```


Starten Sie den Besuch des Knotens `Image`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | Der `Image` Knoten. |

### visitInkDrawingEnd(InkDrawing inkDrawing) {#visitInkDrawingEnd-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingEnd(InkDrawing inkDrawing)
```


Beenden Sie den Besuch des Knotens [InkDrawing](../../com.aspose.note/inkdrawing).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | Der [InkDrawing](../../com.aspose.note/inkdrawing) Knoten. |

### visitInkDrawingStart(InkDrawing inkDrawing) {#visitInkDrawingStart-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingStart(InkDrawing inkDrawing)
```


Starten Sie den Besuch des Knotens [InkDrawing](../../com.aspose.note/inkdrawing).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | Der [InkDrawing](../../com.aspose.note/inkdrawing) Knoten. |

### visitInkParagraphEnd(InkParagraph inkParagraph) {#visitInkParagraphEnd-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphEnd(InkParagraph inkParagraph)
```


Beenden Sie den Besuch des Knotens [InkParagraph](../../com.aspose.note/inkparagraph).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | Der [InkParagraph](../../com.aspose.note/inkparagraph) Knoten. |

### visitInkParagraphStart(InkParagraph inkParagraph) {#visitInkParagraphStart-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphStart(InkParagraph inkParagraph)
```


Starten Sie den Besuch des Knotens [InkParagraph](../../com.aspose.note/inkparagraph).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | Der [InkParagraph](../../com.aspose.note/inkparagraph) Knoten. |

### visitInkWordEnd(InkWord inkWord) {#visitInkWordEnd-com.aspose.note.InkWord-}
```
public void visitInkWordEnd(InkWord inkWord)
```


Beenden Sie den Besuch des Knotens [InkWord](../../com.aspose.note/inkword).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | Der [InkWord](../../com.aspose.note/inkword) Knoten. |

### visitInkWordStart(InkWord inkWord) {#visitInkWordStart-com.aspose.note.InkWord-}
```
public void visitInkWordStart(InkWord inkWord)
```


Starten Sie den Besuch des Knotens [InkWord](../../com.aspose.note/inkword).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | Der [InkWord](../../com.aspose.note/inkword) Knoten. |

### visitLoopEnd(Loop loop) {#visitLoopEnd-com.aspose.note.Loop-}
```
public void visitLoopEnd(Loop loop)
```


Beenden Sie den Besuch des Knotens [Loop](../../com.aspose.note/loop).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | Der [Loop](../../com.aspose.note/loop) Knoten. |

### visitLoopStart(Loop loop) {#visitLoopStart-com.aspose.note.Loop-}
```
public void visitLoopStart(Loop loop)
```


Starten Sie den Besuch des Knotens [Loop](../../com.aspose.note/loop).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | Der [Loop](../../com.aspose.note/loop) Knoten. |

### visitOutlineElementEnd(OutlineElement outlineElement) {#visitOutlineElementEnd-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementEnd(OutlineElement outlineElement)
```


Beenden Sie den Besuch des Knotens `OutlineElement`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | Der `OutlineElement` Knoten. |

### visitOutlineElementStart(OutlineElement outlineElement) {#visitOutlineElementStart-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementStart(OutlineElement outlineElement)
```


Starten Sie den Besuch des Knotens `OutlineElement`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | Der `OutlineElement` Knoten. |

### visitOutlineEnd(Outline outline) {#visitOutlineEnd-com.aspose.note.Outline-}
```
public void visitOutlineEnd(Outline outline)
```


Beenden Sie den Besuch des Knotens `Outline`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | Der `Outline` Knoten. |

### visitOutlineGroupEnd(OutlineGroup outlineGroup) {#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupEnd(OutlineGroup outlineGroup)
```


Beenden Sie den Besuch des Knotens `OutlineGroup`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | Der `OutlineGroup` Knoten. |

### visitOutlineGroupStart(OutlineGroup outlineGroup) {#visitOutlineGroupStart-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupStart(OutlineGroup outlineGroup)
```


Starten Sie den Besuch des Knotens `OutlineGroup`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | Der `OutlineGroup` Knoten. |

### visitOutlineStart(Outline outline) {#visitOutlineStart-com.aspose.note.Outline-}
```
public void visitOutlineStart(Outline outline)
```


Starten Sie den Besuch des Knotens `Outline`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | Der `Outline` Knoten. |

### visitPageEnd(Page page) {#visitPageEnd-com.aspose.note.Page-}
```
public void visitPageEnd(Page page)
```


Beenden Sie den Besuch des Knotens `Page`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Der `Page` Knoten. |

### visitPageStart(Page page) {#visitPageStart-com.aspose.note.Page-}
```
public void visitPageStart(Page page)
```


Starten Sie den Besuch des Knotens `Page`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Der `Page` Knoten. |

### visitRichTextEnd(RichText richText) {#visitRichTextEnd-com.aspose.note.RichText-}
```
public void visitRichTextEnd(RichText richText)
```


Beenden Sie den Besuch des Knotens `RichText`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | Der `RichText` Knoten. |

### visitRichTextStart(RichText richText) {#visitRichTextStart-com.aspose.note.RichText-}
```
public void visitRichTextStart(RichText richText)
```


Starten Sie den Besuch des Knotens `RichText`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | Der `RichText` Knoten. |

### visitTableCellEnd(TableCell tableCell) {#visitTableCellEnd-com.aspose.note.TableCell-}
```
public void visitTableCellEnd(TableCell tableCell)
```


Beenden Sie den Besuch des Knotens `TableCell`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | Der `TableCell` Knoten. |

### visitTableCellStart(TableCell tableCell) {#visitTableCellStart-com.aspose.note.TableCell-}
```
public void visitTableCellStart(TableCell tableCell)
```


Starten Sie den Besuch des Knotens `TableCell`.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | Der `TableCell` Knoten. |

### visitTableEnd(Table table) {#visitTableEnd-com.aspose.note.Table-}
```
public void visitTableEnd(Table table)
```


Ende beim Besuch des `Table` Knotens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | Der `Table` Knoten. |

### visitTableRowEnd(TableRow tableRow) {#visitTableRowEnd-com.aspose.note.TableRow-}
```
public void visitTableRowEnd(TableRow tableRow)
```


Ende beim Besuch des `TableRow` Knotens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | Der `TableRow` Knoten. |

### visitTableRowStart(TableRow tableRow) {#visitTableRowStart-com.aspose.note.TableRow-}
```
public void visitTableRowStart(TableRow tableRow)
```


Start beim Besuch des `TableRow` Knotens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | Der `TableRow` Knoten. |

### visitTableStart(Table table) {#visitTableStart-com.aspose.note.Table-}
```
public void visitTableStart(Table table)
```


Start beim Besuch des `Table` Knotens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | Der `Table` Knoten. |

### visitTitleEnd(Title title) {#visitTitleEnd-com.aspose.note.Title-}
```
public void visitTitleEnd(Title title)
```


Ende beim Besuch des `Title` Knotens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | Der `Title` Knoten. |

### visitTitleStart(Title title) {#visitTitleStart-com.aspose.note.Title-}
```
public void visitTitleStart(Title title)
```


Start beim Besuch des `Title` Knotens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | Der `Title` Knoten. |

