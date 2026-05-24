---
title: "DocumentVisitor"
second_title: "Référence d'API Aspose.Note pour Java"
description: "La classe abstraite pour parcourir le sous-arbre dont la racine est le nœud spécifié."
type: docs
weight: 22
url: /fr/java/com.aspose.note/documentvisitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class DocumentVisitor
```

La classe abstraite pour parcourir le sous-arbre dont la racine est le nœud spécifié.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [DocumentVisitor()](#DocumentVisitor--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [visitAttachedFileEnd(AttachedFile attachedFile)](#visitAttachedFileEnd-com.aspose.note.AttachedFile-) | Fin de la visite du nœud `AttachedFile`. |
| [visitAttachedFileStart(AttachedFile attachedFile)](#visitAttachedFileStart-com.aspose.note.AttachedFile-) | Début de la visite du nœud `AttachedFile`. |
| [visitDocumentEnd(Document document)](#visitDocumentEnd-com.aspose.note.Document-) | Fin de la visite du nœud `Document`. |
| [visitDocumentStart(Document document)](#visitDocumentStart-com.aspose.note.Document-) | Début de la visite du nœud `Document`. |
| [visitImageEnd(Image image)](#visitImageEnd-com.aspose.note.Image-) | Fin de la visite du nœud `Image`. |
| [visitImageStart(Image image)](#visitImageStart-com.aspose.note.Image-) | Début de la visite du nœud `Image`. |
| [visitInkDrawingEnd(InkDrawing inkDrawing)](#visitInkDrawingEnd-com.aspose.note.InkDrawing-) | Fin de la visite du nœud [InkDrawing](../../com.aspose.note/inkdrawing). |
| [visitInkDrawingStart(InkDrawing inkDrawing)](#visitInkDrawingStart-com.aspose.note.InkDrawing-) | Début de la visite du nœud [InkDrawing](../../com.aspose.note/inkdrawing). |
| [visitInkParagraphEnd(InkParagraph inkParagraph)](#visitInkParagraphEnd-com.aspose.note.InkParagraph-) | Fin de la visite du nœud [InkParagraph](../../com.aspose.note/inkparagraph). |
| [visitInkParagraphStart(InkParagraph inkParagraph)](#visitInkParagraphStart-com.aspose.note.InkParagraph-) | Début de la visite du nœud [InkParagraph](../../com.aspose.note/inkparagraph). |
| [visitInkWordEnd(InkWord inkWord)](#visitInkWordEnd-com.aspose.note.InkWord-) | Fin de la visite du nœud [InkWord](../../com.aspose.note/inkword). |
| [visitInkWordStart(InkWord inkWord)](#visitInkWordStart-com.aspose.note.InkWord-) | Début de la visite du nœud [InkWord](../../com.aspose.note/inkword). |
| [visitLoopEnd(Loop loop)](#visitLoopEnd-com.aspose.note.Loop-) | Fin de la visite du nœud [Loop](../../com.aspose.note/loop). |
| [visitLoopStart(Loop loop)](#visitLoopStart-com.aspose.note.Loop-) | Début de la visite du nœud [Loop](../../com.aspose.note/loop). |
| [visitOutlineElementEnd(OutlineElement outlineElement)](#visitOutlineElementEnd-com.aspose.note.OutlineElement-) | Fin de la visite du nœud `OutlineElement`. |
| [visitOutlineElementStart(OutlineElement outlineElement)](#visitOutlineElementStart-com.aspose.note.OutlineElement-) | Début de la visite du nœud `OutlineElement`. |
| [visitOutlineEnd(Outline outline)](#visitOutlineEnd-com.aspose.note.Outline-) | Fin de la visite du nœud `Outline`. |
| [visitOutlineGroupEnd(OutlineGroup outlineGroup)](#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-) | Fin de la visite du nœud `OutlineGroup`. |
| [visitOutlineGroupStart(OutlineGroup outlineGroup)](#visitOutlineGroupStart-com.aspose.note.OutlineGroup-) | Début de la visite du nœud `OutlineGroup`. |
| [visitOutlineStart(Outline outline)](#visitOutlineStart-com.aspose.note.Outline-) | Début de la visite du nœud `Outline`. |
| [visitPageEnd(Page page)](#visitPageEnd-com.aspose.note.Page-) | Fin de la visite du nœud `Page`. |
| [visitPageStart(Page page)](#visitPageStart-com.aspose.note.Page-) | Début de la visite du nœud `Page`. |
| [visitRichTextEnd(RichText richText)](#visitRichTextEnd-com.aspose.note.RichText-) | Fin de la visite du nœud `RichText`. |
| [visitRichTextStart(RichText richText)](#visitRichTextStart-com.aspose.note.RichText-) | Début de la visite du nœud `RichText`. |
| [visitTableCellEnd(TableCell tableCell)](#visitTableCellEnd-com.aspose.note.TableCell-) | Fin de la visite du nœud `TableCell`. |
| [visitTableCellStart(TableCell tableCell)](#visitTableCellStart-com.aspose.note.TableCell-) | Début de la visite du nœud `TableCell`. |
| [visitTableEnd(Table table)](#visitTableEnd-com.aspose.note.Table-) | Fin de la visite du nœud `Table`. |
| [visitTableRowEnd(TableRow tableRow)](#visitTableRowEnd-com.aspose.note.TableRow-) | Fin de la visite du nœud `TableRow`. |
| [visitTableRowStart(TableRow tableRow)](#visitTableRowStart-com.aspose.note.TableRow-) | Début de la visite du nœud `TableRow`. |
| [visitTableStart(Table table)](#visitTableStart-com.aspose.note.Table-) | Début de la visite du nœud `Table`. |
| [visitTitleEnd(Title title)](#visitTitleEnd-com.aspose.note.Title-) | Fin de la visite du nœud `Title`. |
| [visitTitleStart(Title title)](#visitTitleStart-com.aspose.note.Title-) | Début de la visite du nœud `Title`. |
### DocumentVisitor() {#DocumentVisitor--}
```
public DocumentVisitor()
```


### visitAttachedFileEnd(AttachedFile attachedFile) {#visitAttachedFileEnd-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileEnd(AttachedFile attachedFile)
```


