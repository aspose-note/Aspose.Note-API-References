---
title: "Page"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "페이지를 나타냅니다."
type: docs
weight: 69
url: /ko/java/com.aspose.note/page/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode
```
public final class Page extends CompositeNode<IPageChildNode>
```

페이지를 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Page()](#Page--) | `Page` 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 노드의 방문자를 수락합니다. |
| [deepClone()](#deepClone--) | 페이지를 복제합니다. |
| [deepClone(boolean cloneHistory)](#deepClone-boolean-) | 페이지를 복제합니다. |
| [getAuthor()](#getAuthor--) | 작성자를 가져오거나 설정합니다. |
| [getBackgroundColor()](#getBackgroundColor--) | 페이지의 배경색을 가져오거나 설정합니다. |
| [getCreationTime()](#getCreationTime--) | 생성 시간을 가져오거나 설정합니다. |
| [getLastModifiedTime()](#getLastModifiedTime--) | 마지막 수정 시간을 가져오거나 설정합니다. |
| [getLevel()](#getLevel--) | 레벨을 가져오거나 설정합니다. |
| [getMargin()](#getMargin--) | 여백을 가져오거나 설정합니다. |
| [getPageContentRevisionSummary()](#getPageContentRevisionSummary--) | 페이지 및 해당 자식 노드에 대한 리비전 요약을 가져오거나 설정합니다. |
| [getPageLayoutSize()](#getPageLayoutSize--) | 편집기에 표시되는 페이지의 레이아웃 크기를 가져옵니다. |
| [getSizeType()](#getSizeType--) | 페이지의 크기 유형을 가져오거나 설정합니다. |
| [getTitle()](#getTitle--) | 제목을 가져오거나 설정합니다. |
| [isConflictPage()](#isConflictPage--) | 이 페이지가 충돌 페이지인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | 작성자를 가져오거나 설정합니다. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | 페이지의 배경색을 가져오거나 설정합니다. |
| [setConflictPage(boolean value)](#setConflictPage-boolean-) | 이 페이지가 충돌 페이지인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | 생성 시간을 가져오거나 설정합니다. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 마지막 수정 시간을 가져오거나 설정합니다. |
| [setLevel(byte value)](#setLevel-byte-) | 레벨을 가져오거나 설정합니다. |
| [setMargin(Margins value)](#setMargin-com.aspose.note.Margins-) | 여백을 가져오거나 설정합니다. |
| [setPageContentRevisionSummary(RevisionSummary value)](#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-) | 페이지 및 해당 자식 노드에 대한 리비전 요약을 가져오거나 설정합니다. |
| [setPageLayoutSize(Dimension2D value)](#setPageLayoutSize-java.awt.geom.Dimension2D-) | 편집기에서 표시되는 페이지 레이아웃 크기를 설정합니다. |
| [setSizeType(int value)](#setSizeType-int-) | 페이지의 크기 유형을 가져오거나 설정합니다. |
| [setTitle(Title value)](#setTitle-com.aspose.note.Title-) | 제목을 가져오거나 설정합니다. |
### Page() {#Page--}
```
public Page()
```


`Page` 클래스의 새 인스턴스를 초기화합니다.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


노드의 방문자를 수락합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor`에서 파생된 클래스의 객체. |

### deepClone() {#deepClone--}
```
public final Page deepClone()
```


페이지를 복제합니다.

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### deepClone(boolean cloneHistory) {#deepClone-boolean-}
```
public final Page deepClone(boolean cloneHistory)
```


페이지를 복제합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| cloneHistory | boolean | 페이지의 기록을 복제할지 여부를 지정합니다.. |

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


작성자를 가져오거나 설정합니다.

**Returns:**
java.lang.String
### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


페이지의 배경색을 가져오거나 설정합니다.

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


생성 시간을 가져오거나 설정합니다.

**Returns:**
java.util.Date
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


마지막 수정 시간을 가져오거나 설정합니다.

**Returns:**
java.util.Date
### getLevel() {#getLevel--}
```
public byte getLevel()
```


레벨을 가져오거나 설정합니다.

**Returns:**
byte
### getMargin() {#getMargin--}
```
public Margins getMargin()
```


여백을 가져오거나 설정합니다.

**Returns:**
[Margins](../../com.aspose.note/margins)
### getPageContentRevisionSummary() {#getPageContentRevisionSummary--}
```
public RevisionSummary getPageContentRevisionSummary()
```


페이지 및 해당 자식 노드에 대한 리비전 요약을 가져오거나 설정합니다.

**Returns:**
[RevisionSummary](../../com.aspose.note/revisionsummary)
### getPageLayoutSize() {#getPageLayoutSize--}
```
public final Dimension2D getPageLayoutSize()
```


편집기에 표시되는 페이지의 레이아웃 크기를 가져옵니다.

--------------------

이 값은 Microsoft OneNote 애플리케이션에서 문서를 열 때 기본 페이지 레이아웃을 표시하는 데 사용됩니다. 인쇄 및 문서 저장에는 영향을 주지 않습니다. Page.SizeType 속성이 PageSizeType.SizeByContent 로 설정된 경우 이 속성은 콘텐츠의 실제 크기를 반환합니다.

**Returns:**
java.awt.geom.Dimension2D
### getSizeType() {#getSizeType--}
```
public final int getSizeType()
```


페이지의 크기 유형을 가져오거나 설정합니다.

--------------------

기본적으로 페이지는 자동으로 크기가 조정됩니다. 기본값은 [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent)입니다.

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


제목을 가져오거나 설정합니다.

값: `Title`.

**Returns:**
[Title](../../com.aspose.note/title)
### isConflictPage() {#isConflictPage--}
```
public final boolean isConflictPage()
```


이 페이지가 충돌 페이지인지 여부를 나타내는 값을 가져오거나 설정합니다.

--------------------

두 사용자가 동일한 콘텐츠를 업데이트하려 할 때 충돌 페이지가 발생합니다. 이 경우 첫 번째 사용자의 변경 사항은 정상적으로 기록됩니다. 그러나 다른 사용자의 변경 사항은 병합될 수 없습니다. 따라서 페이지 사본이 생성되어 충돌로 표시됩니다.

이 버전에서는 충돌이 첫 번째 사용자의 변경 사항을 우선하도록 해결됩니다. 따라서 문서에 충돌 페이지가 있는 경우 기록에는 표시되지만 저장 시 건너뛰게 됩니다. 이 플래그를 재설정하면 이러한 페이지를 일반 페이지처럼 기록에 저장할 수 있습니다.

온라인 문서에서 충돌 페이지를 조작하는 자세한 예제를 찾을 수 있습니다.

**Returns:**
boolean
### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


작성자를 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String |  |

### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


페이지의 배경색을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.awt.Color |  |

### setConflictPage(boolean value) {#setConflictPage-boolean-}
```
public final void setConflictPage(boolean value)
```


이 페이지가 충돌 페이지인지 여부를 나타내는 값을 가져오거나 설정합니다.

--------------------

두 사용자가 동일한 콘텐츠를 업데이트하려 할 때 충돌 페이지가 발생합니다. 이 경우 첫 번째 사용자의 변경 사항은 정상적으로 기록됩니다. 그러나 다른 사용자의 변경 사항은 병합될 수 없습니다. 따라서 페이지 사본이 생성되어 충돌로 표시됩니다.

이 버전에서는 충돌이 첫 번째 사용자의 변경 사항을 우선하도록 해결됩니다. 따라서 문서에 충돌 페이지가 있는 경우 기록에는 표시되지만 저장 시 건너뛰게 됩니다. 이 플래그를 재설정하면 이러한 페이지를 일반 페이지처럼 기록에 저장할 수 있습니다.

온라인 문서에서 충돌 페이지를 조작하는 자세한 예제를 찾을 수 있습니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean |  |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


생성 시간을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


마지막 수정 시간을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date |  |

### setLevel(byte value) {#setLevel-byte-}
```
public void setLevel(byte value)
```


레벨을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | byte |  |

### setMargin(Margins value) {#setMargin-com.aspose.note.Margins-}
```
public void setMargin(Margins value)
```


여백을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| value | [Margins](../../com.aspose.note/margins) |  |

### setPageContentRevisionSummary(RevisionSummary value) {#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-}
```
public void setPageContentRevisionSummary(RevisionSummary value)
```


페이지 및 해당 자식 노드에 대한 리비전 요약을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| value | [RevisionSummary](../../com.aspose.note/revisionsummary) |  |

### setPageLayoutSize(Dimension2D value) {#setPageLayoutSize-java.awt.geom.Dimension2D-}
```
public final void setPageLayoutSize(Dimension2D value)
```


편집기에서 표시되는 페이지 레이아웃 크기를 설정합니다.

--------------------

이 값은 Microsoft OneNote 애플리케이션에서 문서를 열 때 기본 페이지 레이아웃을 표시하는 데 사용됩니다. 인쇄 및 문서 저장에는 영향을 주지 않습니다. Page.SizeType 속성이 PageSizeType.SizeByContent 로 설정된 경우 이 속성은 콘텐츠의 실제 크기를 반환합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.awt.geom.Dimension2D |  |

### setSizeType(int value) {#setSizeType-int-}
```
public final void setSizeType(int value)
```


페이지의 크기 유형을 가져오거나 설정합니다.

--------------------

기본적으로 페이지는 자동으로 크기가 조정됩니다. 기본값은 [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent)입니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | int |  |

### setTitle(Title value) {#setTitle-com.aspose.note.Title-}
```
public void setTitle(Title value)
```


제목을 가져오거나 설정합니다.

값: `Title`.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| value | [Title](../../com.aspose.note/title) |  |

