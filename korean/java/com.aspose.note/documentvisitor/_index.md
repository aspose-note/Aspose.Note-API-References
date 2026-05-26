---
title: "DocumentVisitor"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "지정된 노드를 루트로 하는 서브트리를 순회하기 위한 추상 클래스입니다."
type: docs
weight: 22
url: /ko/java/com.aspose.note/documentvisitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class DocumentVisitor
```

지정된 노드를 루트로 하는 서브트리를 순회하기 위한 추상 클래스입니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [DocumentVisitor()](#DocumentVisitor--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [visitAttachedFileEnd(AttachedFile attachedFile)](#visitAttachedFileEnd-com.aspose.note.AttachedFile-) | `AttachedFile` 노드 방문을 종료합니다. |
| [visitAttachedFileStart(AttachedFile attachedFile)](#visitAttachedFileStart-com.aspose.note.AttachedFile-) | `AttachedFile` 노드 방문을 시작합니다. |
| [visitDocumentEnd(Document document)](#visitDocumentEnd-com.aspose.note.Document-) | `Document` 노드 방문을 종료합니다. |
| [visitDocumentStart(Document document)](#visitDocumentStart-com.aspose.note.Document-) | `Document` 노드 방문을 시작합니다. |
| [visitImageEnd(Image image)](#visitImageEnd-com.aspose.note.Image-) | `Image` 노드 방문을 종료합니다. |
| [visitImageStart(Image image)](#visitImageStart-com.aspose.note.Image-) | `Image` 노드 방문을 시작합니다. |
| [visitInkDrawingEnd(InkDrawing inkDrawing)](#visitInkDrawingEnd-com.aspose.note.InkDrawing-) | [InkDrawing](../../com.aspose.note/inkdrawing) 노드 방문을 종료합니다. |
| [visitInkDrawingStart(InkDrawing inkDrawing)](#visitInkDrawingStart-com.aspose.note.InkDrawing-) | [InkDrawing](../../com.aspose.note/inkdrawing) 노드 방문을 시작합니다. |
| [visitInkParagraphEnd(InkParagraph inkParagraph)](#visitInkParagraphEnd-com.aspose.note.InkParagraph-) | [InkParagraph](../../com.aspose.note/inkparagraph) 노드 방문을 종료합니다. |
| [visitInkParagraphStart(InkParagraph inkParagraph)](#visitInkParagraphStart-com.aspose.note.InkParagraph-) | [InkParagraph](../../com.aspose.note/inkparagraph) 노드 방문을 시작합니다. |
| [visitInkWordEnd(InkWord inkWord)](#visitInkWordEnd-com.aspose.note.InkWord-) | [InkWord](../../com.aspose.note/inkword) 노드 방문을 종료합니다. |
| [visitInkWordStart(InkWord inkWord)](#visitInkWordStart-com.aspose.note.InkWord-) | [InkWord](../../com.aspose.note/inkword) 노드 방문을 시작합니다. |
| [visitLoopEnd(Loop loop)](#visitLoopEnd-com.aspose.note.Loop-) | [Loop](../../com.aspose.note/loop) 노드 방문을 종료합니다. |
| [visitLoopStart(Loop loop)](#visitLoopStart-com.aspose.note.Loop-) | [Loop](../../com.aspose.note/loop) 노드 방문을 시작합니다. |
| [visitOutlineElementEnd(OutlineElement outlineElement)](#visitOutlineElementEnd-com.aspose.note.OutlineElement-) | `OutlineElement` 노드 방문을 종료합니다. |
| [visitOutlineElementStart(OutlineElement outlineElement)](#visitOutlineElementStart-com.aspose.note.OutlineElement-) | `OutlineElement` 노드 방문을 시작합니다. |
| [visitOutlineEnd(Outline outline)](#visitOutlineEnd-com.aspose.note.Outline-) | `Outline` 노드 방문을 종료합니다. |
| [visitOutlineGroupEnd(OutlineGroup outlineGroup)](#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-) | `OutlineGroup` 노드 방문을 종료합니다. |
| [visitOutlineGroupStart(OutlineGroup outlineGroup)](#visitOutlineGroupStart-com.aspose.note.OutlineGroup-) | `OutlineGroup` 노드 방문을 시작합니다. |
| [visitOutlineStart(Outline outline)](#visitOutlineStart-com.aspose.note.Outline-) | `Outline` 노드 방문을 시작합니다. |
| [visitPageEnd(Page page)](#visitPageEnd-com.aspose.note.Page-) | `Page` 노드 방문을 종료합니다. |
| [visitPageStart(Page page)](#visitPageStart-com.aspose.note.Page-) | `Page` 노드 방문을 시작합니다. |
| [visitRichTextEnd(RichText richText)](#visitRichTextEnd-com.aspose.note.RichText-) | `RichText` 노드 방문을 종료합니다. |
| [visitRichTextStart(RichText richText)](#visitRichTextStart-com.aspose.note.RichText-) | `RichText` 노드 방문을 시작합니다. |
| [visitTableCellEnd(TableCell tableCell)](#visitTableCellEnd-com.aspose.note.TableCell-) | `TableCell` 노드 방문을 종료합니다. |
| [visitTableCellStart(TableCell tableCell)](#visitTableCellStart-com.aspose.note.TableCell-) | `TableCell` 노드 방문을 시작합니다. |
| [visitTableEnd(Table table)](#visitTableEnd-com.aspose.note.Table-) | `Table` 노드 방문을 종료합니다. |
| [visitTableRowEnd(TableRow tableRow)](#visitTableRowEnd-com.aspose.note.TableRow-) | `TableRow` 노드 방문을 종료합니다. |
| [visitTableRowStart(TableRow tableRow)](#visitTableRowStart-com.aspose.note.TableRow-) | `TableRow` 노드 방문을 시작합니다. |
| [visitTableStart(Table table)](#visitTableStart-com.aspose.note.Table-) | `Table` 노드 방문을 시작합니다. |
| [visitTitleEnd(Title title)](#visitTitleEnd-com.aspose.note.Title-) | `Title` 노드 방문을 종료합니다. |
| [visitTitleStart(Title title)](#visitTitleStart-com.aspose.note.Title-) | `Title` 노드 방문을 시작합니다. |
### DocumentVisitor() {#DocumentVisitor--}
```
public DocumentVisitor()
```


### visitAttachedFileEnd(AttachedFile attachedFile) {#visitAttachedFileEnd-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileEnd(AttachedFile attachedFile)
```


