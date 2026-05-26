---
title: "DocumentVisitor"
second_title: "Справочник API Aspose.Note for Java"
description: "Абстрактный класс для итерации по поддереву с корнем в указанном узле."
type: docs
weight: 22
url: /ru/java/com.aspose.note/documentvisitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class DocumentVisitor
```

Абстрактный класс для итерации по поддереву с корнем в указанном узле.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [DocumentVisitor()](#DocumentVisitor--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [visitAttachedFileEnd(AttachedFile attachedFile)](#visitAttachedFileEnd-com.aspose.note.AttachedFile-) | Завершить посещение узла `AttachedFile`. |
| [visitAttachedFileStart(AttachedFile attachedFile)](#visitAttachedFileStart-com.aspose.note.AttachedFile-) | Начать посещение узла `AttachedFile`. |
| [visitDocumentEnd(Document document)](#visitDocumentEnd-com.aspose.note.Document-) | Завершить посещение узла `Document`. |
| [visitDocumentStart(Document document)](#visitDocumentStart-com.aspose.note.Document-) | Начать посещение узла `Document`. |
| [visitImageEnd(Image image)](#visitImageEnd-com.aspose.note.Image-) | Завершить посещение узла `Image`. |
| [visitImageStart(Image image)](#visitImageStart-com.aspose.note.Image-) | Начать посещение узла `Image`. |
| [visitInkDrawingEnd(InkDrawing inkDrawing)](#visitInkDrawingEnd-com.aspose.note.InkDrawing-) | Завершить посещение узла [InkDrawing](../../com.aspose.note/inkdrawing). |
| [visitInkDrawingStart(InkDrawing inkDrawing)](#visitInkDrawingStart-com.aspose.note.InkDrawing-) | Начать посещение узла [InkDrawing](../../com.aspose.note/inkdrawing). |
| [visitInkParagraphEnd(InkParagraph inkParagraph)](#visitInkParagraphEnd-com.aspose.note.InkParagraph-) | Завершить посещение узла [InkParagraph](../../com.aspose.note/inkparagraph). |
| [visitInkParagraphStart(InkParagraph inkParagraph)](#visitInkParagraphStart-com.aspose.note.InkParagraph-) | Начать посещение узла [InkParagraph](../../com.aspose.note/inkparagraph). |
| [visitInkWordEnd(InkWord inkWord)](#visitInkWordEnd-com.aspose.note.InkWord-) | Завершить посещение узла [InkWord](../../com.aspose.note/inkword). |
| [visitInkWordStart(InkWord inkWord)](#visitInkWordStart-com.aspose.note.InkWord-) | Начать посещение узла [InkWord](../../com.aspose.note/inkword). |
| [visitLoopEnd(Loop loop)](#visitLoopEnd-com.aspose.note.Loop-) | Завершить посещение узла [Loop](../../com.aspose.note/loop). |
| [visitLoopStart(Loop loop)](#visitLoopStart-com.aspose.note.Loop-) | Начать посещение узла [Loop](../../com.aspose.note/loop). |
| [visitOutlineElementEnd(OutlineElement outlineElement)](#visitOutlineElementEnd-com.aspose.note.OutlineElement-) | Завершить посещение узла `OutlineElement`. |
| [visitOutlineElementStart(OutlineElement outlineElement)](#visitOutlineElementStart-com.aspose.note.OutlineElement-) | Начать посещение узла `OutlineElement`. |
| [visitOutlineEnd(Outline outline)](#visitOutlineEnd-com.aspose.note.Outline-) | Завершить посещение узла `Outline`. |
| [visitOutlineGroupEnd(OutlineGroup outlineGroup)](#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-) | Завершить посещение узла `OutlineGroup`. |
| [visitOutlineGroupStart(OutlineGroup outlineGroup)](#visitOutlineGroupStart-com.aspose.note.OutlineGroup-) | Начать посещение узла `OutlineGroup`. |
| [visitOutlineStart(Outline outline)](#visitOutlineStart-com.aspose.note.Outline-) | Начать посещение узла `Outline`. |
| [visitPageEnd(Page page)](#visitPageEnd-com.aspose.note.Page-) | Завершить посещение узла `Page`. |
| [visitPageStart(Page page)](#visitPageStart-com.aspose.note.Page-) | Начать посещение узла `Page`. |
| [visitRichTextEnd(RichText richText)](#visitRichTextEnd-com.aspose.note.RichText-) | Завершить посещение узла `RichText`. |
| [visitRichTextStart(RichText richText)](#visitRichTextStart-com.aspose.note.RichText-) | Начать посещение узла `RichText`. |
| [visitTableCellEnd(TableCell tableCell)](#visitTableCellEnd-com.aspose.note.TableCell-) | Завершить посещение узла `TableCell`. |
| [visitTableCellStart(TableCell tableCell)](#visitTableCellStart-com.aspose.note.TableCell-) | Начать посещение узла `TableCell`. |
| [visitTableEnd(Table table)](#visitTableEnd-com.aspose.note.Table-) | Завершить посещение узла `Table`. |
| [visitTableRowEnd(TableRow tableRow)](#visitTableRowEnd-com.aspose.note.TableRow-) | Завершить посещение узла `TableRow`. |
| [visitTableRowStart(TableRow tableRow)](#visitTableRowStart-com.aspose.note.TableRow-) | Начать посещение узла `TableRow`. |
| [visitTableStart(Table table)](#visitTableStart-com.aspose.note.Table-) | Начать посещение узла `Table`. |
| [visitTitleEnd(Title title)](#visitTitleEnd-com.aspose.note.Title-) | Завершить посещение узла `Title`. |
| [visitTitleStart(Title title)](#visitTitleStart-com.aspose.note.Title-) | Начать посещение узла `Title`. |
### DocumentVisitor() {#DocumentVisitor--}
```
public DocumentVisitor()
```


### visitAttachedFileEnd(AttachedFile attachedFile) {#visitAttachedFileEnd-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileEnd(AttachedFile attachedFile)
```


