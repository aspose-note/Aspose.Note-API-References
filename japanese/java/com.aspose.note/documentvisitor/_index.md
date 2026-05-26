---
title: "DocumentVisitor"
second_title: "Aspose.Note for Java API リファレンス"
description: "指定されたノードをルートとするサブツリーを反復処理するための抽象クラスです。"
type: docs
weight: 22
url: /ja/java/com.aspose.note/documentvisitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class DocumentVisitor
```

指定されたノードをルートとするサブツリーを反復処理するための抽象クラスです。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [DocumentVisitor()](#DocumentVisitor--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [visitAttachedFileEnd(AttachedFile attachedFile)](#visitAttachedFileEnd-com.aspose.note.AttachedFile-) | `AttachedFile` ノードの訪問を終了します。 |
| [visitAttachedFileStart(AttachedFile attachedFile)](#visitAttachedFileStart-com.aspose.note.AttachedFile-) | `AttachedFile` ノードの訪問を開始します。 |
| [visitDocumentEnd(Document document)](#visitDocumentEnd-com.aspose.note.Document-) | `Document` ノードの訪問を終了します。 |
| [visitDocumentStart(Document document)](#visitDocumentStart-com.aspose.note.Document-) | `Document` ノードの訪問を開始します。 |
| [visitImageEnd(Image image)](#visitImageEnd-com.aspose.note.Image-) | `Image` ノードの訪問を終了します。 |
| [visitImageStart(Image image)](#visitImageStart-com.aspose.note.Image-) | `Image` ノードの訪問を開始します。 |
| [visitInkDrawingEnd(InkDrawing inkDrawing)](#visitInkDrawingEnd-com.aspose.note.InkDrawing-) | [InkDrawing](../../com.aspose.note/inkdrawing) ノードの訪問を終了します。 |
| [visitInkDrawingStart(InkDrawing inkDrawing)](#visitInkDrawingStart-com.aspose.note.InkDrawing-) | [InkDrawing](../../com.aspose.note/inkdrawing) ノードの訪問を開始します。 |
| [visitInkParagraphEnd(InkParagraph inkParagraph)](#visitInkParagraphEnd-com.aspose.note.InkParagraph-) | [InkParagraph](../../com.aspose.note/inkparagraph) ノードの訪問を終了します。 |
| [visitInkParagraphStart(InkParagraph inkParagraph)](#visitInkParagraphStart-com.aspose.note.InkParagraph-) | [InkParagraph](../../com.aspose.note/inkparagraph) ノードの訪問を開始します。 |
| [visitInkWordEnd(InkWord inkWord)](#visitInkWordEnd-com.aspose.note.InkWord-) | [InkWord](../../com.aspose.note/inkword) ノードの訪問を終了します。 |
| [visitInkWordStart(InkWord inkWord)](#visitInkWordStart-com.aspose.note.InkWord-) | [InkWord](../../com.aspose.note/inkword) ノードの訪問を開始します。 |
| [visitLoopEnd(Loop loop)](#visitLoopEnd-com.aspose.note.Loop-) | [Loop](../../com.aspose.note/loop) ノードの訪問を終了します。 |
| [visitLoopStart(Loop loop)](#visitLoopStart-com.aspose.note.Loop-) | [Loop](../../com.aspose.note/loop) ノードの訪問を開始します。 |
| [visitOutlineElementEnd(OutlineElement outlineElement)](#visitOutlineElementEnd-com.aspose.note.OutlineElement-) | `OutlineElement` ノードの訪問を終了します。 |
| [visitOutlineElementStart(OutlineElement outlineElement)](#visitOutlineElementStart-com.aspose.note.OutlineElement-) | `OutlineElement` ノードの訪問を開始します。 |
| [visitOutlineEnd(Outline outline)](#visitOutlineEnd-com.aspose.note.Outline-) | `Outline` ノードの訪問を終了します。 |
| [visitOutlineGroupEnd(OutlineGroup outlineGroup)](#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-) | `OutlineGroup` ノードの訪問を終了します。 |
| [visitOutlineGroupStart(OutlineGroup outlineGroup)](#visitOutlineGroupStart-com.aspose.note.OutlineGroup-) | `OutlineGroup` ノードの訪問を開始します。 |
| [visitOutlineStart(Outline outline)](#visitOutlineStart-com.aspose.note.Outline-) | `Outline` ノードの訪問を開始します。 |
| [visitPageEnd(Page page)](#visitPageEnd-com.aspose.note.Page-) | `Page` ノードの訪問を終了します。 |
| [visitPageStart(Page page)](#visitPageStart-com.aspose.note.Page-) | `Page` ノードの訪問を開始します。 |
| [visitRichTextEnd(RichText richText)](#visitRichTextEnd-com.aspose.note.RichText-) | `RichText` ノードの訪問を終了します。 |
| [visitRichTextStart(RichText richText)](#visitRichTextStart-com.aspose.note.RichText-) | `RichText` ノードの訪問を開始します。 |
| [visitTableCellEnd(TableCell tableCell)](#visitTableCellEnd-com.aspose.note.TableCell-) | `TableCell` ノードの訪問を終了します。 |
| [visitTableCellStart(TableCell tableCell)](#visitTableCellStart-com.aspose.note.TableCell-) | `TableCell` ノードの訪問を開始します。 |
| [visitTableEnd(Table table)](#visitTableEnd-com.aspose.note.Table-) | `Table` ノードの訪問を終了します。 |
| [visitTableRowEnd(TableRow tableRow)](#visitTableRowEnd-com.aspose.note.TableRow-) | `TableRow` ノードの訪問を終了します。 |
| [visitTableRowStart(TableRow tableRow)](#visitTableRowStart-com.aspose.note.TableRow-) | `TableRow` ノードの訪問を開始します。 |
| [visitTableStart(Table table)](#visitTableStart-com.aspose.note.Table-) | `Table` ノードの訪問を開始します。 |
| [visitTitleEnd(Title title)](#visitTitleEnd-com.aspose.note.Title-) | `Title` ノードの訪問を終了します。 |
| [visitTitleStart(Title title)](#visitTitleStart-com.aspose.note.Title-) | `Title` ノードの訪問を開始します。 |
### DocumentVisitor() {#DocumentVisitor--}
```
public DocumentVisitor()
```


### visitAttachedFileEnd(AttachedFile attachedFile) {#visitAttachedFileEnd-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileEnd(AttachedFile attachedFile)
```