`AttachedFile` 노드 방문을 종료합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | `AttachedFile` 노드. |

### visitAttachedFileStart(AttachedFile attachedFile) {#visitAttachedFileStart-com.aspose.note.AttachedFile-}
```
public void visitAttachedFileStart(AttachedFile attachedFile)
```


`AttachedFile` 노드 방문을 시작합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| attachedFile | [AttachedFile](../../com.aspose.note/attachedfile) | `AttachedFile` 노드. |

### visitDocumentEnd(Document document) {#visitDocumentEnd-com.aspose.note.Document-}
```
public void visitDocumentEnd(Document document)
```


`Document` 노드 방문을 종료합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | `Document` 노드. |

### visitDocumentStart(Document document) {#visitDocumentStart-com.aspose.note.Document-}
```
public void visitDocumentStart(Document document)
```


`Document` 노드 방문을 시작합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| document | [Document](../../com.aspose.note/document) | `Document` 노드. |

### visitImageEnd(Image image) {#visitImageEnd-com.aspose.note.Image-}
```
public void visitImageEnd(Image image)
```


`Image` 노드 방문을 종료합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | `Image` 노드. |

### visitImageStart(Image image) {#visitImageStart-com.aspose.note.Image-}
```
public void visitImageStart(Image image)
```


`Image` 노드 방문을 시작합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| image | [Image](../../com.aspose.note/image) | `Image` 노드. |

