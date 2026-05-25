---
title: "DocumentVisitor"
second_title: "Riferimento API di Aspose.Note per Java"
description: "La classe astratta per iterare attraverso il sottoalbero con radice nel nodo specificato."
type: docs
weight: 22
url: /it/java/com.aspose.note/documentvisitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class DocumentVisitor
```

La classe astratta per iterare attraverso il sottoalbero con radice nel nodo specificato.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [DocumentVisitor()](#DocumentVisitor--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [visitAttachedFileEnd(AttachedFile attachedFile)](#visitAttachedFileEnd-com.aspose.note.AttachedFile-) | Fine per visitare il nodo `AttachedFile`. |
| [visitAttachedFileStart(AttachedFile attachedFile)](#visitAttachedFileStart-com.aspose.note.AttachedFile-) | Inizio a visitare il nodo `AttachedFile`. |
| [visitDocumentEnd(Document document)](#visitDocumentEnd-com.aspose.note.Document-) | Fine a visitare il nodo `Document`. |
| [visitDocumentStart(Document document)](#visitDocumentStart-com.aspose.note.Document-) | Inizio a visitare il nodo `Document`. |
| [visitImageEnd(Image image)](#visitImageEnd-com.aspose.note.Image-) | Fine a visitare il nodo `Image`. |
| [visitImageStart(Image image)](#visitImageStart-com.aspose.note.Image-) | Inizio a visitare il nodo `Image`. |
| [visitInkDrawingEnd(InkDrawing inkDrawing)](#visitInkDrawingEnd-com.aspose.note.InkDrawing-) | Fine a visitare il nodo [InkDrawing](../../com.aspose.note/inkdrawing). |
| [visitInkDrawingStart(InkDrawing inkDrawing)](#visitInkDrawingStart-com.aspose.note.InkDrawing-) | Inizio a visitare il nodo [InkDrawing](../../com.aspose.note/inkdrawing). |
| [visitInkParagraphEnd(InkParagraph inkParagraph)](#visitInkParagraphEnd-com.aspose.note.InkParagraph-) | Fine a visitare il nodo [InkParagraph](../../com.aspose.note/inkparagraph). |
| [visitInkParagraphStart(InkParagraph inkParagraph)](#visitInkParagraphStart-com.aspose.note.InkParagraph-) | Inizio a visitare il nodo [InkParagraph](../../com.aspose.note/inkparagraph). |
| [visitInkWordEnd(InkWord inkWord)](#visitInkWordEnd-com.aspose.note.InkWord-) | Fine a visitare il nodo [InkWord](../../com.aspose.note/inkword). |
| [visitInkWordStart(InkWord inkWord)](#visitInkWordStart-com.aspose.note.InkWord-) | Inizio a visitare il nodo [InkWord](../../com.aspose.note/inkword). |
| [visitLoopEnd(Loop loop)](#visitLoopEnd-com.aspose.note.Loop-) | Fine a visitare il nodo [Loop](../../com.aspose.note/loop). |
| [visitLoopStart(Loop loop)](#visitLoopStart-com.aspose.note.Loop-) | Inizio a visitare il nodo [Loop](../../com.aspose.note/loop). |
| [visitOutlineElementEnd(OutlineElement outlineElement)](#visitOutlineElementEnd-com.aspose.note.OutlineElement-) | Fine a visitare il nodo `OutlineElement`. |
| [visitOutlineElementStart(OutlineElement outlineElement)](#visitOutlineElementStart-com.aspose.note.OutlineElement-) | Inizio a visitare il nodo `OutlineElement`. |
| [visitOutlineEnd(Outline outline)](#visitOutlineEnd-com.aspose.note.Outline-) | Fine a visitare il nodo `Outline`. |
| [visitOutlineGroupEnd(OutlineGroup outlineGroup)](#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-) | Fine a visitare il nodo `OutlineGroup`. |
| [visitOutlineGroupStart(OutlineGroup outlineGroup)](#visitOutlineGroupStart-com.aspose.note.OutlineGroup-) | Inizio a visitare il nodo `OutlineGroup`. |
| [visitOutlineStart(Outline outline)](#visitOutlineStart-com.aspose.note.Outline-) | Inizio a visitare il nodo `Outline`. |
| [visitPageEnd(Page page)](#visitPageEnd-com.aspose.note.Page-) | Fine a visitare il nodo `Page`. |
| [visitPageStart(Page page)](#visitPageStart-com.aspose.note.Page-) | Inizio a visitare il nodo `Page`. |
| [visitRichTextEnd(RichText richText)](#visitRichTextEnd-com.aspose.note.RichText-) | Fine a visitare il nodo `RichText`. |
| [visitRichTextStart(RichText richText)](#visitRichTextStart-com.aspose.note.RichText-) | Inizio a visitare il nodo `RichText`. |
| [visitTableCellEnd(TableCell tableCell)](#visitTableCellEnd-com.aspose.note.TableCell-) | Fine a visitare il nodo `TableCell`. |
| [visitTableCellStart(TableCell tableCell)](#visitTableCellStart-com.aspose.note.TableCell-) | Inizio a visitare il nodo `TableCell`. |
| [visitTableEnd(Table table)](#visitTableEnd-com.aspose.note.Table-) | Fine per visitare il nodo `Table`. |
| [visitTableRowEnd(TableRow tableRow)](#visitTableRowEnd-com.aspose.note.TableRow-) | Fine per visitare il nodo `TableRow`. |
| [visitTableRowStart(TableRow tableRow)](#visitTableRowStart-com.aspose.note.TableRow-) | Inizio per visitare il nodo `TableRow`. |
| [visitTableStart(Table table)](#visitTableStart-com.aspose.note.Table-) | Inizio per visitare il nodo `Table`. |
| [visitTitleEnd(Title title)](#visitTitleEnd-com.aspose.note.Title-) | Fine per visitare il nodo `Title`. |
| [visitTitleStart(Title title)](#visitTitleStart-com.aspose.note.Title-) | Inizio per visitare il nodo `Title`. |
### DocumentVisitor() {#DocumentVisitor--}
```
public DocumentVisitor()
```


### visitAttachedFileEnd(AttachedFile attachedFile) {#visitAttachedFileEnd-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileEnd(AttachedFile attachedFile)
```


