---
title: "DocumentVisitor"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Kelas abstrak untuk iterasi melalui subtree dengan akar pada node yang ditentukan."
type: docs
weight: 22
url: /id/java/com.aspose.note/documentvisitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class DocumentVisitor
```

Kelas abstrak untuk iterasi melalui subtree dengan akar pada node yang ditentukan.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [DocumentVisitor()](#DocumentVisitor--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [visitAttachedFileEnd(AttachedFile attachedFile)](#visitAttachedFileEnd-com.aspose.note.AttachedFile-) | Akhir untuk mengunjungi node `AttachedFile`. |
| [visitAttachedFileStart(AttachedFile attachedFile)](#visitAttachedFileStart-com.aspose.note.AttachedFile-) | Mulai mengunjungi node `AttachedFile`. |
| [visitDocumentEnd(Document document)](#visitDocumentEnd-com.aspose.note.Document-) | Selesai mengunjungi node `Document`. |
| [visitDocumentStart(Document document)](#visitDocumentStart-com.aspose.note.Document-) | Mulai mengunjungi node `Document`. |
| [visitImageEnd(Image image)](#visitImageEnd-com.aspose.note.Image-) | Selesai mengunjungi node `Image`. |
| [visitImageStart(Image image)](#visitImageStart-com.aspose.note.Image-) | Mulai mengunjungi node `Image`. |
| [visitInkDrawingEnd(InkDrawing inkDrawing)](#visitInkDrawingEnd-com.aspose.note.InkDrawing-) | Selesai mengunjungi node [InkDrawing](../../com.aspose.note/inkdrawing). |
| [visitInkDrawingStart(InkDrawing inkDrawing)](#visitInkDrawingStart-com.aspose.note.InkDrawing-) | Mulai mengunjungi node [InkDrawing](../../com.aspose.note/inkdrawing). |
| [visitInkParagraphEnd(InkParagraph inkParagraph)](#visitInkParagraphEnd-com.aspose.note.InkParagraph-) | Selesai mengunjungi node [InkParagraph](../../com.aspose.note/inkparagraph). |
| [visitInkParagraphStart(InkParagraph inkParagraph)](#visitInkParagraphStart-com.aspose.note.InkParagraph-) | Mulai mengunjungi node [InkParagraph](../../com.aspose.note/inkparagraph). |
| [visitInkWordEnd(InkWord inkWord)](#visitInkWordEnd-com.aspose.note.InkWord-) | Selesai mengunjungi node [InkWord](../../com.aspose.note/inkword). |
| [visitInkWordStart(InkWord inkWord)](#visitInkWordStart-com.aspose.note.InkWord-) | Mulai mengunjungi node [InkWord](../../com.aspose.note/inkword). |
| [visitLoopEnd(Loop loop)](#visitLoopEnd-com.aspose.note.Loop-) | Selesai mengunjungi node [Loop](../../com.aspose.note/loop). |
| [visitLoopStart(Loop loop)](#visitLoopStart-com.aspose.note.Loop-) | Mulai mengunjungi node [Loop](../../com.aspose.note/loop). |
| [visitOutlineElementEnd(OutlineElement outlineElement)](#visitOutlineElementEnd-com.aspose.note.OutlineElement-) | Selesai mengunjungi node `OutlineElement`. |
| [visitOutlineElementStart(OutlineElement outlineElement)](#visitOutlineElementStart-com.aspose.note.OutlineElement-) | Mulai mengunjungi node `OutlineElement`. |
| [visitOutlineEnd(Outline outline)](#visitOutlineEnd-com.aspose.note.Outline-) | Selesai mengunjungi node `Outline`. |
| [visitOutlineGroupEnd(OutlineGroup outlineGroup)](#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-) | Selesai mengunjungi node `OutlineGroup`. |
| [visitOutlineGroupStart(OutlineGroup outlineGroup)](#visitOutlineGroupStart-com.aspose.note.OutlineGroup-) | Mulai mengunjungi node `OutlineGroup`. |
| [visitOutlineStart(Outline outline)](#visitOutlineStart-com.aspose.note.Outline-) | Mulai mengunjungi node `Outline`. |
| [visitPageEnd(Page page)](#visitPageEnd-com.aspose.note.Page-) | Selesai mengunjungi node `Page`. |
| [visitPageStart(Page page)](#visitPageStart-com.aspose.note.Page-) | Mulai mengunjungi node `Page`. |
| [visitRichTextEnd(RichText richText)](#visitRichTextEnd-com.aspose.note.RichText-) | Selesai mengunjungi node `RichText`. |
| [visitRichTextStart(RichText richText)](#visitRichTextStart-com.aspose.note.RichText-) | Mulai mengunjungi node `RichText`. |
| [visitTableCellEnd(TableCell tableCell)](#visitTableCellEnd-com.aspose.note.TableCell-) | Selesai mengunjungi node `TableCell`. |
| [visitTableCellStart(TableCell tableCell)](#visitTableCellStart-com.aspose.note.TableCell-) | Mulai mengunjungi node `TableCell`. |
| [visitTableEnd(Table table)](#visitTableEnd-com.aspose.note.Table-) | Akhir untuk mengunjungi node `Table`. |
| [visitTableRowEnd(TableRow tableRow)](#visitTableRowEnd-com.aspose.note.TableRow-) | Akhir untuk mengunjungi node `TableRow`. |
| [visitTableRowStart(TableRow tableRow)](#visitTableRowStart-com.aspose.note.TableRow-) | Mulai mengunjungi node `TableRow`. |
| [visitTableStart(Table table)](#visitTableStart-com.aspose.note.Table-) | Mulai mengunjungi node `Table`. |
| [visitTitleEnd(Title title)](#visitTitleEnd-com.aspose.note.Title-) | Akhir untuk mengunjungi node `Title`. |
| [visitTitleStart(Title title)](#visitTitleStart-com.aspose.note.Title-) | Mulai mengunjungi node `Title`. |
### DocumentVisitor() {#DocumentVisitor--}
```
public DocumentVisitor()
```


### visitAttachedFileEnd(AttachedFile attachedFile) {#visitAttachedFileEnd-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileEnd(AttachedFile attachedFile)
```


