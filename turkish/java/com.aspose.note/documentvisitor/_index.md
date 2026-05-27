---
title: "DocumentVisitor"
second_title: "Aspose.Note for Java API Referansı"
description: "Belirtilen düğümde kök olan alt ağaçta yineleme yapmak için soyut sınıf."
type: docs
weight: 22
url: /tr/java/com.aspose.note/documentvisitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class DocumentVisitor
```

Belirtilen düğümde kök olan alt ağaçta yineleme yapmak için soyut sınıf.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [DocumentVisitor()](#DocumentVisitor--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [visitAttachedFileEnd(AttachedFile attachedFile)](#visitAttachedFileEnd-com.aspose.note.AttachedFile-) | `AttachedFile` düğümünü ziyaret etmeyi bitir. |
| [visitAttachedFileStart(AttachedFile attachedFile)](#visitAttachedFileStart-com.aspose.note.AttachedFile-) | Başlat `AttachedFile` düğümünü ziyaret etmeyi. |
| [visitDocumentEnd(Document document)](#visitDocumentEnd-com.aspose.note.Document-) | Bitir `Document` düğümünü ziyaret etmeyi. |
| [visitDocumentStart(Document document)](#visitDocumentStart-com.aspose.note.Document-) | Başlat `Document` düğümünü ziyaret etmeyi. |
| [visitImageEnd(Image image)](#visitImageEnd-com.aspose.note.Image-) | Bitir `Image` düğümünü ziyaret etmeyi. |
| [visitImageStart(Image image)](#visitImageStart-com.aspose.note.Image-) | Başlat `Image` düğümünü ziyaret etmeyi. |
| [visitInkDrawingEnd(InkDrawing inkDrawing)](#visitInkDrawingEnd-com.aspose.note.InkDrawing-) | Bitir [InkDrawing](../../com.aspose.note/inkdrawing) düğümünü ziyaret etmeyi. |
| [visitInkDrawingStart(InkDrawing inkDrawing)](#visitInkDrawingStart-com.aspose.note.InkDrawing-) | Başlat [InkDrawing](../../com.aspose.note/inkdrawing) düğümünü ziyaret etmeyi. |
| [visitInkParagraphEnd(InkParagraph inkParagraph)](#visitInkParagraphEnd-com.aspose.note.InkParagraph-) | Bitir [InkParagraph](../../com.aspose.note/inkparagraph) düğümünü ziyaret etmeyi. |
| [visitInkParagraphStart(InkParagraph inkParagraph)](#visitInkParagraphStart-com.aspose.note.InkParagraph-) | Başlat [InkParagraph](../../com.aspose.note/inkparagraph) düğümünü ziyaret etmeyi. |
| [visitInkWordEnd(InkWord inkWord)](#visitInkWordEnd-com.aspose.note.InkWord-) | Bitir [InkWord](../../com.aspose.note/inkword) düğümünü ziyaret etmeyi. |
| [visitInkWordStart(InkWord inkWord)](#visitInkWordStart-com.aspose.note.InkWord-) | Başlat [InkWord](../../com.aspose.note/inkword) düğümünü ziyaret etmeyi. |
| [visitLoopEnd(Loop loop)](#visitLoopEnd-com.aspose.note.Loop-) | Bitir [Loop](../../com.aspose.note/loop) düğümünü ziyaret etmeyi. |
| [visitLoopStart(Loop loop)](#visitLoopStart-com.aspose.note.Loop-) | Başlat [Loop](../../com.aspose.note/loop) düğümünü ziyaret etmeyi. |
| [visitOutlineElementEnd(OutlineElement outlineElement)](#visitOutlineElementEnd-com.aspose.note.OutlineElement-) | Bitir `OutlineElement` düğümünü ziyaret etmeyi. |
| [visitOutlineElementStart(OutlineElement outlineElement)](#visitOutlineElementStart-com.aspose.note.OutlineElement-) | Başlat `OutlineElement` düğümünü ziyaret etmeyi. |
| [visitOutlineEnd(Outline outline)](#visitOutlineEnd-com.aspose.note.Outline-) | Bitir `Outline` düğümünü ziyaret etmeyi. |
| [visitOutlineGroupEnd(OutlineGroup outlineGroup)](#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-) | Bitir `OutlineGroup` düğümünü ziyaret etmeyi. |
| [visitOutlineGroupStart(OutlineGroup outlineGroup)](#visitOutlineGroupStart-com.aspose.note.OutlineGroup-) | Başlat `OutlineGroup` düğümünü ziyaret etmeyi. |
| [visitOutlineStart(Outline outline)](#visitOutlineStart-com.aspose.note.Outline-) | Başlat `Outline` düğümünü ziyaret etmeyi. |
| [visitPageEnd(Page page)](#visitPageEnd-com.aspose.note.Page-) | Bitir `Page` düğümünü ziyaret etmeyi. |
| [visitPageStart(Page page)](#visitPageStart-com.aspose.note.Page-) | Başlat `Page` düğümünü ziyaret etmeyi. |
| [visitRichTextEnd(RichText richText)](#visitRichTextEnd-com.aspose.note.RichText-) | Bitir `RichText` düğümünü ziyaret etmeyi. |
| [visitRichTextStart(RichText richText)](#visitRichTextStart-com.aspose.note.RichText-) | Başlat `RichText` düğümünü ziyaret etmeyi. |
| [visitTableCellEnd(TableCell tableCell)](#visitTableCellEnd-com.aspose.note.TableCell-) | Bitir `TableCell` düğümünü ziyaret etmeyi. |
| [visitTableCellStart(TableCell tableCell)](#visitTableCellStart-com.aspose.note.TableCell-) | Başlat `TableCell` düğümünü ziyaret etmeyi. |
| [visitTableEnd(Table table)](#visitTableEnd-com.aspose.note.Table-) | `Table` düğümünü ziyaret etmeyi bitir. |
| [visitTableRowEnd(TableRow tableRow)](#visitTableRowEnd-com.aspose.note.TableRow-) | `TableRow` düğümünü ziyaret etmeyi bitir. |
| [visitTableRowStart(TableRow tableRow)](#visitTableRowStart-com.aspose.note.TableRow-) | `TableRow` düğümünü ziyaret etmeye başla. |
| [visitTableStart(Table table)](#visitTableStart-com.aspose.note.Table-) | `Table` düğümünü ziyaret etmeye başla. |
| [visitTitleEnd(Title title)](#visitTitleEnd-com.aspose.note.Title-) | `Title` düğümünü ziyaret etmeyi bitir. |
| [visitTitleStart(Title title)](#visitTitleStart-com.aspose.note.Title-) | `Title` düğümünü ziyaret etmeye başla. |
### DocumentVisitor() {#DocumentVisitor--}
```
public DocumentVisitor()
```


### visitAttachedFileEnd(AttachedFile attachedFile) {#visitAttachedFileEnd-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileEnd(AttachedFile attachedFile)
```