Fine per visitare il nodo `AttachedFile`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | Il nodo `AttachedFile`. |

### visitAttachedFileStart(AttachedFile attachedFile) {#visitAttachedFileStart-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileStart(AttachedFile attachedFile)
```


Inizio a visitare il nodo `AttachedFile`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | Il nodo `AttachedFile`. |

### visitDocumentEnd(Document document) {#visitDocumentEnd-com.aspose.note.Document-}
```
public void visitDocumentEnd(Document document)
```


Fine a visitare il nodo `Document`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | Il nodo `Document`. |

### visitDocumentStart(Document document) {#visitDocumentStart-com.aspose.note.Document-}
```
public void visitDocumentStart(Document document)
```


Inizio a visitare il nodo `Document`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | Il nodo `Document`. |

### visitImageEnd(Image image) {#visitImageEnd-com.aspose.note.Image-}
```
public void visitImageEnd(Image image)
```


Fine a visitare il nodo `Image`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | Il nodo `Image`. |

### visitImageStart(Image image) {#visitImageStart-com.aspose.note.Image-}
```
public void visitImageStart(Image image)
```


Inizio a visitare il nodo `Image`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | Il nodo `Image`. |

### visitInkDrawingEnd(InkDrawing inkDrawing) {#visitInkDrawingEnd-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingEnd(InkDrawing inkDrawing)
```


Fine a visitare il nodo [InkDrawing](../../com.aspose.note/inkdrawing).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | Il nodo [InkDrawing](../../com.aspose.note/inkdrawing). |

### visitInkDrawingStart(InkDrawing inkDrawing) {#visitInkDrawingStart-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingStart(InkDrawing inkDrawing)
```


Inizio a visitare il nodo [InkDrawing](../../com.aspose.note/inkdrawing).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | Il nodo [InkDrawing](../../com.aspose.note/inkdrawing). |

### visitInkParagraphEnd(InkParagraph inkParagraph) {#visitInkParagraphEnd-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphEnd(InkParagraph inkParagraph)
```


Fine a visitare il nodo [InkParagraph](../../com.aspose.note/inkparagraph).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | Il nodo [InkParagraph](../../com.aspose.note/inkparagraph). |

### visitInkParagraphStart(InkParagraph inkParagraph) {#visitInkParagraphStart-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphStart(InkParagraph inkParagraph)
```


Inizio a visitare il nodo [InkParagraph](../../com.aspose.note/inkparagraph).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | Il nodo [InkParagraph](../../com.aspose.note/inkparagraph). |

### visitInkWordEnd(InkWord inkWord) {#visitInkWordEnd-com.aspose.note.InkWord-}
```
public void visitInkWordEnd(InkWord inkWord)
```


Fine a visitare il nodo [InkWord](../../com.aspose.note/inkword).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | Il nodo [InkWord](../../com.aspose.note/inkword). |

### visitInkWordStart(InkWord inkWord) {#visitInkWordStart-com.aspose.note.InkWord-}
```
public void visitInkWordStart(InkWord inkWord)
```


Inizio a visitare il nodo [InkWord](../../com.aspose.note/inkword).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | Il nodo [InkWord](../../com.aspose.note/inkword). |

### visitLoopEnd(Loop loop) {#visitLoopEnd-com.aspose.note.Loop-}
```
public void visitLoopEnd(Loop loop)
```


Fine a visitare il nodo [Loop](../../com.aspose.note/loop).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | Il nodo [Loop](../../com.aspose.note/loop). |

### visitLoopStart(Loop loop) {#visitLoopStart-com.aspose.note.Loop-}
```
public void visitLoopStart(Loop loop)
```


Inizio a visitare il nodo [Loop](../../com.aspose.note/loop).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | Il nodo [Loop](../../com.aspose.note/loop). |

### visitOutlineElementEnd(OutlineElement outlineElement) {#visitOutlineElementEnd-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementEnd(OutlineElement outlineElement)
```