Завершить посещение узла `AttachedFile`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | Узел `AttachedFile`. |

### visitAttachedFileStart(AttachedFile attachedFile) {#visitAttachedFileStart-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileStart(AttachedFile attachedFile)
```


Начать посещение узла `AttachedFile`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | Узел `AttachedFile`. |

### visitDocumentEnd(Document document) {#visitDocumentEnd-com.aspose.note.Document-}
```
public void visitDocumentEnd(Document document)
```


Завершить посещение узла `Document`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | Узел `Document`. |

### visitDocumentStart(Document document) {#visitDocumentStart-com.aspose.note.Document-}
```
public void visitDocumentStart(Document document)
```


Начать посещение узла `Document`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | Узел `Document`. |

### visitImageEnd(Image image) {#visitImageEnd-com.aspose.note.Image-}
```
public void visitImageEnd(Image image)
```


Завершить посещение узла `Image`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | Узел `Image`. |

### visitImageStart(Image image) {#visitImageStart-com.aspose.note.Image-}
```
public void visitImageStart(Image image)
```


Начать посещение узла `Image`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | Узел `Image`. |

### visitInkDrawingEnd(InkDrawing inkDrawing) {#visitInkDrawingEnd-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingEnd(InkDrawing inkDrawing)
```


Завершить посещение узла [InkDrawing](../../com.aspose.note/inkdrawing).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | Узел [InkDrawing](../../com.aspose.note/inkdrawing). |

### visitInkDrawingStart(InkDrawing inkDrawing) {#visitInkDrawingStart-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingStart(InkDrawing inkDrawing)
```


Начать посещение узла [InkDrawing](../../com.aspose.note/inkdrawing).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | Узел [InkDrawing](../../com.aspose.note/inkdrawing). |

### visitInkParagraphEnd(InkParagraph inkParagraph) {#visitInkParagraphEnd-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphEnd(InkParagraph inkParagraph)
```


Завершить посещение узла [InkParagraph](../../com.aspose.note/inkparagraph).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | Узел [InkParagraph](../../com.aspose.note/inkparagraph). |

### visitInkParagraphStart(InkParagraph inkParagraph) {#visitInkParagraphStart-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphStart(InkParagraph inkParagraph)
```


Начать посещение узла [InkParagraph](../../com.aspose.note/inkparagraph).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | Узел [InkParagraph](../../com.aspose.note/inkparagraph). |

### visitInkWordEnd(InkWord inkWord) {#visitInkWordEnd-com.aspose.note.InkWord-}
```
public void visitInkWordEnd(InkWord inkWord)
```


Завершить посещение узла [InkWord](../../com.aspose.note/inkword).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | Узел [InkWord](../../com.aspose.note/inkword). |

### visitInkWordStart(InkWord inkWord) {#visitInkWordStart-com.aspose.note.InkWord-}
```
public void visitInkWordStart(InkWord inkWord)
```


Начать посещение узла [InkWord](../../com.aspose.note/inkword).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | Узел [InkWord](../../com.aspose.note/inkword). |

### visitLoopEnd(Loop loop) {#visitLoopEnd-com.aspose.note.Loop-}
```
public void visitLoopEnd(Loop loop)
```


Завершить посещение узла [Loop](../../com.aspose.note/loop).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | Узел [Loop](../../com.aspose.note/loop). |

### visitLoopStart(Loop loop) {#visitLoopStart-com.aspose.note.Loop-}
```
public void visitLoopStart(Loop loop)
```


Начать посещение узла [Loop](../../com.aspose.note/loop).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | Узел [Loop](../../com.aspose.note/loop). |

### visitOutlineElementEnd(OutlineElement outlineElement) {#visitOutlineElementEnd-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementEnd(OutlineElement outlineElement)
```