`AttachedFile` düğümünü ziyaret etmeyi bitir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | `AttachedFile` düğümü. |

### visitAttachedFileStart(AttachedFile attachedFile) {#visitAttachedFileStart-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileStart(AttachedFile attachedFile)
```


Başlat `AttachedFile` düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | `AttachedFile` düğümü. |

### visitDocumentEnd(Document document) {#visitDocumentEnd-com.aspose.note.Document-}
```
public void visitDocumentEnd(Document document)
```


Bitir `Document` düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | `Document` düğümü. |

### visitDocumentStart(Document document) {#visitDocumentStart-com.aspose.note.Document-}
```
public void visitDocumentStart(Document document)
```


Başlat `Document` düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | `Document` düğümü. |

### visitImageEnd(Image image) {#visitImageEnd-com.aspose.note.Image-}
```
public void visitImageEnd(Image image)
```


Bitir `Image` düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | `Image` düğümü. |

### visitImageStart(Image image) {#visitImageStart-com.aspose.note.Image-}
```
public void visitImageStart(Image image)
```


Başlat `Image` düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | `Image` düğümü. |

### visitInkDrawingEnd(InkDrawing inkDrawing) {#visitInkDrawingEnd-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingEnd(InkDrawing inkDrawing)
```


Bitir [InkDrawing](../../com.aspose.note/inkdrawing) düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | [InkDrawing](../../com.aspose.note/inkdrawing) düğümü. |

### visitInkDrawingStart(InkDrawing inkDrawing) {#visitInkDrawingStart-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingStart(InkDrawing inkDrawing)
```


Başlat [InkDrawing](../../com.aspose.note/inkdrawing) düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | [InkDrawing](../../com.aspose.note/inkdrawing) düğümü. |

### visitInkParagraphEnd(InkParagraph inkParagraph) {#visitInkParagraphEnd-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphEnd(InkParagraph inkParagraph)
```


Bitir [InkParagraph](../../com.aspose.note/inkparagraph) düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | [InkParagraph](../../com.aspose.note/inkparagraph) düğümü. |

