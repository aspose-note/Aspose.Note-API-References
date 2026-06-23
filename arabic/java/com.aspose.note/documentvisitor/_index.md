---
title: "DocumentVisitor"
second_title: "مرجع Aspose.Note لـ Java API"
description: "الفئة المجردة للتنقل عبر الشجرة الفرعية بجذر عند العقدة المحددة."
type: docs
weight: 22
url: /ar/java/com.aspose.note/documentvisitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class DocumentVisitor
```

الفئة المجردة للتنقل عبر الشجرة الفرعية بجذر عند العقدة المحددة.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [DocumentVisitor()](#DocumentVisitor--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [visitAttachedFileEnd(AttachedFile attachedFile)](#visitAttachedFileEnd-com.aspose.note.AttachedFile-) | انتهاء زيارة العقدة `AttachedFile`. |
| [visitAttachedFileStart(AttachedFile attachedFile)](#visitAttachedFileStart-com.aspose.note.AttachedFile-) | ابدأ بزيارة عقدة `AttachedFile`. |
| [visitDocumentEnd(Document document)](#visitDocumentEnd-com.aspose.note.Document-) | انتهى من زيارة عقدة `Document`. |
| [visitDocumentStart(Document document)](#visitDocumentStart-com.aspose.note.Document-) | ابدأ بزيارة عقدة `Document`. |
| [visitImageEnd(Image image)](#visitImageEnd-com.aspose.note.Image-) | انتهى من زيارة عقدة `Image`. |
| [visitImageStart(Image image)](#visitImageStart-com.aspose.note.Image-) | ابدأ بزيارة عقدة `Image`. |
| [visitInkDrawingEnd(InkDrawing inkDrawing)](#visitInkDrawingEnd-com.aspose.note.InkDrawing-) | انتهى من زيارة عقدة [InkDrawing](../../com.aspose.note/inkdrawing). |
| [visitInkDrawingStart(InkDrawing inkDrawing)](#visitInkDrawingStart-com.aspose.note.InkDrawing-) | ابدأ بزيارة عقدة [InkDrawing](../../com.aspose.note/inkdrawing). |
| [visitInkParagraphEnd(InkParagraph inkParagraph)](#visitInkParagraphEnd-com.aspose.note.InkParagraph-) | انتهى من زيارة عقدة [InkParagraph](../../com.aspose.note/inkparagraph). |
| [visitInkParagraphStart(InkParagraph inkParagraph)](#visitInkParagraphStart-com.aspose.note.InkParagraph-) | ابدأ بزيارة عقدة [InkParagraph](../../com.aspose.note/inkparagraph). |
| [visitInkWordEnd(InkWord inkWord)](#visitInkWordEnd-com.aspose.note.InkWord-) | انتهى من زيارة عقدة [InkWord](../../com.aspose.note/inkword). |
| [visitInkWordStart(InkWord inkWord)](#visitInkWordStart-com.aspose.note.InkWord-) | ابدأ بزيارة عقدة [InkWord](../../com.aspose.note/inkword). |
| [visitLoopEnd(Loop loop)](#visitLoopEnd-com.aspose.note.Loop-) | انتهى من زيارة عقدة [Loop](../../com.aspose.note/loop). |
| [visitLoopStart(Loop loop)](#visitLoopStart-com.aspose.note.Loop-) | ابدأ بزيارة عقدة [Loop](../../com.aspose.note/loop). |
| [visitOutlineElementEnd(OutlineElement outlineElement)](#visitOutlineElementEnd-com.aspose.note.OutlineElement-) | انتهى من زيارة عقدة `OutlineElement`. |
| [visitOutlineElementStart(OutlineElement outlineElement)](#visitOutlineElementStart-com.aspose.note.OutlineElement-) | ابدأ بزيارة عقدة `OutlineElement`. |
| [visitOutlineEnd(Outline outline)](#visitOutlineEnd-com.aspose.note.Outline-) | انتهى من زيارة عقدة `Outline`. |
| [visitOutlineGroupEnd(OutlineGroup outlineGroup)](#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-) | انتهى من زيارة عقدة `OutlineGroup`. |
| [visitOutlineGroupStart(OutlineGroup outlineGroup)](#visitOutlineGroupStart-com.aspose.note.OutlineGroup-) | ابدأ بزيارة عقدة `OutlineGroup`. |
| [visitOutlineStart(Outline outline)](#visitOutlineStart-com.aspose.note.Outline-) | ابدأ بزيارة عقدة `Outline`. |
| [visitPageEnd(Page page)](#visitPageEnd-com.aspose.note.Page-) | انتهى من زيارة عقدة `Page`. |
| [visitPageStart(Page page)](#visitPageStart-com.aspose.note.Page-) | ابدأ بزيارة عقدة `Page`. |
| [visitRichTextEnd(RichText richText)](#visitRichTextEnd-com.aspose.note.RichText-) | انتهى من زيارة عقدة `RichText`. |
| [visitRichTextStart(RichText richText)](#visitRichTextStart-com.aspose.note.RichText-) | ابدأ بزيارة عقدة `RichText`. |
| [visitTableCellEnd(TableCell tableCell)](#visitTableCellEnd-com.aspose.note.TableCell-) | انتهى من زيارة عقدة `TableCell`. |
| [visitTableCellStart(TableCell tableCell)](#visitTableCellStart-com.aspose.note.TableCell-) | ابدأ بزيارة عقدة `TableCell`. |
| [visitTableEnd(Table table)](#visitTableEnd-com.aspose.note.Table-) | انتهاء زيارة عقدة `Table`. |
| [visitTableRowEnd(TableRow tableRow)](#visitTableRowEnd-com.aspose.note.TableRow-) | انتهاء زيارة عقدة `TableRow`. |
| [visitTableRowStart(TableRow tableRow)](#visitTableRowStart-com.aspose.note.TableRow-) | بدء زيارة عقدة `TableRow`. |
| [visitTableStart(Table table)](#visitTableStart-com.aspose.note.Table-) | بدء زيارة عقدة `Table`. |
| [visitTitleEnd(Title title)](#visitTitleEnd-com.aspose.note.Title-) | انتهاء زيارة عقدة `Title`. |
| [visitTitleStart(Title title)](#visitTitleStart-com.aspose.note.Title-) | بدء زيارة عقدة `Title`. |
### DocumentVisitor() {#DocumentVisitor--}
```
public DocumentVisitor()
```


### visitAttachedFileEnd(AttachedFile attachedFile) {#visitAttachedFileEnd-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileEnd(AttachedFile attachedFile)
```