Akhir untuk mengunjungi node `AttachedFile`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | Node `AttachedFile`. |

### visitAttachedFileStart(AttachedFile attachedFile) {#visitAttachedFileStart-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileStart(AttachedFile attachedFile)
```


Mulai mengunjungi node `AttachedFile`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | Node `AttachedFile`. |

### visitDocumentEnd(Document document) {#visitDocumentEnd-com.aspose.note.Document-}
```
public void visitDocumentEnd(Document document)
```


Selesai mengunjungi node `Document`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | Node `Document`. |

### visitDocumentStart(Document document) {#visitDocumentStart-com.aspose.note.Document-}
```
public void visitDocumentStart(Document document)
```


Mulai mengunjungi node `Document`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | Node `Document`. |

### visitImageEnd(Image image) {#visitImageEnd-com.aspose.note.Image-}
```
public void visitImageEnd(Image image)
```


Selesai mengunjungi node `Image`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | Node `Image`. |

### visitImageStart(Image image) {#visitImageStart-com.aspose.note.Image-}
```
public void visitImageStart(Image image)
```


Mulai mengunjungi node `Image`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | Node `Image`. |

### visitInkDrawingEnd(InkDrawing inkDrawing) {#visitInkDrawingEnd-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingEnd(InkDrawing inkDrawing)
```


Selesai mengunjungi node [InkDrawing](../../com.aspose.note/inkdrawing).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | Node [InkDrawing](../../com.aspose.note/inkdrawing). |

### visitInkDrawingStart(InkDrawing inkDrawing) {#visitInkDrawingStart-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingStart(InkDrawing inkDrawing)
```


Mulai mengunjungi node [InkDrawing](../../com.aspose.note/inkdrawing).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | Node [InkDrawing](../../com.aspose.note/inkdrawing). |

### visitInkParagraphEnd(InkParagraph inkParagraph) {#visitInkParagraphEnd-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphEnd(InkParagraph inkParagraph)
```


Selesai mengunjungi node [InkParagraph](../../com.aspose.note/inkparagraph).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | Node [InkParagraph](../../com.aspose.note/inkparagraph). |

### visitInkParagraphStart(InkParagraph inkParagraph) {#visitInkParagraphStart-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphStart(InkParagraph inkParagraph)
```


Mulai mengunjungi node [InkParagraph](../../com.aspose.note/inkparagraph).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | Node [InkParagraph](../../com.aspose.note/inkparagraph). |

### visitInkWordEnd(InkWord inkWord) {#visitInkWordEnd-com.aspose.note.InkWord-}
```
public void visitInkWordEnd(InkWord inkWord)
```


Selesai mengunjungi node [InkWord](../../com.aspose.note/inkword).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | Node [InkWord](../../com.aspose.note/inkword). |

### visitInkWordStart(InkWord inkWord) {#visitInkWordStart-com.aspose.note.InkWord-}
```
public void visitInkWordStart(InkWord inkWord)
```


Mulai mengunjungi node [InkWord](../../com.aspose.note/inkword).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | Node [InkWord](../../com.aspose.note/inkword). |

### visitLoopEnd(Loop loop) {#visitLoopEnd-com.aspose.note.Loop-}
```
public void visitLoopEnd(Loop loop)
```


Selesai mengunjungi node [Loop](../../com.aspose.note/loop).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | Node [Loop](../../com.aspose.note/loop). |

### visitLoopStart(Loop loop) {#visitLoopStart-com.aspose.note.Loop-}
```
public void visitLoopStart(Loop loop)
```


Mulai mengunjungi node [Loop](../../com.aspose.note/loop).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | Node [Loop](../../com.aspose.note/loop). |

### visitOutlineElementEnd(OutlineElement outlineElement) {#visitOutlineElementEnd-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementEnd(OutlineElement outlineElement)
```