### visitInkParagraphStart(InkParagraph inkParagraph) {#visitInkParagraphStart-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphStart(InkParagraph inkParagraph)
```


Başlat [InkParagraph](../../com.aspose.note/inkparagraph) düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | [InkParagraph](../../com.aspose.note/inkparagraph) düğümü. |

### visitInkWordEnd(InkWord inkWord) {#visitInkWordEnd-com.aspose.note.InkWord-}
```
public void visitInkWordEnd(InkWord inkWord)
```


Bitir [InkWord](../../com.aspose.note/inkword) düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | [InkWord](../../com.aspose.note/inkword) düğümü. |

### visitInkWordStart(InkWord inkWord) {#visitInkWordStart-com.aspose.note.InkWord-}
```
public void visitInkWordStart(InkWord inkWord)
```


Başlat [InkWord](../../com.aspose.note/inkword) düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | [InkWord](../../com.aspose.note/inkword) düğümü. |

### visitLoopEnd(Loop loop) {#visitLoopEnd-com.aspose.note.Loop-}
```
public void visitLoopEnd(Loop loop)
```


Bitir [Loop](../../com.aspose.note/loop) düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | [Loop](../../com.aspose.note/loop) düğümü. |

### visitLoopStart(Loop loop) {#visitLoopStart-com.aspose.note.Loop-}
```
public void visitLoopStart(Loop loop)
```


Başlat [Loop](../../com.aspose.note/loop) düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | [Loop](../../com.aspose.note/loop) düğümü. |

### visitOutlineElementEnd(OutlineElement outlineElement) {#visitOutlineElementEnd-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementEnd(OutlineElement outlineElement)
```


Bitir `OutlineElement` düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | `OutlineElement` düğümü. |

### visitOutlineElementStart(OutlineElement outlineElement) {#visitOutlineElementStart-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementStart(OutlineElement outlineElement)
```


Başlat `OutlineElement` düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | `OutlineElement` düğümü. |

### visitOutlineEnd(Outline outline) {#visitOutlineEnd-com.aspose.note.Outline-}
```
public void visitOutlineEnd(Outline outline)
```


Bitir `Outline` düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | `Outline` düğümü. |

### visitOutlineGroupEnd(OutlineGroup outlineGroup) {#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupEnd(OutlineGroup outlineGroup)
```


Bitir `OutlineGroup` düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | `OutlineGroup` düğümü. |

### visitOutlineGroupStart(OutlineGroup outlineGroup) {#visitOutlineGroupStart-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupStart(OutlineGroup outlineGroup)
```


Başlat `OutlineGroup` düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | `OutlineGroup` düğümü. |

### visitOutlineStart(Outline outline) {#visitOutlineStart-com.aspose.note.Outline-}
```
public void visitOutlineStart(Outline outline)
```


Başlat `Outline` düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | `Outline` düğümü. |

### visitPageEnd(Page page) {#visitPageEnd-com.aspose.note.Page-}
```
public void visitPageEnd(Page page)
```


Bitir `Page` düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | `Page` düğümü. |

### visitPageStart(Page page) {#visitPageStart-com.aspose.note.Page-}
```
public void visitPageStart(Page page)
```


Başlat `Page` düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | `Page` düğümü. |

### visitRichTextEnd(RichText richText) {#visitRichTextEnd-com.aspose.note.RichText-}
```
public void visitRichTextEnd(RichText richText)
```


Bitir `RichText` düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | `RichText` düğümü. |

### visitRichTextStart(RichText richText) {#visitRichTextStart-com.aspose.note.RichText-}
```
public void visitRichTextStart(RichText richText)
```


Başlat `RichText` düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | `RichText` düğümü. |

### visitTableCellEnd(TableCell tableCell) {#visitTableCellEnd-com.aspose.note.TableCell-}
```
public void visitTableCellEnd(TableCell tableCell)
```


Bitir `TableCell` düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | `TableCell` düğümü. |

### visitTableCellStart(TableCell tableCell) {#visitTableCellStart-com.aspose.note.TableCell-}
```
public void visitTableCellStart(TableCell tableCell)
```


Başlat `TableCell` düğümünü ziyaret etmeyi.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | `TableCell` düğümü. |

### visitTableEnd(Table table) {#visitTableEnd-com.aspose.note.Table-}
```
public void visitTableEnd(Table table)
```


`Table` düğümünü ziyaret etmeyi bitir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | `Table` düğümü. |

### visitTableRowEnd(TableRow tableRow) {#visitTableRowEnd-com.aspose.note.TableRow-}
```
public void visitTableRowEnd(TableRow tableRow)
```


`TableRow` düğümünü ziyaret etmeyi bitir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | `TableRow` düğümü. |

### visitTableRowStart(TableRow tableRow) {#visitTableRowStart-com.aspose.note.TableRow-}
```
public void visitTableRowStart(TableRow tableRow)
```


`TableRow` düğümünü ziyaret etmeye başla.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | `TableRow` düğümü. |

### visitTableStart(Table table) {#visitTableStart-com.aspose.note.Table-}
```
public void visitTableStart(Table table)
```


`Table` düğümünü ziyaret etmeye başla.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | `Table` düğümü. |

### visitTitleEnd(Title title) {#visitTitleEnd-com.aspose.note.Title-}
```
public void visitTitleEnd(Title title)
```


`Title` düğümünü ziyaret etmeyi bitir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | `Title` düğümü. |

### visitTitleStart(Title title) {#visitTitleStart-com.aspose.note.Title-}
```
public void visitTitleStart(Title title)
```


`Title` düğümünü ziyaret etmeye başla.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | `Title` düğümü. |