انتهاء زيارة العقدة `AttachedFile`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | العقدة `AttachedFile`. |

### visitAttachedFileStart(AttachedFile attachedFile) {#visitAttachedFileStart-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileStart(AttachedFile attachedFile)
```


ابدأ بزيارة عقدة `AttachedFile`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | العقدة `AttachedFile`. |

### visitDocumentEnd(Document document) {#visitDocumentEnd-com.aspose.note.Document-}
```
public void visitDocumentEnd(Document document)
```


انتهى من زيارة عقدة `Document`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | العقدة `Document`. |

### visitDocumentStart(Document document) {#visitDocumentStart-com.aspose.note.Document-}
```
public void visitDocumentStart(Document document)
```


ابدأ بزيارة عقدة `Document`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | العقدة `Document`. |

### visitImageEnd(Image image) {#visitImageEnd-com.aspose.note.Image-}
```
public void visitImageEnd(Image image)
```


انتهى من زيارة عقدة `Image`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | العقدة `Image`. |

### visitImageStart(Image image) {#visitImageStart-com.aspose.note.Image-}
```
public void visitImageStart(Image image)
```


ابدأ بزيارة عقدة `Image`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | العقدة `Image`. |

### visitInkDrawingEnd(InkDrawing inkDrawing) {#visitInkDrawingEnd-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingEnd(InkDrawing inkDrawing)
```


انتهى من زيارة عقدة [InkDrawing](../../com.aspose.note/inkdrawing).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | العقدة [InkDrawing](../../com.aspose.note/inkdrawing). |

### visitInkDrawingStart(InkDrawing inkDrawing) {#visitInkDrawingStart-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingStart(InkDrawing inkDrawing)
```


ابدأ بزيارة عقدة [InkDrawing](../../com.aspose.note/inkdrawing).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | العقدة [InkDrawing](../../com.aspose.note/inkdrawing). |

### visitInkParagraphEnd(InkParagraph inkParagraph) {#visitInkParagraphEnd-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphEnd(InkParagraph inkParagraph)
```


انتهى من زيارة عقدة [InkParagraph](../../com.aspose.note/inkparagraph).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | العقدة [InkParagraph](../../com.aspose.note/inkparagraph). |

### visitInkParagraphStart(InkParagraph inkParagraph) {#visitInkParagraphStart-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphStart(InkParagraph inkParagraph)
```


ابدأ بزيارة عقدة [InkParagraph](../../com.aspose.note/inkparagraph).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | العقدة [InkParagraph](../../com.aspose.note/inkparagraph). |

### visitInkWordEnd(InkWord inkWord) {#visitInkWordEnd-com.aspose.note.InkWord-}
```
public void visitInkWordEnd(InkWord inkWord)
```


انتهى من زيارة عقدة [InkWord](../../com.aspose.note/inkword).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | العقدة [InkWord](../../com.aspose.note/inkword). |

### visitInkWordStart(InkWord inkWord) {#visitInkWordStart-com.aspose.note.InkWord-}
```
public void visitInkWordStart(InkWord inkWord)
```


ابدأ بزيارة عقدة [InkWord](../../com.aspose.note/inkword).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | العقدة [InkWord](../../com.aspose.note/inkword). |

### visitLoopEnd(Loop loop) {#visitLoopEnd-com.aspose.note.Loop-}
```
public void visitLoopEnd(Loop loop)
```


انتهى من زيارة عقدة [Loop](../../com.aspose.note/loop).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | العقدة [Loop](../../com.aspose.note/loop). |

### visitLoopStart(Loop loop) {#visitLoopStart-com.aspose.note.Loop-}
```
public void visitLoopStart(Loop loop)
```


ابدأ بزيارة عقدة [Loop](../../com.aspose.note/loop).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | العقدة [Loop](../../com.aspose.note/loop). |

### visitOutlineElementEnd(OutlineElement outlineElement) {#visitOutlineElementEnd-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementEnd(OutlineElement outlineElement)
```


