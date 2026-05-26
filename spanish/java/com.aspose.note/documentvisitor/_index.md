---
title: "DocumentVisitor"
second_title: "Referencia de API de Aspose.Note para Java"
description: "La clase abstracta para iterar a través del subárbol con raíz en el nodo especificado."
type: docs
weight: 22
url: /es/java/com.aspose.note/documentvisitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class DocumentVisitor
```

La clase abstracta para iterar a través del subárbol con raíz en el nodo especificado.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [DocumentVisitor()](#DocumentVisitor--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [visitAttachedFileEnd(AttachedFile attachedFile)](#visitAttachedFileEnd-com.aspose.note.AttachedFile-) | Fin para visitar el nodo `AttachedFile`. |
| [visitAttachedFileStart(AttachedFile attachedFile)](#visitAttachedFileStart-com.aspose.note.AttachedFile-) | Iniciar la visita al nodo `AttachedFile`. |
| [visitDocumentEnd(Document document)](#visitDocumentEnd-com.aspose.note.Document-) | Finalizar la visita al nodo `Document`. |
| [visitDocumentStart(Document document)](#visitDocumentStart-com.aspose.note.Document-) | Iniciar la visita al nodo `Document`. |
| [visitImageEnd(Image image)](#visitImageEnd-com.aspose.note.Image-) | Finalizar la visita al nodo `Image`. |
| [visitImageStart(Image image)](#visitImageStart-com.aspose.note.Image-) | Iniciar la visita al nodo `Image`. |
| [visitInkDrawingEnd(InkDrawing inkDrawing)](#visitInkDrawingEnd-com.aspose.note.InkDrawing-) | Finalizar la visita al nodo [InkDrawing](../../com.aspose.note/inkdrawing). |
| [visitInkDrawingStart(InkDrawing inkDrawing)](#visitInkDrawingStart-com.aspose.note.InkDrawing-) | Iniciar la visita al nodo [InkDrawing](../../com.aspose.note/inkdrawing). |
| [visitInkParagraphEnd(InkParagraph inkParagraph)](#visitInkParagraphEnd-com.aspose.note.InkParagraph-) | Finalizar la visita al nodo [InkParagraph](../../com.aspose.note/inkparagraph). |
| [visitInkParagraphStart(InkParagraph inkParagraph)](#visitInkParagraphStart-com.aspose.note.InkParagraph-) | Iniciar la visita al nodo [InkParagraph](../../com.aspose.note/inkparagraph). |
| [visitInkWordEnd(InkWord inkWord)](#visitInkWordEnd-com.aspose.note.InkWord-) | Finalizar la visita al nodo [InkWord](../../com.aspose.note/inkword). |
| [visitInkWordStart(InkWord inkWord)](#visitInkWordStart-com.aspose.note.InkWord-) | Iniciar la visita al nodo [InkWord](../../com.aspose.note/inkword). |
| [visitLoopEnd(Loop loop)](#visitLoopEnd-com.aspose.note.Loop-) | Finalizar la visita al nodo [Loop](../../com.aspose.note/loop). |
| [visitLoopStart(Loop loop)](#visitLoopStart-com.aspose.note.Loop-) | Iniciar la visita al nodo [Loop](../../com.aspose.note/loop). |
| [visitOutlineElementEnd(OutlineElement outlineElement)](#visitOutlineElementEnd-com.aspose.note.OutlineElement-) | Finalizar la visita al nodo `OutlineElement`. |
| [visitOutlineElementStart(OutlineElement outlineElement)](#visitOutlineElementStart-com.aspose.note.OutlineElement-) | Iniciar la visita al nodo `OutlineElement`. |
| [visitOutlineEnd(Outline outline)](#visitOutlineEnd-com.aspose.note.Outline-) | Finalizar la visita al nodo `Outline`. |
| [visitOutlineGroupEnd(OutlineGroup outlineGroup)](#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-) | Finalizar la visita al nodo `OutlineGroup`. |
| [visitOutlineGroupStart(OutlineGroup outlineGroup)](#visitOutlineGroupStart-com.aspose.note.OutlineGroup-) | Iniciar la visita al nodo `OutlineGroup`. |
| [visitOutlineStart(Outline outline)](#visitOutlineStart-com.aspose.note.Outline-) | Iniciar la visita al nodo `Outline`. |
| [visitPageEnd(Page page)](#visitPageEnd-com.aspose.note.Page-) | Finalizar la visita al nodo `Page`. |
| [visitPageStart(Page page)](#visitPageStart-com.aspose.note.Page-) | Iniciar la visita al nodo `Page`. |
| [visitRichTextEnd(RichText richText)](#visitRichTextEnd-com.aspose.note.RichText-) | Finalizar la visita al nodo `RichText`. |
| [visitRichTextStart(RichText richText)](#visitRichTextStart-com.aspose.note.RichText-) | Iniciar la visita al nodo `RichText`. |
| [visitTableCellEnd(TableCell tableCell)](#visitTableCellEnd-com.aspose.note.TableCell-) | Finalizar la visita al nodo `TableCell`. |
| [visitTableCellStart(TableCell tableCell)](#visitTableCellStart-com.aspose.note.TableCell-) | Iniciar la visita al nodo `TableCell`. |
| [visitTableEnd(Table table)](#visitTableEnd-com.aspose.note.Table-) | Fin de visitar el nodo `Table`. |
| [visitTableRowEnd(TableRow tableRow)](#visitTableRowEnd-com.aspose.note.TableRow-) | Fin de visitar el nodo `TableRow`. |
| [visitTableRowStart(TableRow tableRow)](#visitTableRowStart-com.aspose.note.TableRow-) | Inicio de visitar el nodo `TableRow`. |
| [visitTableStart(Table table)](#visitTableStart-com.aspose.note.Table-) | Inicio de visitar el nodo `Table`. |
| [visitTitleEnd(Title title)](#visitTitleEnd-com.aspose.note.Title-) | Fin de visitar el nodo `Title`. |
| [visitTitleStart(Title title)](#visitTitleStart-com.aspose.note.Title-) | Inicio de visitar el nodo `Title`. |
### DocumentVisitor() {#DocumentVisitor--}
```
public DocumentVisitor()
```


### visitAttachedFileEnd(AttachedFile attachedFile) {#visitAttachedFileEnd-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileEnd(AttachedFile attachedFile)
```