Fine a visitare il nodo `OutlineElement`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | Il nodo `OutlineElement`. |

### visitOutlineElementStart(OutlineElement outlineElement) {#visitOutlineElementStart-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementStart(OutlineElement outlineElement)
```


Inizio a visitare il nodo `OutlineElement`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | Il nodo `OutlineElement`. |

### visitOutlineEnd(Outline outline) {#visitOutlineEnd-com.aspose.note.Outline-}
```
public void visitOutlineEnd(Outline outline)
```


Fine a visitare il nodo `Outline`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | Il nodo `Outline`. |

### visitOutlineGroupEnd(OutlineGroup outlineGroup) {#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupEnd(OutlineGroup outlineGroup)
```


Fine a visitare il nodo `OutlineGroup`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | Il nodo `OutlineGroup`. |

### visitOutlineGroupStart(OutlineGroup outlineGroup) {#visitOutlineGroupStart-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupStart(OutlineGroup outlineGroup)
```


Inizio a visitare il nodo `OutlineGroup`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | Il nodo `OutlineGroup`. |

### visitOutlineStart(Outline outline) {#visitOutlineStart-com.aspose.note.Outline-}
```
public void visitOutlineStart(Outline outline)
```


Inizio a visitare il nodo `Outline`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | Il nodo `Outline`. |

### visitPageEnd(Page page) {#visitPageEnd-com.aspose.note.Page-}
```
public void visitPageEnd(Page page)
```


Fine a visitare il nodo `Page`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Il nodo `Page`. |

### visitPageStart(Page page) {#visitPageStart-com.aspose.note.Page-}
```
public void visitPageStart(Page page)
```


Inizio a visitare il nodo `Page`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Il nodo `Page`. |

### visitRichTextEnd(RichText richText) {#visitRichTextEnd-com.aspose.note.RichText-}
```
public void visitRichTextEnd(RichText richText)
```


Fine a visitare il nodo `RichText`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | Il nodo `RichText`. |

### visitRichTextStart(RichText richText) {#visitRichTextStart-com.aspose.note.RichText-}
```
public void visitRichTextStart(RichText richText)
```


Inizio a visitare il nodo `RichText`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | Il nodo `RichText`. |

### visitTableCellEnd(TableCell tableCell) {#visitTableCellEnd-com.aspose.note.TableCell-}
```
public void visitTableCellEnd(TableCell tableCell)
```


Fine a visitare il nodo `TableCell`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | Il nodo `TableCell`. |

### visitTableCellStart(TableCell tableCell) {#visitTableCellStart-com.aspose.note.TableCell-}
```
public void visitTableCellStart(TableCell tableCell)
```


Inizio a visitare il nodo `TableCell`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | Il nodo `TableCell`. |

### visitTableEnd(Table table) {#visitTableEnd-com.aspose.note.Table-}
```
public void visitTableEnd(Table table)
```


Fine per visitare il nodo `Table`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | Il nodo `Table`. |

### visitTableRowEnd(TableRow tableRow) {#visitTableRowEnd-com.aspose.note.TableRow-}
```
public void visitTableRowEnd(TableRow tableRow)
```


Fine per visitare il nodo `TableRow`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | Il nodo `TableRow`. |

### visitTableRowStart(TableRow tableRow) {#visitTableRowStart-com.aspose.note.TableRow-}
```
public void visitTableRowStart(TableRow tableRow)
```


Inizio per visitare il nodo `TableRow`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | Il nodo `TableRow`. |

### visitTableStart(Table table) {#visitTableStart-com.aspose.note.Table-}
```
public void visitTableStart(Table table)
```


Inizio per visitare il nodo `Table`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | Il nodo `Table`. |

### visitTitleEnd(Title title) {#visitTitleEnd-com.aspose.note.Title-}
```
public void visitTitleEnd(Title title)
```


Fine per visitare il nodo `Title`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | Il nodo `Title`. |

### visitTitleStart(Title title) {#visitTitleStart-com.aspose.note.Title-}
```
public void visitTitleStart(Title title)
```


Inizio per visitare il nodo `Title`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | Il nodo `Title`. |