انتهى من زيارة عقدة `OutlineElement`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | العقدة `OutlineElement`. |

### visitOutlineElementStart(OutlineElement outlineElement) {#visitOutlineElementStart-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementStart(OutlineElement outlineElement)
```


ابدأ بزيارة عقدة `OutlineElement`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | العقدة `OutlineElement`. |

### visitOutlineEnd(Outline outline) {#visitOutlineEnd-com.aspose.note.Outline-}
```
public void visitOutlineEnd(Outline outline)
```


انتهى من زيارة عقدة `Outline`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | العقدة `Outline`. |

### visitOutlineGroupEnd(OutlineGroup outlineGroup) {#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupEnd(OutlineGroup outlineGroup)
```


انتهى من زيارة عقدة `OutlineGroup`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | العقدة `OutlineGroup`. |

### visitOutlineGroupStart(OutlineGroup outlineGroup) {#visitOutlineGroupStart-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupStart(OutlineGroup outlineGroup)
```


ابدأ بزيارة عقدة `OutlineGroup`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | العقدة `OutlineGroup`. |

### visitOutlineStart(Outline outline) {#visitOutlineStart-com.aspose.note.Outline-}
```
public void visitOutlineStart(Outline outline)
```


ابدأ بزيارة عقدة `Outline`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | العقدة `Outline`. |

### visitPageEnd(Page page) {#visitPageEnd-com.aspose.note.Page-}
```
public void visitPageEnd(Page page)
```


انتهى من زيارة عقدة `Page`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | العقدة `Page`. |

### visitPageStart(Page page) {#visitPageStart-com.aspose.note.Page-}
```
public void visitPageStart(Page page)
```


ابدأ بزيارة عقدة `Page`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | العقدة `Page`. |

### visitRichTextEnd(RichText richText) {#visitRichTextEnd-com.aspose.note.RichText-}
```
public void visitRichTextEnd(RichText richText)
```


انتهى من زيارة عقدة `RichText`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | العقدة `RichText`. |

### visitRichTextStart(RichText richText) {#visitRichTextStart-com.aspose.note.RichText-}
```
public void visitRichTextStart(RichText richText)
```


ابدأ بزيارة عقدة `RichText`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | العقدة `RichText`. |

### visitTableCellEnd(TableCell tableCell) {#visitTableCellEnd-com.aspose.note.TableCell-}
```
public void visitTableCellEnd(TableCell tableCell)
```


انتهى من زيارة عقدة `TableCell`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | العقدة `TableCell`. |

### visitTableCellStart(TableCell tableCell) {#visitTableCellStart-com.aspose.note.TableCell-}
```
public void visitTableCellStart(TableCell tableCell)
```


ابدأ بزيارة عقدة `TableCell`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | العقدة `TableCell`. |

### visitTableEnd(Table table) {#visitTableEnd-com.aspose.note.Table-}
```
public void visitTableEnd(Table table)
```


انتهاء زيارة عقدة `Table`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | العقدة `Table`. |

### visitTableRowEnd(TableRow tableRow) {#visitTableRowEnd-com.aspose.note.TableRow-}
```
public void visitTableRowEnd(TableRow tableRow)
```


انتهاء زيارة عقدة `TableRow`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | العقدة `TableRow`. |

### visitTableRowStart(TableRow tableRow) {#visitTableRowStart-com.aspose.note.TableRow-}
```
public void visitTableRowStart(TableRow tableRow)
```


بدء زيارة عقدة `TableRow`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | العقدة `TableRow`. |

### visitTableStart(Table table) {#visitTableStart-com.aspose.note.Table-}
```
public void visitTableStart(Table table)
```


بدء زيارة عقدة `Table`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | العقدة `Table`. |

### visitTitleEnd(Title title) {#visitTitleEnd-com.aspose.note.Title-}
```
public void visitTitleEnd(Title title)
```


انتهاء زيارة عقدة `Title`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | الع العقدة `Title`. |

### visitTitleStart(Title title) {#visitTitleStart-com.aspose.note.Title-}
```
public void visitTitleStart(Title title)
```


بدء زيارة عقدة `Title`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | الع العقدة `Title`. |