Fin de la visite du nœud `AttachedFile`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | Le nœud `AttachedFile`. |

### visitAttachedFileStart(AttachedFile attachedFile) {#visitAttachedFileStart-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileStart(AttachedFile attachedFile)
```


Début de la visite du nœud `AttachedFile`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | Le nœud `AttachedFile`. |

### visitDocumentEnd(Document document) {#visitDocumentEnd-com.aspose.note.Document-}
```
public void visitDocumentEnd(Document document)
```


Fin de la visite du nœud `Document`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | Le nœud `Document`. |

### visitDocumentStart(Document document) {#visitDocumentStart-com.aspose.note.Document-}
```
public void visitDocumentStart(Document document)
```


Début de la visite du nœud `Document`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | Le nœud `Document`. |

### visitImageEnd(Image image) {#visitImageEnd-com.aspose.note.Image-}
```
public void visitImageEnd(Image image)
```


Fin de la visite du nœud `Image`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | Le nœud `Image`. |

### visitImageStart(Image image) {#visitImageStart-com.aspose.note.Image-}
```
public void visitImageStart(Image image)
```


Début de la visite du nœud `Image`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | Le nœud `Image`. |

### visitInkDrawingEnd(InkDrawing inkDrawing) {#visitInkDrawingEnd-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingEnd(InkDrawing inkDrawing)
```


Fin de la visite du nœud [InkDrawing](../../com.aspose.note/inkdrawing).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | Le nœud [InkDrawing](../../com.aspose.note/inkdrawing). |

### visitInkDrawingStart(InkDrawing inkDrawing) {#visitInkDrawingStart-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingStart(InkDrawing inkDrawing)
```


Début de la visite du nœud [InkDrawing](../../com.aspose.note/inkdrawing).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | Le nœud [InkDrawing](../../com.aspose.note/inkdrawing). |

### visitInkParagraphEnd(InkParagraph inkParagraph) {#visitInkParagraphEnd-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphEnd(InkParagraph inkParagraph)
```


Fin de la visite du nœud [InkParagraph](../../com.aspose.note/inkparagraph).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | Le nœud [InkParagraph](../../com.aspose.note/inkparagraph). |

### visitInkParagraphStart(InkParagraph inkParagraph) {#visitInkParagraphStart-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphStart(InkParagraph inkParagraph)
```


Début de la visite du nœud [InkParagraph](../../com.aspose.note/inkparagraph).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | Le nœud [InkParagraph](../../com.aspose.note/inkparagraph). |

### visitInkWordEnd(InkWord inkWord) {#visitInkWordEnd-com.aspose.note.InkWord-}
```
public void visitInkWordEnd(InkWord inkWord)
```


Fin de la visite du nœud [InkWord](../../com.aspose.note/inkword).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | Le nœud [InkWord](../../com.aspose.note/inkword). |

### visitInkWordStart(InkWord inkWord) {#visitInkWordStart-com.aspose.note.InkWord-}
```
public void visitInkWordStart(InkWord inkWord)
```


Début de la visite du nœud [InkWord](../../com.aspose.note/inkword).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | Le nœud [InkWord](../../com.aspose.note/inkword). |

### visitLoopEnd(Loop loop) {#visitLoopEnd-com.aspose.note.Loop-}
```
public void visitLoopEnd(Loop loop)
```


Fin de la visite du nœud [Loop](../../com.aspose.note/loop).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | Le nœud [Loop](../../com.aspose.note/loop). |

### visitLoopStart(Loop loop) {#visitLoopStart-com.aspose.note.Loop-}
```
public void visitLoopStart(Loop loop)
```


Début de la visite du nœud [Loop](../../com.aspose.note/loop).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | Le nœud [Loop](../../com.aspose.note/loop). |

### visitOutlineElementEnd(OutlineElement outlineElement) {#visitOutlineElementEnd-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementEnd(OutlineElement outlineElement)
```


