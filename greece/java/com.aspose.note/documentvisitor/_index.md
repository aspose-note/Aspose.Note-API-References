---
title: "DocumentVisitor"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Η αφηρημένη κλάση για την επανάληψη μέσω του υποδέντρου με ρίζα στον καθορισμένο κόμβο."
type: docs
weight: 22
url: /el/java/com.aspose.note/documentvisitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class DocumentVisitor
```

Η αφηρημένη κλάση για την επανάληψη μέσω του υποδέντρου με ρίζα στον καθορισμένο κόμβο.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [DocumentVisitor()](#DocumentVisitor--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [visitAttachedFileEnd(AttachedFile attachedFile)](#visitAttachedFileEnd-com.aspose.note.AttachedFile-) | Τέλος για την επίσκεψη του κόμβου `AttachedFile`. |
| [visitAttachedFileStart(AttachedFile attachedFile)](#visitAttachedFileStart-com.aspose.note.AttachedFile-) | Ξεκινήστε την επίσκεψη στον κόμβο `AttachedFile`. |
| [visitDocumentEnd(Document document)](#visitDocumentEnd-com.aspose.note.Document-) | Τελειώστε την επίσκεψη στον κόμβο `Document`. |
| [visitDocumentStart(Document document)](#visitDocumentStart-com.aspose.note.Document-) | Ξεκινήστε την επίσκεψη στον κόμβο `Document`. |
| [visitImageEnd(Image image)](#visitImageEnd-com.aspose.note.Image-) | Τελειώστε την επίσκεψη στον κόμβο `Image`. |
| [visitImageStart(Image image)](#visitImageStart-com.aspose.note.Image-) | Ξεκινήστε την επίσκεψη στον κόμβο `Image`. |
| [visitInkDrawingEnd(InkDrawing inkDrawing)](#visitInkDrawingEnd-com.aspose.note.InkDrawing-) | Τελειώστε την επίσκεψη στον κόμβο [InkDrawing](../../com.aspose.note/inkdrawing). |
| [visitInkDrawingStart(InkDrawing inkDrawing)](#visitInkDrawingStart-com.aspose.note.InkDrawing-) | Ξεκινήστε την επίσκεψη στον κόμβο [InkDrawing](../../com.aspose.note/inkdrawing). |
| [visitInkParagraphEnd(InkParagraph inkParagraph)](#visitInkParagraphEnd-com.aspose.note.InkParagraph-) | Τελειώστε την επίσκεψη στον κόμβο [InkParagraph](../../com.aspose.note/inkparagraph). |
| [visitInkParagraphStart(InkParagraph inkParagraph)](#visitInkParagraphStart-com.aspose.note.InkParagraph-) | Ξεκινήστε την επίσκεψη στον κόμβο [InkParagraph](../../com.aspose.note/inkparagraph). |
| [visitInkWordEnd(InkWord inkWord)](#visitInkWordEnd-com.aspose.note.InkWord-) | Τελειώστε την επίσκεψη στον κόμβο [InkWord](../../com.aspose.note/inkword). |
| [visitInkWordStart(InkWord inkWord)](#visitInkWordStart-com.aspose.note.InkWord-) | Ξεκινήστε την επίσκεψη στον κόμβο [InkWord](../../com.aspose.note/inkword). |
| [visitLoopEnd(Loop loop)](#visitLoopEnd-com.aspose.note.Loop-) | Τελειώστε την επίσκεψη στον κόμβο [Loop](../../com.aspose.note/loop). |
| [visitLoopStart(Loop loop)](#visitLoopStart-com.aspose.note.Loop-) | Ξεκινήστε την επίσκεψη στον κόμβο [Loop](../../com.aspose.note/loop). |
| [visitOutlineElementEnd(OutlineElement outlineElement)](#visitOutlineElementEnd-com.aspose.note.OutlineElement-) | Τελειώστε την επίσκεψη στον κόμβο `OutlineElement`. |
| [visitOutlineElementStart(OutlineElement outlineElement)](#visitOutlineElementStart-com.aspose.note.OutlineElement-) | Ξεκινήστε την επίσκεψη στον κόμβο `OutlineElement`. |
| [visitOutlineEnd(Outline outline)](#visitOutlineEnd-com.aspose.note.Outline-) | Τελειώστε την επίσκεψη στον κόμβο `Outline`. |
| [visitOutlineGroupEnd(OutlineGroup outlineGroup)](#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-) | Τελειώστε την επίσκεψη στον κόμβο `OutlineGroup`. |
| [visitOutlineGroupStart(OutlineGroup outlineGroup)](#visitOutlineGroupStart-com.aspose.note.OutlineGroup-) | Ξεκινήστε την επίσκεψη στον κόμβο `OutlineGroup`. |
| [visitOutlineStart(Outline outline)](#visitOutlineStart-com.aspose.note.Outline-) | Ξεκινήστε την επίσκεψη στον κόμβο `Outline`. |
| [visitPageEnd(Page page)](#visitPageEnd-com.aspose.note.Page-) | Τελειώστε την επίσκεψη στον κόμβο `Page`. |
| [visitPageStart(Page page)](#visitPageStart-com.aspose.note.Page-) | Ξεκινήστε την επίσκεψη στον κόμβο `Page`. |
| [visitRichTextEnd(RichText richText)](#visitRichTextEnd-com.aspose.note.RichText-) | Τελειώστε την επίσκεψη στον κόμβο `RichText`. |
| [visitRichTextStart(RichText richText)](#visitRichTextStart-com.aspose.note.RichText-) | Ξεκινήστε την επίσκεψη στον κόμβο `RichText`. |
| [visitTableCellEnd(TableCell tableCell)](#visitTableCellEnd-com.aspose.note.TableCell-) | Τελειώστε την επίσκεψη στον κόμβο `TableCell`. |
| [visitTableCellStart(TableCell tableCell)](#visitTableCellStart-com.aspose.note.TableCell-) | Ξεκινήστε την επίσκεψη στον κόμβο `TableCell`. |
| [visitTableEnd(Table table)](#visitTableEnd-com.aspose.note.Table-) | Τέλος της επίσκεψης του κόμβου `Table`. |
| [visitTableRowEnd(TableRow tableRow)](#visitTableRowEnd-com.aspose.note.TableRow-) | Τέλος της επίσκεψης του κόμβου `TableRow`. |
| [visitTableRowStart(TableRow tableRow)](#visitTableRowStart-com.aspose.note.TableRow-) | Έναρξη της επίσκεψης του κόμβου `TableRow`. |
| [visitTableStart(Table table)](#visitTableStart-com.aspose.note.Table-) | Έναρξη της επίσκεψης του κόμβου `Table`. |
| [visitTitleEnd(Title title)](#visitTitleEnd-com.aspose.note.Title-) | Τέλος της επίσκεψης του κόμβου `Title`. |
| [visitTitleStart(Title title)](#visitTitleStart-com.aspose.note.Title-) | Έναρξη της επίσκεψης του κόμβου `Title`. |
### DocumentVisitor() {#DocumentVisitor--}
```
public DocumentVisitor()
```


### visitAttachedFileEnd(AttachedFile attachedFile) {#visitAttachedFileEnd-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileEnd(AttachedFile attachedFile)
```