Fin para visitar el nodo `AttachedFile`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | El nodo `AttachedFile`. |

### visitAttachedFileStart(AttachedFile attachedFile) {#visitAttachedFileStart-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileStart(AttachedFile attachedFile)
```


Iniciar la visita al nodo `AttachedFile`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | El nodo `AttachedFile`. |

### visitDocumentEnd(Document document) {#visitDocumentEnd-com.aspose.note.Document-}
```
public void visitDocumentEnd(Document document)
```


Finalizar la visita al nodo `Document`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | El nodo `Document`. |

### visitDocumentStart(Document document) {#visitDocumentStart-com.aspose.note.Document-}
```
public void visitDocumentStart(Document document)
```


Iniciar la visita al nodo `Document`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | El nodo `Document`. |

### visitImageEnd(Image image) {#visitImageEnd-com.aspose.note.Image-}
```
public void visitImageEnd(Image image)
```


Finalizar la visita al nodo `Image`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | El nodo `Image`. |

### visitImageStart(Image image) {#visitImageStart-com.aspose.note.Image-}
```
public void visitImageStart(Image image)
```


Iniciar la visita al nodo `Image`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | El nodo `Image`. |

### visitInkDrawingEnd(InkDrawing inkDrawing) {#visitInkDrawingEnd-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingEnd(InkDrawing inkDrawing)
```


Finalizar la visita al nodo [InkDrawing](../../com.aspose.note/inkdrawing).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | El nodo [InkDrawing](../../com.aspose.note/inkdrawing). |

### visitInkDrawingStart(InkDrawing inkDrawing) {#visitInkDrawingStart-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingStart(InkDrawing inkDrawing)
```


Iniciar la visita al nodo [InkDrawing](../../com.aspose.note/inkdrawing).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | El nodo [InkDrawing](../../com.aspose.note/inkdrawing). |

### visitInkParagraphEnd(InkParagraph inkParagraph) {#visitInkParagraphEnd-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphEnd(InkParagraph inkParagraph)
```


Finalizar la visita al nodo [InkParagraph](../../com.aspose.note/inkparagraph).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | El nodo [InkParagraph](../../com.aspose.note/inkparagraph). |

### visitInkParagraphStart(InkParagraph inkParagraph) {#visitInkParagraphStart-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphStart(InkParagraph inkParagraph)
```


Iniciar la visita al nodo [InkParagraph](../../com.aspose.note/inkparagraph).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | El nodo [InkParagraph](../../com.aspose.note/inkparagraph). |

### visitInkWordEnd(InkWord inkWord) {#visitInkWordEnd-com.aspose.note.InkWord-}
```
public void visitInkWordEnd(InkWord inkWord)
```


Finalizar la visita al nodo [InkWord](../../com.aspose.note/inkword).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | El nodo [InkWord](../../com.aspose.note/inkword). |

### visitInkWordStart(InkWord inkWord) {#visitInkWordStart-com.aspose.note.InkWord-}
```
public void visitInkWordStart(InkWord inkWord)
```


Iniciar la visita al nodo [InkWord](../../com.aspose.note/inkword).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | El nodo [InkWord](../../com.aspose.note/inkword). |

### visitLoopEnd(Loop loop) {#visitLoopEnd-com.aspose.note.Loop-}
```
public void visitLoopEnd(Loop loop)
```


Finalizar la visita al nodo [Loop](../../com.aspose.note/loop).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | El nodo [Loop](../../com.aspose.note/loop). |

### visitLoopStart(Loop loop) {#visitLoopStart-com.aspose.note.Loop-}
```
public void visitLoopStart(Loop loop)
```


Iniciar la visita al nodo [Loop](../../com.aspose.note/loop).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | El nodo [Loop](../../com.aspose.note/loop). |

### visitOutlineElementEnd(OutlineElement outlineElement) {#visitOutlineElementEnd-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementEnd(OutlineElement outlineElement)
```