Fin de la visite du nœud `OutlineElement`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | Le nœud `OutlineElement`. |

### visitOutlineElementStart(OutlineElement outlineElement) {#visitOutlineElementStart-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementStart(OutlineElement outlineElement)
```


Début de la visite du nœud `OutlineElement`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | Le nœud `OutlineElement`. |

### visitOutlineEnd(Outline outline) {#visitOutlineEnd-com.aspose.note.Outline-}
```
public void visitOutlineEnd(Outline outline)
```


Fin de la visite du nœud `Outline`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | Le nœud `Outline`. |

### visitOutlineGroupEnd(OutlineGroup outlineGroup) {#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupEnd(OutlineGroup outlineGroup)
```


Fin de la visite du nœud `OutlineGroup`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | Le nœud `OutlineGroup`. |

### visitOutlineGroupStart(OutlineGroup outlineGroup) {#visitOutlineGroupStart-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupStart(OutlineGroup outlineGroup)
```


Début de la visite du nœud `OutlineGroup`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | Le nœud `OutlineGroup`. |

### visitOutlineStart(Outline outline) {#visitOutlineStart-com.aspose.note.Outline-}
```
public void visitOutlineStart(Outline outline)
```


Début de la visite du nœud `Outline`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | Le nœud `Outline`. |

### visitPageEnd(Page page) {#visitPageEnd-com.aspose.note.Page-}
```
public void visitPageEnd(Page page)
```


Fin de la visite du nœud `Page`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Le nœud `Page`. |

### visitPageStart(Page page) {#visitPageStart-com.aspose.note.Page-}
```
public void visitPageStart(Page page)
```


Début de la visite du nœud `Page`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Le nœud `Page`. |

### visitRichTextEnd(RichText richText) {#visitRichTextEnd-com.aspose.note.RichText-}
```
public void visitRichTextEnd(RichText richText)
```


Fin de la visite du nœud `RichText`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | Le nœud `RichText`. |

### visitRichTextStart(RichText richText) {#visitRichTextStart-com.aspose.note.RichText-}
```
public void visitRichTextStart(RichText richText)
```


Début de la visite du nœud `RichText`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | Le nœud `RichText`. |

### visitTableCellEnd(TableCell tableCell) {#visitTableCellEnd-com.aspose.note.TableCell-}
```
public void visitTableCellEnd(TableCell tableCell)
```


Fin de la visite du nœud `TableCell`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | Le nœud `TableCell`. |

### visitTableCellStart(TableCell tableCell) {#visitTableCellStart-com.aspose.note.TableCell-}
```
public void visitTableCellStart(TableCell tableCell)
```


Début de la visite du nœud `TableCell`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | Le nœud `TableCell`. |

### visitTableEnd(Table table) {#visitTableEnd-com.aspose.note.Table-}
```
public void visitTableEnd(Table table)
```


Fin de la visite du nœud `Table`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | Le nœud `Table`. |

### visitTableRowEnd(TableRow tableRow) {#visitTableRowEnd-com.aspose.note.TableRow-}
```
public void visitTableRowEnd(TableRow tableRow)
```


Fin de la visite du nœud `TableRow`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | Le nœud `TableRow`. |

### visitTableRowStart(TableRow tableRow) {#visitTableRowStart-com.aspose.note.TableRow-}
```
public void visitTableRowStart(TableRow tableRow)
```


Début de la visite du nœud `TableRow`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | Le nœud `TableRow`. |

### visitTableStart(Table table) {#visitTableStart-com.aspose.note.Table-}
```
public void visitTableStart(Table table)
```


Début de la visite du nœud `Table`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | Le nœud `Table`. |

### visitTitleEnd(Title title) {#visitTitleEnd-com.aspose.note.Title-}
```
public void visitTitleEnd(Title title)
```


Fin de la visite du nœud `Title`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | Le nœud `Title`. |

### visitTitleStart(Title title) {#visitTitleStart-com.aspose.note.Title-}
```
public void visitTitleStart(Title title)
```


Début de la visite du nœud `Title`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | Le nœud `Title`. |