`AttachedFile` ノードの訪問を終了します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | `AttachedFile` ノードです。 |

### visitAttachedFileStart(AttachedFile attachedFile) {#visitAttachedFileStart-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileStart(AttachedFile attachedFile)
```


`AttachedFile` ノードの訪問を開始します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | `AttachedFile` ノードです。 |

### visitDocumentEnd(Document document) {#visitDocumentEnd-com.aspose.note.Document-}
```
public void visitDocumentEnd(Document document)
```


`Document` ノードの訪問を終了します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | `Document` ノードです。 |

### visitDocumentStart(Document document) {#visitDocumentStart-com.aspose.note.Document-}
```
public void visitDocumentStart(Document document)
```


`Document` ノードの訪問を開始します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | `Document` ノードです。 |

### visitImageEnd(Image image) {#visitImageEnd-com.aspose.note.Image-}
```
public void visitImageEnd(Image image)
```


`Image` ノードの訪問を終了します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | `Image` ノードです。 |

### visitImageStart(Image image) {#visitImageStart-com.aspose.note.Image-}
```
public void visitImageStart(Image image)
```


`Image` ノードの訪問を開始します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | `Image` ノードです。 |

### visitInkDrawingEnd(InkDrawing inkDrawing) {#visitInkDrawingEnd-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingEnd(InkDrawing inkDrawing)
```


[InkDrawing](../../com.aspose.note/inkdrawing) ノードの訪問を終了します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | この [InkDrawing](../../com.aspose.note/inkdrawing) ノードです。 |

### visitInkDrawingStart(InkDrawing inkDrawing) {#visitInkDrawingStart-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingStart(InkDrawing inkDrawing)
```


[InkDrawing](../../com.aspose.note/inkdrawing) ノードの訪問を開始します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | この [InkDrawing](../../com.aspose.note/inkdrawing) ノードです。 |

### visitInkParagraphEnd(InkParagraph inkParagraph) {#visitInkParagraphEnd-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphEnd(InkParagraph inkParagraph)
```


[InkParagraph](../../com.aspose.note/inkparagraph) ノードの訪問を終了します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | この [InkParagraph](../../com.aspose.note/inkparagraph) ノードです。 |

### visitInkParagraphStart(InkParagraph inkParagraph) {#visitInkParagraphStart-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphStart(InkParagraph inkParagraph)
```


[InkParagraph](../../com.aspose.note/inkparagraph) ノードの訪問を開始します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | この [InkParagraph](../../com.aspose.note/inkparagraph) ノードです。 |

### visitInkWordEnd(InkWord inkWord) {#visitInkWordEnd-com.aspose.note.InkWord-}
```
public void visitInkWordEnd(InkWord inkWord)
```


[InkWord](../../com.aspose.note/inkword) ノードの訪問を終了します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | この [InkWord](../../com.aspose.note/inkword) ノードです。 |

### visitInkWordStart(InkWord inkWord) {#visitInkWordStart-com.aspose.note.InkWord-}
```
public void visitInkWordStart(InkWord inkWord)
```


[InkWord](../../com.aspose.note/inkword) ノードの訪問を開始します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | この [InkWord](../../com.aspose.note/inkword) ノードです。 |

### visitLoopEnd(Loop loop) {#visitLoopEnd-com.aspose.note.Loop-}
```
public void visitLoopEnd(Loop loop)
```


[Loop](../../com.aspose.note/loop) ノードの訪問を終了します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | この [Loop](../../com.aspose.note/loop) ノードです。 |

### visitLoopStart(Loop loop) {#visitLoopStart-com.aspose.note.Loop-}
```
public void visitLoopStart(Loop loop)
```


[Loop](../../com.aspose.note/loop) ノードの訪問を開始します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | この [Loop](../../com.aspose.note/loop) ノードです。 |

### visitOutlineElementEnd(OutlineElement outlineElement) {#visitOutlineElementEnd-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementEnd(OutlineElement outlineElement)
```


