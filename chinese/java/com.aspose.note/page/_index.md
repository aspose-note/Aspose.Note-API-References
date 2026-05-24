---
title: "Page"
second_title: "Aspose.Note for Java API 参考"
description: "表示一个页面。"
type: docs
weight: 69
url: /zh/java/com.aspose.note/page/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode
```
public final class Page extends CompositeNode<IPageChildNode>
```

表示一个页面。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Page()](#Page--) | 初始化 `Page` 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 接受节点的访问者。 |
| [deepClone()](#deepClone--) | 克隆页面。 |
| [deepClone(boolean cloneHistory)](#deepClone-boolean-) | 克隆页面。 |
| [getAuthor()](#getAuthor--) | 获取或设置作者。 |
| [getBackgroundColor()](#getBackgroundColor--) | 获取或设置页面的背景颜色。 |
| [getCreationTime()](#getCreationTime--) | 获取或设置创建时间。 |
| [getLastModifiedTime()](#getLastModifiedTime--) | 获取或设置最后修改时间。 |
| [getLevel()](#getLevel--) | 获取或设置级别。 |
| [getMargin()](#getMargin--) | 获取或设置边距。 |
| [getPageContentRevisionSummary()](#getPageContentRevisionSummary--) | 获取或设置页面及其子节点的修订摘要。 |
| [getPageLayoutSize()](#getPageLayoutSize--) | 获取在编辑器中显示的页面布局大小。 |
| [getSizeType()](#getSizeType--) | 获取或设置页面的大小类型。 |
| [getTitle()](#getTitle--) | 获取或设置标题。 |
| [isConflictPage()](#isConflictPage--) | 获取或设置一个值，指示此页面是否为冲突页面。 |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | 获取或设置作者。 |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | 获取或设置页面的背景颜色。 |
| [setConflictPage(boolean value)](#setConflictPage-boolean-) | 获取或设置一个值，指示此页面是否为冲突页面。 |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | 获取或设置创建时间。 |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 获取或设置最后修改时间。 |
| [setLevel(byte value)](#setLevel-byte-) | 获取或设置级别。 |
| [setMargin(Margins value)](#setMargin-com.aspose.note.Margins-) | 获取或设置边距。 |
| [setPageContentRevisionSummary(RevisionSummary value)](#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-) | 获取或设置页面及其子节点的修订摘要。 |
| [setPageLayoutSize(Dimension2D value)](#setPageLayoutSize-java.awt.geom.Dimension2D-) | 设置在编辑器中显示的页面布局大小。 |
| [setSizeType(int value)](#setSizeType-int-) | 获取或设置页面的大小类型。 |
| [setTitle(Title value)](#setTitle-com.aspose.note.Title-) | 获取或设置标题。 |
### Page() {#Page--}
```
public Page()
```


初始化 `Page` 类的新实例。

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


接受节点的访问者。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | 从 `DocumentVisitor` 派生的类的对象。 |

### deepClone() {#deepClone--}
```
public final Page deepClone()
```


克隆页面。

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### deepClone(boolean cloneHistory) {#deepClone-boolean-}
```
public final Page deepClone(boolean cloneHistory)
```


克隆页面。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cloneHistory | boolean | 指定是否应克隆页面的历史记录。 |

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


获取或设置作者。

**Returns:**
java.lang.String
### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


获取或设置页面的背景颜色。

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


获取或设置创建时间。

**Returns:**
java.util.Date
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


获取或设置最后修改时间。

**Returns:**
java.util.Date
### getLevel() {#getLevel--}
```
public byte getLevel()
```


获取或设置级别。

**Returns:**
byte
### getMargin() {#getMargin--}
```
public Margins getMargin()
```


获取或设置边距。

**Returns:**
[Margins](../../com.aspose.note/margins)
### getPageContentRevisionSummary() {#getPageContentRevisionSummary--}
```
public RevisionSummary getPageContentRevisionSummary()
```


获取或设置页面及其子节点的修订摘要。

**Returns:**
[RevisionSummary](../../com.aspose.note/revisionsummary)
### getPageLayoutSize() {#getPageLayoutSize--}
```
public final Dimension2D getPageLayoutSize()
```


获取在编辑器中显示的页面布局大小。

--------------------

此值由 Microsoft OneNote 应用程序在打开文档时用于显示底层页面布局。它不会影响文档的打印和保存。当 Page.SizeType 属性设置为 PageSizeType.SizeByContent 时，此属性返回内容的实际大小。

**Returns:**
java.awt.geom.Dimension2D
### getSizeType() {#getSizeType--}
```
public final int getSizeType()
```


获取或设置页面的大小类型。

--------------------

默认情况下，页面会自动调整大小。默认值是 [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent)。

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


获取或设置标题。

值：该 `Title`。

**Returns:**
[Title](../../com.aspose.note/title)
### isConflictPage() {#isConflictPage--}
```
public final boolean isConflictPage()
```


获取或设置一个值，指示此页面是否为冲突页面。

--------------------

当两个用户尝试更新相同内容时，会出现冲突页面。在这种情况下，第一位用户的更改会正常写入，但另一位用户的更改无法合并。因此会创建页面的副本并标记为冲突。

在此版本中，冲突会以第一位用户的更改为准进行解决。因此，如果文档中存在冲突页面，它们将在历史记录中显示，但在保存时会被跳过。可以重置此标志，以将这些页面像普通页面一样保存到历史记录中。

有关冲突页面操作的详细示例可在在线文档中找到。

**Returns:**
boolean
### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


获取或设置作者。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


获取或设置页面的背景颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.awt.Color |  |

### setConflictPage(boolean value) {#setConflictPage-boolean-}
```
public final void setConflictPage(boolean value)
```


获取或设置一个值，指示此页面是否为冲突页面。

--------------------

当两个用户尝试更新相同内容时，会出现冲突页面。在这种情况下，第一位用户的更改会正常写入，但另一位用户的更改无法合并。因此会创建页面的副本并标记为冲突。

在此版本中，冲突会以第一位用户的更改为准进行解决。因此，如果文档中存在冲突页面，它们将在历史记录中显示，但在保存时会被跳过。可以重置此标志，以将这些页面像普通页面一样保存到历史记录中。

有关冲突页面操作的详细示例可在在线文档中找到。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


获取或设置创建时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


获取或设置最后修改时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date |  |

### setLevel(byte value) {#setLevel-byte-}
```
public void setLevel(byte value)
```


获取或设置级别。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | byte |  |

### setMargin(Margins value) {#setMargin-com.aspose.note.Margins-}
```
public void setMargin(Margins value)
```


获取或设置边距。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Margins](../../com.aspose.note/margins) |  |

### setPageContentRevisionSummary(RevisionSummary value) {#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-}
```
public void setPageContentRevisionSummary(RevisionSummary value)
```


获取或设置页面及其子节点的修订摘要。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [RevisionSummary](../../com.aspose.note/revisionsummary) |  |

### setPageLayoutSize(Dimension2D value) {#setPageLayoutSize-java.awt.geom.Dimension2D-}
```
public final void setPageLayoutSize(Dimension2D value)
```


设置在编辑器中显示的页面布局大小。

--------------------

此值由 Microsoft OneNote 应用程序在打开文档时用于显示底层页面布局。它不会影响文档的打印和保存。当 Page.SizeType 属性设置为 PageSizeType.SizeByContent 时，此属性返回内容的实际大小。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.awt.geom.Dimension2D |  |

### setSizeType(int value) {#setSizeType-int-}
```
public final void setSizeType(int value)
```


获取或设置页面的大小类型。

--------------------

默认情况下，页面会自动调整大小。默认值是 [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTitle(Title value) {#setTitle-com.aspose.note.Title-}
```
public void setTitle(Title value)
```


获取或设置标题。

值：该 `Title`。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Title](../../com.aspose.note/title) |  |