Τέλος για την επίσκεψη του κόμβου `AttachedFile`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | Ο κόμβος `AttachedFile`. |

### visitAttachedFileStart(AttachedFile attachedFile) {#visitAttachedFileStart-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileStart(AttachedFile attachedFile)
```


Ξεκινήστε την επίσκεψη στον κόμβο `AttachedFile`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | Ο κόμβος `AttachedFile`. |

### visitDocumentEnd(Document document) {#visitDocumentEnd-com.aspose.note.Document-}
```
public void visitDocumentEnd(Document document)
```


Τελειώστε την επίσκεψη στον κόμβο `Document`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | Ο κόμβος `Document`. |

### visitDocumentStart(Document document) {#visitDocumentStart-com.aspose.note.Document-}
```
public void visitDocumentStart(Document document)
```


Ξεκινήστε την επίσκεψη στον κόμβο `Document`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | Ο κόμβος `Document`. |

### visitImageEnd(Image image) {#visitImageEnd-com.aspose.note.Image-}
```
public void visitImageEnd(Image image)
```


Τελειώστε την επίσκεψη στον κόμβο `Image`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | Ο κόμβος `Image`. |

### visitImageStart(Image image) {#visitImageStart-com.aspose.note.Image-}
```
public void visitImageStart(Image image)
```


Ξεκινήστε την επίσκεψη στον κόμβο `Image`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | Ο κόμβος `Image`. |

### visitInkDrawingEnd(InkDrawing inkDrawing) {#visitInkDrawingEnd-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingEnd(InkDrawing inkDrawing)
```