Завершить посещение узла `OutlineElement`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | Узел `OutlineElement`. |

### visitOutlineElementStart(OutlineElement outlineElement) {#visitOutlineElementStart-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementStart(OutlineElement outlineElement)
```


Начать посещение узла `OutlineElement`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | Узел `OutlineElement`. |

### visitOutlineEnd(Outline outline) {#visitOutlineEnd-com.aspose.note.Outline-}
```
public void visitOutlineEnd(Outline outline)
```


Завершить посещение узла `Outline`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | Узел `Outline`. |

### visitOutlineGroupEnd(OutlineGroup outlineGroup) {#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupEnd(OutlineGroup outlineGroup)
```


Завершить посещение узла `OutlineGroup`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | Узел `OutlineGroup`. |

### visitOutlineGroupStart(OutlineGroup outlineGroup) {#visitOutlineGroupStart-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupStart(OutlineGroup outlineGroup)
```


Начать посещение узла `OutlineGroup`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | Узел `OutlineGroup`. |

### visitOutlineStart(Outline outline) {#visitOutlineStart-com.aspose.note.Outline-}
```
public void visitOutlineStart(Outline outline)
```


Начать посещение узла `Outline`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | Узел `Outline`. |

### visitPageEnd(Page page) {#visitPageEnd-com.aspose.note.Page-}
```
public void visitPageEnd(Page page)
```


Завершить посещение узла `Page`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Узел `Page`. |

### visitPageStart(Page page) {#visitPageStart-com.aspose.note.Page-}
```
public void visitPageStart(Page page)
```


Начать посещение узла `Page`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Узел `Page`. |

### visitRichTextEnd(RichText richText) {#visitRichTextEnd-com.aspose.note.RichText-}
```
public void visitRichTextEnd(RichText richText)
```


Завершить посещение узла `RichText`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | Узел `RichText`. |

### visitRichTextStart(RichText richText) {#visitRichTextStart-com.aspose.note.RichText-}
```
public void visitRichTextStart(RichText richText)
```


Начать посещение узла `RichText`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | Узел `RichText`. |

### visitTableCellEnd(TableCell tableCell) {#visitTableCellEnd-com.aspose.note.TableCell-}
```
public void visitTableCellEnd(TableCell tableCell)
```


Завершить посещение узла `TableCell`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | Узел `TableCell`. |

### visitTableCellStart(TableCell tableCell) {#visitTableCellStart-com.aspose.note.TableCell-}
```
public void visitTableCellStart(TableCell tableCell)
```


Начать посещение узла `TableCell`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | Узел `TableCell`. |

### visitTableEnd(Table table) {#visitTableEnd-com.aspose.note.Table-}
```
public void visitTableEnd(Table table)
```


Завершить посещение узла `Table`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | Узел `Table`. |

### visitTableRowEnd(TableRow tableRow) {#visitTableRowEnd-com.aspose.note.TableRow-}
```
public void visitTableRowEnd(TableRow tableRow)
```


Завершить посещение узла `TableRow`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | Узел `TableRow`. |

### visitTableRowStart(TableRow tableRow) {#visitTableRowStart-com.aspose.note.TableRow-}
```
public void visitTableRowStart(TableRow tableRow)
```


Начать посещение узла `TableRow`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | Узел `TableRow`. |

### visitTableStart(Table table) {#visitTableStart-com.aspose.note.Table-}
```
public void visitTableStart(Table table)
```


Начать посещение узла `Table`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | Узел `Table`. |

### visitTitleEnd(Title title) {#visitTitleEnd-com.aspose.note.Title-}
```
public void visitTitleEnd(Title title)
```


Завершить посещение узла `Title`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | Узел `Title`. |

### visitTitleStart(Title title) {#visitTitleStart-com.aspose.note.Title-}
```
public void visitTitleStart(Title title)
```


Начать посещение узла `Title`.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | Узел `Title`. |