Selesai mengunjungi node `OutlineElement`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | Node `OutlineElement`. |

### visitOutlineElementStart(OutlineElement outlineElement) {#visitOutlineElementStart-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementStart(OutlineElement outlineElement)
```


Mulai mengunjungi node `OutlineElement`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | Node `OutlineElement`. |

### visitOutlineEnd(Outline outline) {#visitOutlineEnd-com.aspose.note.Outline-}
```
public void visitOutlineEnd(Outline outline)
```


Selesai mengunjungi node `Outline`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | Node `Outline`. |

### visitOutlineGroupEnd(OutlineGroup outlineGroup) {#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupEnd(OutlineGroup outlineGroup)
```


Selesai mengunjungi node `OutlineGroup`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | Node `OutlineGroup`. |

### visitOutlineGroupStart(OutlineGroup outlineGroup) {#visitOutlineGroupStart-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupStart(OutlineGroup outlineGroup)
```


Mulai mengunjungi node `OutlineGroup`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | Node `OutlineGroup`. |

### visitOutlineStart(Outline outline) {#visitOutlineStart-com.aspose.note.Outline-}
```
public void visitOutlineStart(Outline outline)
```


Mulai mengunjungi node `Outline`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | Node `Outline`. |

### visitPageEnd(Page page) {#visitPageEnd-com.aspose.note.Page-}
```
public void visitPageEnd(Page page)
```


Selesai mengunjungi node `Page`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Node `Page`. |

### visitPageStart(Page page) {#visitPageStart-com.aspose.note.Page-}
```
public void visitPageStart(Page page)
```


Mulai mengunjungi node `Page`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Node `Page`. |

### visitRichTextEnd(RichText richText) {#visitRichTextEnd-com.aspose.note.RichText-}
```
public void visitRichTextEnd(RichText richText)
```


Selesai mengunjungi node `RichText`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | Node `RichText`. |

### visitRichTextStart(RichText richText) {#visitRichTextStart-com.aspose.note.RichText-}
```
public void visitRichTextStart(RichText richText)
```


Mulai mengunjungi node `RichText`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | Node `RichText`. |

### visitTableCellEnd(TableCell tableCell) {#visitTableCellEnd-com.aspose.note.TableCell-}
```
public void visitTableCellEnd(TableCell tableCell)
```


Selesai mengunjungi node `TableCell`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | Node `TableCell`. |

### visitTableCellStart(TableCell tableCell) {#visitTableCellStart-com.aspose.note.TableCell-}
```
public void visitTableCellStart(TableCell tableCell)
```


Mulai mengunjungi node `TableCell`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | Node `TableCell`. |

### visitTableEnd(Table table) {#visitTableEnd-com.aspose.note.Table-}
```
public void visitTableEnd(Table table)
```


Akhir untuk mengunjungi node `Table`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | Node `Table`. |

### visitTableRowEnd(TableRow tableRow) {#visitTableRowEnd-com.aspose.note.TableRow-}
```
public void visitTableRowEnd(TableRow tableRow)
```


Akhir untuk mengunjungi node `TableRow`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | Node `TableRow`. |

### visitTableRowStart(TableRow tableRow) {#visitTableRowStart-com.aspose.note.TableRow-}
```
public void visitTableRowStart(TableRow tableRow)
```


Mulai mengunjungi node `TableRow`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | Node `TableRow`. |

### visitTableStart(Table table) {#visitTableStart-com.aspose.note.Table-}
```
public void visitTableStart(Table table)
```


Mulai mengunjungi node `Table`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | Node `Table`. |

### visitTitleEnd(Title title) {#visitTitleEnd-com.aspose.note.Title-}
```
public void visitTitleEnd(Title title)
```


Akhir untuk mengunjungi node `Title`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | Node `Title`. |

### visitTitleStart(Title title) {#visitTitleStart-com.aspose.note.Title-}
```
public void visitTitleStart(Title title)
```


Mulai mengunjungi node `Title`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | Node `Title`. |