Τελειώστε την επίσκεψη στον κόμβο [InkDrawing](../../com.aspose.note/inkdrawing).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | Ο κόμβος [InkDrawing](../../com.aspose.note/inkdrawing). |

### visitInkDrawingStart(InkDrawing inkDrawing) {#visitInkDrawingStart-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingStart(InkDrawing inkDrawing)
```


Ξεκινήστε την επίσκεψη στον κόμβο [InkDrawing](../../com.aspose.note/inkdrawing).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | Ο κόμβος [InkDrawing](../../com.aspose.note/inkdrawing). |

### visitInkParagraphEnd(InkParagraph inkParagraph) {#visitInkParagraphEnd-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphEnd(InkParagraph inkParagraph)
```


Τελειώστε την επίσκεψη στον κόμβο [InkParagraph](../../com.aspose.note/inkparagraph).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | Ο κόμβος [InkParagraph](../../com.aspose.note/inkparagraph). |

### visitInkParagraphStart(InkParagraph inkParagraph) {#visitInkParagraphStart-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphStart(InkParagraph inkParagraph)
```


Ξεκινήστε την επίσκεψη στον κόμβο [InkParagraph](../../com.aspose.note/inkparagraph).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | Ο κόμβος [InkParagraph](../../com.aspose.note/inkparagraph). |

### visitInkWordEnd(InkWord inkWord) {#visitInkWordEnd-com.aspose.note.InkWord-}
```
public void visitInkWordEnd(InkWord inkWord)
```


Τελειώστε την επίσκεψη στον κόμβο [InkWord](../../com.aspose.note/inkword).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | Ο κόμβος [InkWord](../../com.aspose.note/inkword). |

### visitInkWordStart(InkWord inkWord) {#visitInkWordStart-com.aspose.note.InkWord-}
```
public void visitInkWordStart(InkWord inkWord)
```


Ξεκινήστε την επίσκεψη στον κόμβο [InkWord](../../com.aspose.note/inkword).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | Ο κόμβος [InkWord](../../com.aspose.note/inkword). |

### visitLoopEnd(Loop loop) {#visitLoopEnd-com.aspose.note.Loop-}
```
public void visitLoopEnd(Loop loop)
```


Τελειώστε την επίσκεψη στον κόμβο [Loop](../../com.aspose.note/loop).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | Ο κόμβος [Loop](../../com.aspose.note/loop). |

### visitLoopStart(Loop loop) {#visitLoopStart-com.aspose.note.Loop-}
```
public void visitLoopStart(Loop loop)
```


Ξεκινήστε την επίσκεψη στον κόμβο [Loop](../../com.aspose.note/loop).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | Ο κόμβος [Loop](../../com.aspose.note/loop). |

### visitOutlineElementEnd(OutlineElement outlineElement) {#visitOutlineElementEnd-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementEnd(OutlineElement outlineElement)
```


Τελειώστε την επίσκεψη στον κόμβο `OutlineElement`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | Ο κόμβος `OutlineElement`. |

### visitOutlineElementStart(OutlineElement outlineElement) {#visitOutlineElementStart-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementStart(OutlineElement outlineElement)
```


Ξεκινήστε την επίσκεψη στον κόμβο `OutlineElement`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | Ο κόμβος `OutlineElement`. |

### visitOutlineEnd(Outline outline) {#visitOutlineEnd-com.aspose.note.Outline-}
```
public void visitOutlineEnd(Outline outline)
```


Τελειώστε την επίσκεψη στον κόμβο `Outline`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | Ο κόμβος `Outline`. |

### visitOutlineGroupEnd(OutlineGroup outlineGroup) {#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupEnd(OutlineGroup outlineGroup)
```