### visitInkDrawingEnd(InkDrawing inkDrawing) {#visitInkDrawingEnd-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingEnd(InkDrawing inkDrawing)
```


[InkDrawing](../../com.aspose.note/inkdrawing) 노드 방문을 종료합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | [InkDrawing](../../com.aspose.note/inkdrawing) 노드. |

### visitInkDrawingStart(InkDrawing inkDrawing) {#visitInkDrawingStart-com.aspose.note.InkDrawing-}
```
public void visitInkDrawingStart(InkDrawing inkDrawing)
```


[InkDrawing](../../com.aspose.note/inkdrawing) 노드 방문을 시작합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| inkDrawing | [InkDrawing](../../com.aspose.note/inkdrawing) | [InkDrawing](../../com.aspose.note/inkdrawing) 노드. |

### visitInkParagraphEnd(InkParagraph inkParagraph) {#visitInkParagraphEnd-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphEnd(InkParagraph inkParagraph)
```


[InkParagraph](../../com.aspose.note/inkparagraph) 노드 방문을 종료합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | [InkParagraph](../../com.aspose.note/inkparagraph) 노드. |

### visitInkParagraphStart(InkParagraph inkParagraph) {#visitInkParagraphStart-com.aspose.note.InkParagraph-}
```
public void visitInkParagraphStart(InkParagraph inkParagraph)
```


[InkParagraph](../../com.aspose.note/inkparagraph) 노드 방문을 시작합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| inkParagraph | [InkParagraph](../../com.aspose.note/inkparagraph) | [InkParagraph](../../com.aspose.note/inkparagraph) 노드. |

### visitInkWordEnd(InkWord inkWord) {#visitInkWordEnd-com.aspose.note.InkWord-}
```
public void visitInkWordEnd(InkWord inkWord)
```


[InkWord](../../com.aspose.note/inkword) 노드 방문을 종료합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | [InkWord](../../com.aspose.note/inkword) 노드. |

### visitInkWordStart(InkWord inkWord) {#visitInkWordStart-com.aspose.note.InkWord-}
```
public void visitInkWordStart(InkWord inkWord)
```


[InkWord](../../com.aspose.note/inkword) 노드 방문을 시작합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| inkWord | [InkWord](../../com.aspose.note/inkword) | [InkWord](../../com.aspose.note/inkword) 노드. |

### visitLoopEnd(Loop loop) {#visitLoopEnd-com.aspose.note.Loop-}
```
public void visitLoopEnd(Loop loop)
```


[Loop](../../com.aspose.note/loop) 노드 방문을 종료합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | [Loop](../../com.aspose.note/loop) 노드. |

### visitLoopStart(Loop loop) {#visitLoopStart-com.aspose.note.Loop-}
```
public void visitLoopStart(Loop loop)
```


[Loop](../../com.aspose.note/loop) 노드 방문을 시작합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| loop | [Loop](../../com.aspose.note/loop) | [Loop](../../com.aspose.note/loop) 노드. |

### visitOutlineElementEnd(OutlineElement outlineElement) {#visitOutlineElementEnd-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementEnd(OutlineElement outlineElement)
```


`OutlineElement` 노드 방문을 종료합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | `OutlineElement` 노드. |

### visitOutlineElementStart(OutlineElement outlineElement) {#visitOutlineElementStart-com.aspose.note.OutlineElement-}
```
public void visitOutlineElementStart(OutlineElement outlineElement)
```


`OutlineElement` 노드 방문을 시작합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| outlineElement | [OutlineElement](../../com.aspose.note/outlineelement) | `OutlineElement` 노드. |

### visitOutlineEnd(Outline outline) {#visitOutlineEnd-com.aspose.note.Outline-}
```
public void visitOutlineEnd(Outline outline)
```


`Outline` 노드 방문을 종료합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | `Outline` 노드. |

### visitOutlineGroupEnd(OutlineGroup outlineGroup) {#visitOutlineGroupEnd-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupEnd(OutlineGroup outlineGroup)
```