Finalizar la visita al nodo `OutlineElement`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | El nodo `OutlineElement`. |

### visitOutlineElementStart(OutlineElement outlineElement) {#visitOutlineElementStart-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementStart(OutlineElement outlineElement)
```


Iniciar la visita al nodo `OutlineElement`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | El nodo `OutlineElement`. |

### visitOutlineEnd(Outline outline) {#visitOutlineEnd-com.aspose.note.Outline-}
```
public void visitOutlineEnd(Outline outline)
```


Finalizar la visita al nodo `Outline`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | El nodo `Outline`. |

### visitOutlineGroupEnd(OutlineGroup outlineGroup) {#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupEnd(OutlineGroup outlineGroup)
```


Finalizar la visita al nodo `OutlineGroup`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | El nodo `OutlineGroup`. |

### visitOutlineGroupStart(OutlineGroup outlineGroup) {#visitOutlineGroupStart-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupStart(OutlineGroup outlineGroup)
```


Iniciar la visita al nodo `OutlineGroup`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | El nodo `OutlineGroup`. |

### visitOutlineStart(Outline outline) {#visitOutlineStart-com.aspose.note.Outline-}
```
public void visitOutlineStart(Outline outline)
```


Iniciar la visita al nodo `Outline`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | El nodo `Outline`. |

### visitPageEnd(Page page) {#visitPageEnd-com.aspose.note.Page-}
```
public void visitPageEnd(Page page)
```


Finalizar la visita al nodo `Page`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | El nodo `Page`. |

### visitPageStart(Page page) {#visitPageStart-com.aspose.note.Page-}
```
public void visitPageStart(Page page)
```


Iniciar la visita al nodo `Page`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | El nodo `Page`. |

### visitRichTextEnd(RichText richText) {#visitRichTextEnd-com.aspose.note.RichText-}
```
public void visitRichTextEnd(RichText richText)
```


Finalizar la visita al nodo `RichText`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | El nodo `RichText`. |

### visitRichTextStart(RichText richText) {#visitRichTextStart-com.aspose.note.RichText-}
```
public void visitRichTextStart(RichText richText)
```


Iniciar la visita al nodo `RichText`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | El nodo `RichText`. |

### visitTableCellEnd(TableCell tableCell) {#visitTableCellEnd-com.aspose.note.TableCell-}
```
public void visitTableCellEnd(TableCell tableCell)
```


Finalizar la visita al nodo `TableCell`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | El nodo `TableCell`. |

### visitTableCellStart(TableCell tableCell) {#visitTableCellStart-com.aspose.note.TableCell-}
```
public void visitTableCellStart(TableCell tableCell)
```


Iniciar la visita al nodo `TableCell`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | El nodo `TableCell`. |

### visitTableEnd(Table table) {#visitTableEnd-com.aspose.note.Table-}
```
public void visitTableEnd(Table table)
```


Fin de visitar el nodo `Table`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | El nodo `Table`. |

### visitTableRowEnd(TableRow tableRow) {#visitTableRowEnd-com.aspose.note.TableRow-}
```
public void visitTableRowEnd(TableRow tableRow)
```


Fin de visitar el nodo `TableRow`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | El nodo `TableRow`. |

### visitTableRowStart(TableRow tableRow) {#visitTableRowStart-com.aspose.note.TableRow-}
```
public void visitTableRowStart(TableRow tableRow)
```


Inicio de visitar el nodo `TableRow`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | El nodo `TableRow`. |

### visitTableStart(Table table) {#visitTableStart-com.aspose.note.Table-}
```
public void visitTableStart(Table table)
```


Inicio de visitar el nodo `Table`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | El nodo `Table`. |

### visitTitleEnd(Title title) {#visitTitleEnd-com.aspose.note.Title-}
```
public void visitTitleEnd(Title title)
```


Fin de visitar el nodo `Title`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | El nodo `Title`. |

### visitTitleStart(Title title) {#visitTitleStart-com.aspose.note.Title-}
```
public void visitTitleStart(Title title)
```


Inicio de visitar el nodo `Title`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | El nodo `Title`. |

