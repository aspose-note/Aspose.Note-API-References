---
title: "SaveOptions"
second_title: "Aspose.Note for Java API 参考"
description: "一个抽象基类，表示特定格式的文档保存选项。"
type: docs
weight: 85
url: /zh/java/com.aspose.note/saveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SaveOptions
```

一个抽象基类，表示特定格式的文档保存选项。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getFontsSubsystem()](#getFontsSubsystem--) | 获取或设置保存时使用的字体设置 |
| [getPageCount()](#getPageCount--) | 获取或设置要保存的页数。 |
| [getPageIndex()](#getPageIndex--) | 获取或设置要保存的第一页的索引。 |
| [getSaveFormat()](#getSaveFormat--) | 获取或设置文档保存的格式。 |
| [setFontsSubsystem(FontsSubsystem value)](#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-) | 获取或设置保存时使用的字体设置 |
| [setPageCount(int value)](#setPageCount-int-) | 获取或设置要保存的页数。 |
| [setPageIndex(int value)](#setPageIndex-int-) | 获取或设置要保存的第一页的索引。 |
### getFontsSubsystem() {#getFontsSubsystem--}
```
public final FontsSubsystem getFontsSubsystem()
```


获取或设置保存时使用的字体设置

**Returns:**
[FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


获取或设置要保存的页数。默认值为 \{@link int\#Int32Extensions.MaxValue\}，这表示文档的所有页面都将被渲染。

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


获取或设置要保存的第一页的索引。默认值为 0。

**Returns:**
int
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


获取或设置文档保存的格式。

**Returns:**
int
### setFontsSubsystem(FontsSubsystem value) {#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-}
```
public final void setFontsSubsystem(FontsSubsystem value)
```


获取或设置保存时使用的字体设置

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem) |  |

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


获取或设置要保存的页数。默认值为 \{@link int\#Int32Extensions.MaxValue\}，这表示文档的所有页面都将被渲染。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


获取或设置要保存的第一页的索引。默认值为 0。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