`OutlineGroup` 노드 방문을 종료합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | `OutlineGroup` 노드. |

### visitOutlineGroupStart(OutlineGroup outlineGroup) {#visitOutlineGroupStart-com.aspose.note.OutlineGroup-}
```
public void visitOutlineGroupStart(OutlineGroup outlineGroup)
```


`OutlineGroup` 노드 방문을 시작합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| outlineGroup | [OutlineGroup](../../com.aspose.note/outlinegroup) | `OutlineGroup` 노드. |

### visitOutlineStart(Outline outline) {#visitOutlineStart-com.aspose.note.Outline-}
```
public void visitOutlineStart(Outline outline)
```


`Outline` 노드 방문을 시작합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| outline | [Outline](../../com.aspose.note/outline) | `Outline` 노드. |

### visitPageEnd(Page page) {#visitPageEnd-com.aspose.note.Page-}
```
public void visitPageEnd(Page page)
```


`Page` 노드 방문을 종료합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | `Page` 노드. |

### visitPageStart(Page page) {#visitPageStart-com.aspose.note.Page-}
```
public void visitPageStart(Page page)
```


`Page` 노드 방문을 시작합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | `Page` 노드. |

### visitRichTextEnd(RichText richText) {#visitRichTextEnd-com.aspose.note.RichText-}
```
public void visitRichTextEnd(RichText richText)
```


`RichText` 노드 방문을 종료합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | `RichText` 노드. |

### visitRichTextStart(RichText richText) {#visitRichTextStart-com.aspose.note.RichText-}
```
public void visitRichTextStart(RichText richText)
```


`RichText` 노드 방문을 시작합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| richText | [RichText](../../com.aspose.note/richtext) | `RichText` 노드. |

### visitTableCellEnd(TableCell tableCell) {#visitTableCellEnd-com.aspose.note.TableCell-}
```
public void visitTableCellEnd(TableCell tableCell)
```


`TableCell` 노드 방문을 종료합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | `TableCell` 노드. |

### visitTableCellStart(TableCell tableCell) {#visitTableCellStart-com.aspose.note.TableCell-}
```
public void visitTableCellStart(TableCell tableCell)
```


`TableCell` 노드 방문을 시작합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| tableCell | [TableCell](../../com.aspose.note/tablecell) | `TableCell` 노드. |

### visitTableEnd(Table table) {#visitTableEnd-com.aspose.note.Table-}
```
public void visitTableEnd(Table table)
```


`Table` 노드 방문을 종료합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | `Table` 노드. |

### visitTableRowEnd(TableRow tableRow) {#visitTableRowEnd-com.aspose.note.TableRow-}
```
public void visitTableRowEnd(TableRow tableRow)
```


`TableRow` 노드 방문을 종료합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | `TableRow` 노드. |

### visitTableRowStart(TableRow tableRow) {#visitTableRowStart-com.aspose.note.TableRow-}
```
public void visitTableRowStart(TableRow tableRow)
```


`TableRow` 노드 방문을 시작합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| tableRow | [TableRow](../../com.aspose.note/tablerow) | `TableRow` 노드. |

### visitTableStart(Table table) {#visitTableStart-com.aspose.note.Table-}
```
public void visitTableStart(Table table)
```


`Table` 노드 방문을 시작합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| table | [Table](../../com.aspose.note/table) | `Table` 노드. |

### visitTitleEnd(Title title) {#visitTitleEnd-com.aspose.note.Title-}
```
public void visitTitleEnd(Title title)
```


`Title` 노드 방문을 종료합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | `Title` 노드. |

### visitTitleStart(Title title) {#visitTitleStart-com.aspose.note.Title-}
```
public void visitTitleStart(Title title)
```


`Title` 노드 방문을 시작합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| title | [Title](../../com.aspose.note/title) | `Title` 노드. |