Τελειώστε την επίσκεψη στον κόμβο `OutlineGroup`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | Ο κόμβος `OutlineGroup`. |

### visitOutlineGroupStart(OutlineGroup outlineGroup) {#visitOutlineGroupStart-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupStart(OutlineGroup outlineGroup)
```


Ξεκινήστε την επίσκεψη στον κόμβο `OutlineGroup`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | Ο κόμβος `OutlineGroup`. |

### visitOutlineStart(Outline outline) {#visitOutlineStart-com.aspose.note.Outline-}
```
public void visitOutlineStart(Outline outline)
```


Ξεκινήστε την επίσκεψη στον κόμβο `Outline`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | Ο κόμβος `Outline`. |

### visitPageEnd(Page page) {#visitPageEnd-com.aspose.note.Page-}
```
public void visitPageEnd(Page page)
```


Τελειώστε την επίσκεψη στον κόμβο `Page`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Ο κόμβος `Page`. |

### visitPageStart(Page page) {#visitPageStart-com.aspose.note.Page-}
```
public void visitPageStart(Page page)
```


Ξεκινήστε την επίσκεψη στον κόμβο `Page`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Ο κόμβος `Page`. |

### visitRichTextEnd(RichText richText) {#visitRichTextEnd-com.aspose.note.RichText-}
```
public void visitRichTextEnd(RichText richText)
```


Τελειώστε την επίσκεψη στον κόμβο `RichText`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | Ο κόμβος `RichText`. |

### visitRichTextStart(RichText richText) {#visitRichTextStart-com.aspose.note.RichText-}
```
public void visitRichTextStart(RichText richText)
```


Ξεκινήστε την επίσκεψη στον κόμβο `RichText`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | Ο κόμβος `RichText`. |

### visitTableCellEnd(TableCell tableCell) {#visitTableCellEnd-com.aspose.note.TableCell-}
```
public void visitTableCellEnd(TableCell tableCell)
```


Τελειώστε την επίσκεψη στον κόμβο `TableCell`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | Ο κόμβος `TableCell`. |

### visitTableCellStart(TableCell tableCell) {#visitTableCellStart-com.aspose.note.TableCell-}
```
public void visitTableCellStart(TableCell tableCell)
```


Ξεκινήστε την επίσκεψη στον κόμβο `TableCell`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | Ο κόμβος `TableCell`. |

### visitTableEnd(Table table) {#visitTableEnd-com.aspose.note.Table-}
```
public void visitTableEnd(Table table)
```


Τέλος της επίσκεψης του κόμβου `Table`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | Ο κόμβος `Table`. |

### visitTableRowEnd(TableRow tableRow) {#visitTableRowEnd-com.aspose.note.TableRow-}
```
public void visitTableRowEnd(TableRow tableRow)
```


Τέλος της επίσκεψης του κόμβου `TableRow`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | Ο κόμβος `TableRow`. |

### visitTableRowStart(TableRow tableRow) {#visitTableRowStart-com.aspose.note.TableRow-}
```
public void visitTableRowStart(TableRow tableRow)
```


Έναρξη της επίσκεψης του κόμβου `TableRow`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | Ο κόμβος `TableRow`. |

### visitTableStart(Table table) {#visitTableStart-com.aspose.note.Table-}
```
public void visitTableStart(Table table)
```


Έναρξη της επίσκεψης του κόμβου `Table`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | Ο κόμβος `Table`. |

### visitTitleEnd(Title title) {#visitTitleEnd-com.aspose.note.Title-}
```
public void visitTitleEnd(Title title)
```


Τέλος της επίσκεψης του κόμβου `Title`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | Ο κόμβος `Title`. |

### visitTitleStart(Title title) {#visitTitleStart-com.aspose.note.Title-}
```
public void visitTitleStart(Title title)
```


Έναρξη της επίσκεψης του κόμβου `Title`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | Ο κόμβος `Title`. |

