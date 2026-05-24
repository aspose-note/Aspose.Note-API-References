---
title: "DocumentVisitor"
second_title: "Aspose.Note for Java API 参考"
description: "用于在指定节点为根遍历子树的抽象类。"
type: docs
weight: 22
url: /zh/java/com.aspose.note/documentvisitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class DocumentVisitor
```

用于在指定节点为根遍历子树的抽象类。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [DocumentVisitor()](#DocumentVisitor--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [visitAttachedFileEnd(AttachedFile attachedFile)](#visitAttachedFileEnd-com.aspose.note.AttachedFile-) | 结束访问 `AttachedFile` 节点。 |
| [visitAttachedFileStart(AttachedFile attachedFile)](#visitAttachedFileStart-com.aspose.note.AttachedFile-) | 开始访问 `AttachedFile` 节点。 |
| [visitDocumentEnd(Document document)](#visitDocumentEnd-com.aspose.note.Document-) | 结束访问 `Document` 节点。 |
| [visitDocumentStart(Document document)](#visitDocumentStart-com.aspose.note.Document-) | 开始访问 `Document` 节点。 |
| [visitImageEnd(Image image)](#visitImageEnd-com.aspose.note.Image-) | 结束访问 `Image` 节点。 |
| [visitImageStart(Image image)](#visitImageStart-com.aspose.note.Image-) | 开始访问 `Image` 节点。 |
| [visitInkDrawingEnd(InkDrawing inkDrawing)](#visitInkDrawingEnd-com.aspose.note.InkDrawing-) | 结束访问 [InkDrawing](../../com.aspose.note/inkdrawing) 节点。 |
| [visitInkDrawingStart(InkDrawing inkDrawing)](#visitInkDrawingStart-com.aspose.note.InkDrawing-) | 开始访问 [InkDrawing](../../com.aspose.note/inkdrawing) 节点。 |
| [visitInkParagraphEnd(InkParagraph inkParagraph)](#visitInkParagraphEnd-com.aspose.note.InkParagraph-) | 结束访问 [InkParagraph](../../com.aspose.note/inkparagraph) 节点。 |
| [visitInkParagraphStart(InkParagraph inkParagraph)](#visitInkParagraphStart-com.aspose.note.InkParagraph-) | 开始访问 [InkParagraph](../../com.aspose.note/inkparagraph) 节点。 |
| [visitInkWordEnd(InkWord inkWord)](#visitInkWordEnd-com.aspose.note.InkWord-) | 结束访问 [InkWord](../../com.aspose.note/inkword) 节点。 |
| [visitInkWordStart(InkWord inkWord)](#visitInkWordStart-com.aspose.note.InkWord-) | 开始访问 [InkWord](../../com.aspose.note/inkword) 节点。 |
| [visitLoopEnd(Loop loop)](#visitLoopEnd-com.aspose.note.Loop-) | 结束访问 [Loop](../../com.aspose.note/loop) 节点。 |
| [visitLoopStart(Loop loop)](#visitLoopStart-com.aspose.note.Loop-) | 开始访问 [Loop](../../com.aspose.note/loop) 节点。 |
| [visitOutlineElementEnd(OutlineElement outlineElement)](#visitOutlineElementEnd-com.aspose.note.OutlineElement-) | 结束访问 `OutlineElement` 节点。 |
| [visitOutlineElementStart(OutlineElement outlineElement)](#visitOutlineElementStart-com.aspose.note.OutlineElement-) | 开始访问 `OutlineElement` 节点。 |
| [visitOutlineEnd(Outline outline)](#visitOutlineEnd-com.aspose.note.Outline-) | 结束访问 `Outline` 节点。 |
| [visitOutlineGroupEnd(OutlineGroup outlineGroup)](#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-) | 结束访问 `OutlineGroup` 节点。 |
| [visitOutlineGroupStart(OutlineGroup outlineGroup)](#visitOutlineGroupStart-com.aspose.note.OutlineGroup-) | 开始访问 `OutlineGroup` 节点。 |
| [visitOutlineStart(Outline outline)](#visitOutlineStart-com.aspose.note.Outline-) | 开始访问 `Outline` 节点。 |
| [visitPageEnd(Page page)](#visitPageEnd-com.aspose.note.Page-) | 结束访问 `Page` 节点。 |
| [visitPageStart(Page page)](#visitPageStart-com.aspose.note.Page-) | 开始访问 `Page` 节点。 |
| [visitRichTextEnd(RichText richText)](#visitRichTextEnd-com.aspose.note.RichText-) | 结束访问 `RichText` 节点。 |
| [visitRichTextStart(RichText richText)](#visitRichTextStart-com.aspose.note.RichText-) | 开始访问 `RichText` 节点。 |
| [visitTableCellEnd(TableCell tableCell)](#visitTableCellEnd-com.aspose.note.TableCell-) | 结束访问 `TableCell` 节点。 |
| [visitTableCellStart(TableCell tableCell)](#visitTableCellStart-com.aspose.note.TableCell-) | 开始访问 `TableCell` 节点。 |
| [visitTableEnd(Table table)](#visitTableEnd-com.aspose.note.Table-) | 结束访问 `Table` 节点。 |
| [visitTableRowEnd(TableRow tableRow)](#visitTableRowEnd-com.aspose.note.TableRow-) | 结束访问 `TableRow` 节点。 |
| [visitTableRowStart(TableRow tableRow)](#visitTableRowStart-com.aspose.note.TableRow-) | 开始访问 `TableRow` 节点。 |
| [visitTableStart(Table table)](#visitTableStart-com.aspose.note.Table-) | 开始访问 `Table` 节点。 |
| [visitTitleEnd(Title title)](#visitTitleEnd-com.aspose.note.Title-) | 结束访问 `Title` 节点。 |
| [visitTitleStart(Title title)](#visitTitleStart-com.aspose.note.Title-) | 开始访问 `Title` 节点。 |
### DocumentVisitor() {#DocumentVisitor--}
```
public DocumentVisitor()
```


### visitAttachedFileEnd(AttachedFile attachedFile) {#visitAttachedFileEnd-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileEnd(AttachedFile attachedFile)
```