`OutlineElement` ノードの訪問を終了します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | `OutlineElement` ノードです。 |

### visitOutlineElementStart(OutlineElement outlineElement) {#visitOutlineElementStart-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementStart(OutlineElement outlineElement)
```


`OutlineElement` ノードの訪問を開始します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | `OutlineElement` ノードです。 |

### visitOutlineEnd(Outline outline) {#visitOutlineEnd-com.aspose.note.Outline-}
```
public void visitOutlineEnd(Outline outline)
```


`Outline` ノードの訪問を終了します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | `Outline` ノードです。 |

### visitOutlineGroupEnd(OutlineGroup outlineGroup) {#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupEnd(OutlineGroup outlineGroup)
```


`OutlineGroup` ノードの訪問を終了します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | `OutlineGroup` ノードです。 |

### visitOutlineGroupStart(OutlineGroup outlineGroup) {#visitOutlineGroupStart-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupStart(OutlineGroup outlineGroup)
```


`OutlineGroup` ノードの訪問を開始します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | `OutlineGroup` ノードです。 |

### visitOutlineStart(Outline outline) {#visitOutlineStart-com.aspose.note.Outline-}
```
public void visitOutlineStart(Outline outline)
```


`Outline` ノードの訪問を開始します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | `Outline` ノードです。 |

### visitPageEnd(Page page) {#visitPageEnd-com.aspose.note.Page-}
```
public void visitPageEnd(Page page)
```


`Page` ノードの訪問を終了します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | `Page` ノードです。 |

### visitPageStart(Page page) {#visitPageStart-com.aspose.note.Page-}
```
public void visitPageStart(Page page)
```


`Page` ノードの訪問を開始します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | `Page` ノードです。 |

### visitRichTextEnd(RichText richText) {#visitRichTextEnd-com.aspose.note.RichText-}
```
public void visitRichTextEnd(RichText richText)
```


`RichText` ノードの訪問を終了します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | `RichText` ノードです。 |

### visitRichTextStart(RichText richText) {#visitRichTextStart-com.aspose.note.RichText-}
```
public void visitRichTextStart(RichText richText)
```


`RichText` ノードの訪問を開始します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | `RichText` ノードです。 |

### visitTableCellEnd(TableCell tableCell) {#visitTableCellEnd-com.aspose.note.TableCell-}
```
public void visitTableCellEnd(TableCell tableCell)
```


`TableCell` ノードの訪問を終了します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | `TableCell` ノードです。 |

### visitTableCellStart(TableCell tableCell) {#visitTableCellStart-com.aspose.note.TableCell-}
```
public void visitTableCellStart(TableCell tableCell)
```


`TableCell` ノードの訪問を開始します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | `TableCell` ノードです。 |

### visitTableEnd(Table table) {#visitTableEnd-com.aspose.note.Table-}
```
public void visitTableEnd(Table table)
```


`Table` ノードの訪問を終了します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | `Table` ノードです。 |

### visitTableRowEnd(TableRow tableRow) {#visitTableRowEnd-com.aspose.note.TableRow-}
```
public void visitTableRowEnd(TableRow tableRow)
```


`TableRow` ノードの訪問を終了します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | `TableRow` ノードです。 |

### visitTableRowStart(TableRow tableRow) {#visitTableRowStart-com.aspose.note.TableRow-}
```
public void visitTableRowStart(TableRow tableRow)
```


`TableRow` ノードの訪問を開始します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | `TableRow` ノードです。 |

### visitTableStart(Table table) {#visitTableStart-com.aspose.note.Table-}
```
public void visitTableStart(Table table)
```


`Table` ノードの訪問を開始します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | `Table` ノードです。 |

### visitTitleEnd(Title title) {#visitTitleEnd-com.aspose.note.Title-}
```
public void visitTitleEnd(Title title)
```


`Title` ノードの訪問を終了します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | `Title` ノードです。 |

### visitTitleStart(Title title) {#visitTitleStart-com.aspose.note.Title-}
```
public void visitTitleStart(Title title)
```


`Title` ノードの訪問を開始します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | `Title` ノードです。 |