结束访问 `AttachedFile` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | 该 `AttachedFile` 节点。 |

### visitAttachedFileStart(AttachedFile attachedFile) {#visitAttachedFileStart-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileStart(AttachedFile attachedFile)
```


开始访问 `AttachedFile` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | 该 `AttachedFile` 节点。 |

### visitDocumentEnd(Document document) {#visitDocumentEnd-com.aspose.note.Document-}
```
public void visitDocumentEnd(Document document)
```


结束访问 `Document` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | 该 `Document` 节点。 |

### visitDocumentStart(Document document) {#visitDocumentStart-com.aspose.note.Document-}
```
public void visitDocumentStart(Document document)
```


开始访问 `Document` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | 该 `Document` 节点。 |

### visitImageEnd(Image image) {#visitImageEnd-com.aspose.note.Image-}
```
public void visitImageEnd(Image image)
```


结束访问 `Image` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | 该 `Image` 节点。 |

### visitImageStart(Image image) {#visitImageStart-com.aspose.note.Image-}
```
public void visitImageStart(Image image)
```


开始访问 `Image` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | 该 `Image` 节点。 |

### visitInkDrawingEnd(InkDrawing inkDrawing) {#visitInkDrawingEnd-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingEnd(InkDrawing inkDrawing)
```


结束访问 [InkDrawing](../../com.aspose.note/inkdrawing) 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | 该 [InkDrawing](../../com.aspose.note/inkdrawing) 节点。 |

### visitInkDrawingStart(InkDrawing inkDrawing) {#visitInkDrawingStart-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingStart(InkDrawing inkDrawing)
```


开始访问 [InkDrawing](../../com.aspose.note/inkdrawing) 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | 该 [InkDrawing](../../com.aspose.note/inkdrawing) 节点。 |

### visitInkParagraphEnd(InkParagraph inkParagraph) {#visitInkParagraphEnd-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphEnd(InkParagraph inkParagraph)
```


结束访问 [InkParagraph](../../com.aspose.note/inkparagraph) 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | 该 [InkParagraph](../../com.aspose.note/inkparagraph) 节点。 |

### visitInkParagraphStart(InkParagraph inkParagraph) {#visitInkParagraphStart-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphStart(InkParagraph inkParagraph)
```


开始访问 [InkParagraph](../../com.aspose.note/inkparagraph) 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | 该 [InkParagraph](../../com.aspose.note/inkparagraph) 节点。 |

### visitInkWordEnd(InkWord inkWord) {#visitInkWordEnd-com.aspose.note.InkWord-}
```
public void visitInkWordEnd(InkWord inkWord)
```


结束访问 [InkWord](../../com.aspose.note/inkword) 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | 该 [InkWord](../../com.aspose.note/inkword) 节点。 |

### visitInkWordStart(InkWord inkWord) {#visitInkWordStart-com.aspose.note.InkWord-}
```
public void visitInkWordStart(InkWord inkWord)
```


开始访问 [InkWord](../../com.aspose.note/inkword) 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | 该 [InkWord](../../com.aspose.note/inkword) 节点。 |

### visitLoopEnd(Loop loop) {#visitLoopEnd-com.aspose.note.Loop-}
```
public void visitLoopEnd(Loop loop)
```


结束访问 [Loop](../../com.aspose.note/loop) 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | 该 [Loop](../../com.aspose.note/loop) 节点。 |

### visitLoopStart(Loop loop) {#visitLoopStart-com.aspose.note.Loop-}
```
public void visitLoopStart(Loop loop)
```


开始访问 [Loop](../../com.aspose.note/loop) 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | 该 [Loop](../../com.aspose.note/loop) 节点。 |

### visitOutlineElementEnd(OutlineElement outlineElement) {#visitOutlineElementEnd-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementEnd(OutlineElement outlineElement)
```


结束访问 `OutlineElement` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | 该 `OutlineElement` 节点。 |

### visitOutlineElementStart(OutlineElement outlineElement) {#visitOutlineElementStart-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementStart(OutlineElement outlineElement)
```


开始访问 `OutlineElement` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | 该 `OutlineElement` 节点。 |

### visitOutlineEnd(Outline outline) {#visitOutlineEnd-com.aspose.note.Outline-}
```
public void visitOutlineEnd(Outline outline)
```


结束访问 `Outline` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | 该 `Outline` 节点。 |

### visitOutlineGroupEnd(OutlineGroup outlineGroup) {#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupEnd(OutlineGroup outlineGroup)
```


结束访问 `OutlineGroup` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | 该 `OutlineGroup` 节点。 |

### visitOutlineGroupStart(OutlineGroup outlineGroup) {#visitOutlineGroupStart-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupStart(OutlineGroup outlineGroup)
```


开始访问 `OutlineGroup` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | 该 `OutlineGroup` 节点。 |

### visitOutlineStart(Outline outline) {#visitOutlineStart-com.aspose.note.Outline-}
```
public void visitOutlineStart(Outline outline)
```


开始访问 `Outline` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | 该 `Outline` 节点。 |

### visitPageEnd(Page page) {#visitPageEnd-com.aspose.note.Page-}
```
public void visitPageEnd(Page page)
```


结束访问 `Page` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | 该 `Page` 节点。 |

### visitPageStart(Page page) {#visitPageStart-com.aspose.note.Page-}
```
public void visitPageStart(Page page)
```


开始访问 `Page` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | 该 `Page` 节点。 |

### visitRichTextEnd(RichText richText) {#visitRichTextEnd-com.aspose.note.RichText-}
```
public void visitRichTextEnd(RichText richText)
```


结束访问 `RichText` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | 该 `RichText` 节点。 |

### visitRichTextStart(RichText richText) {#visitRichTextStart-com.aspose.note.RichText-}
```
public void visitRichTextStart(RichText richText)
```


开始访问 `RichText` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | 该 `RichText` 节点。 |

### visitTableCellEnd(TableCell tableCell) {#visitTableCellEnd-com.aspose.note.TableCell-}
```
public void visitTableCellEnd(TableCell tableCell)
```


结束访问 `TableCell` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | 该 `TableCell` 节点。 |

### visitTableCellStart(TableCell tableCell) {#visitTableCellStart-com.aspose.note.TableCell-}
```
public void visitTableCellStart(TableCell tableCell)
```


开始访问 `TableCell` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | 该 `TableCell` 节点。 |

### visitTableEnd(Table table) {#visitTableEnd-com.aspose.note.Table-}
```
public void visitTableEnd(Table table)
```


结束访问 `Table` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | 该 `Table` 节点。 |

### visitTableRowEnd(TableRow tableRow) {#visitTableRowEnd-com.aspose.note.TableRow-}
```
public void visitTableRowEnd(TableRow tableRow)
```


结束访问 `TableRow` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | 该 `TableRow` 节点。 |

### visitTableRowStart(TableRow tableRow) {#visitTableRowStart-com.aspose.note.TableRow-}
```
public void visitTableRowStart(TableRow tableRow)
```


开始访问 `TableRow` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | 该 `TableRow` 节点。 |

### visitTableStart(Table table) {#visitTableStart-com.aspose.note.Table-}
```
public void visitTableStart(Table table)
```


开始访问 `Table` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | 该 `Table` 节点。 |

### visitTitleEnd(Title title) {#visitTitleEnd-com.aspose.note.Title-}
```
public void visitTitleEnd(Title title)
```


结束访问 `Title` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | 该 `Title` 节点。 |

### visitTitleStart(Title title) {#visitTitleStart-com.aspose.note.Title-}
```
public void visitTitleStart(Title title)
```


开始访问 `Title` 节点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | 该 `Title` 节点。 |

