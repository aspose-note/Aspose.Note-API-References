---
title: "PageHistory"
second_title: "Aspose.Note for Java API 参考"
description: "表示页面历史。"
type: docs
weight: 70
url: /zh/java/com.aspose.note/pagehistory/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericList
```
public class PageHistory implements System.Collections.Generic.IGenericList<Page>
```

表示页面历史。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [PageHistory(Page page)](#PageHistory-com.aspose.note.Page-) | 初始化 `PageHistory` 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [addItem(Page item)](#addItem-com.aspose.note.Page-) | 将页面版本添加到 `PageHistory` 的末尾。 |
| [addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items)](#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--) | 将页面版本添加到 `PageHistory` 的末尾。 |
| [clear()](#clear--) | 清除页面历史记录。 |
| [containsItem(Page item)](#containsItem-com.aspose.note.Page-) | 确定页面历史记录是否包含该页面版本。 |
| [copyToTArray(Page[] array, int arrayIndex)](#copyToTArray-com.aspose.note.Page---int-) | 将页面版本复制到数组中，从特定索引开始。 |
| [getCurrent()](#getCurrent--) | 获取当前页面版本。 |
| [get_Item(int index)](#get-Item-int-) | 获取或设置 `PageHistory` 中指定索引的页面版本。 |
| [indexOfItem(Page item)](#indexOfItem-com.aspose.note.Page-) | 确定页面历史中特定页面版本的索引。 |
| [insertItem(int index, Page item)](#insertItem-int-com.aspose.note.Page-) | 在页面历史中插入页面版本。 |
| [isReadOnly()](#isReadOnly--) | 获取一个值，指示页面历史是否为只读。 |
| [iterator()](#iterator--) | 返回一个枚举器，用于遍历 `PageHistory` 的子节点。 |
| [removeAt(int index)](#removeAt-int-) | 移除 `PageHistory` 中指定索引的页面版本。 |
| [removeItem(Page item)](#removeItem-com.aspose.note.Page-) | 从 `PageHistory` 中移除页面版本。 |
| [removeRange(int index, int count)](#removeRange-int-int-) | 从 `PageHistory` 中移除一系列页面版本。 |
| [set_Item(int index, Page value)](#set-Item-int-com.aspose.note.Page-) | 获取或设置 `PageHistory` 中指定索引的页面版本。 |
| [size()](#size--) | 获取页面历史中页面版本的计数。 |
### PageHistory(Page page) {#PageHistory-com.aspose.note.Page-}
```
public PageHistory(Page page)
```


初始化 `PageHistory` 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | 当前页面版本。 |

### addItem(Page item) {#addItem-com.aspose.note.Page-}
```
public void addItem(Page item)
```


将页面版本添加到 `PageHistory` 的末尾。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | 页面版本。 |

### addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items) {#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--}
```
public void addRange(System.Collections.Generic.IGenericEnumerable<Page> items)
```


将页面版本添加到 `PageHistory` 的末尾。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 项 | com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.Page&gt; | 页面版本的 `IEnumerable\\{Page\\}` 集合。 |

### clear() {#clear--}
```
public void clear()
```


清除页面历史记录。

### containsItem(Page item) {#containsItem-com.aspose.note.Page-}
```
public boolean containsItem(Page item)
```


确定页面历史记录是否包含该页面版本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | 页面版本。 |

**Returns:**
boolean - 该 `bool`。
### copyToTArray(Page[] array, int arrayIndex) {#copyToTArray-com.aspose.note.Page---int-}
```
public void copyToTArray(Page[] array, int arrayIndex)
```


将页面版本复制到数组中，从特定索引开始。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| array | [Page\[\]](../../com.aspose.note/page) | 目标数组。 |
| arrayIndex | int | 数组索引。 |

### getCurrent() {#getCurrent--}
```
public Page getCurrent()
```


获取当前页面版本。

**Returns:**
[Page](../../com.aspose.note/page)
### get_Item(int index) {#get-Item-int-}
```
public Page get_Item(int index)
```


获取或设置 `PageHistory` 中指定索引的页面版本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| index | int | 索引。 |

**Returns:**
[Page](../../com.aspose.note/page) - The page version.
### indexOfItem(Page item) {#indexOfItem-com.aspose.note.Page-}
```
public int indexOfItem(Page item)
```


确定页面历史中特定页面版本的索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | 页面版本。 |

**Returns:**
int - 该 `int`。
### insertItem(int index, Page item) {#insertItem-int-com.aspose.note.Page-}
```
public void insertItem(int index, Page item)
```


在页面历史中插入页面版本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| index | int | 索引。 |
| item | [Page](../../com.aspose.note/page) | 页面版本。 |

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


获取一个值，指示页面历史是否为只读。

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Page> iterator()
```


返回一个枚举器，用于遍历 `PageHistory` 的子节点。

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.Page&gt; - 该 `IEnumerator`。
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


移除 `PageHistory` 中指定索引的页面版本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| index | int | 索引。 |

### removeItem(Page item) {#removeItem-com.aspose.note.Page-}
```
public boolean removeItem(Page item)
```


从 `PageHistory` 中移除页面版本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | 页面版本。 |

**Returns:**
boolean - 该 `bool`。
### removeRange(int index, int count) {#removeRange-int-int-}
```
public void removeRange(int index, int count)
```


从 `PageHistory` 中移除一系列页面版本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| index | int | 索引。 |
| count | int | 计数。 |

### set_Item(int index, Page value) {#set-Item-int-com.aspose.note.Page-}
```
public void set_Item(int index, Page value)
```


获取或设置 `PageHistory` 中指定索引的页面版本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| index | int | 索引。 |
| value | [Page](../../com.aspose.note/page) |  |

### size() {#size--}
```
public int size()
```


获取页面历史中页面版本的计数。

**Returns:**
int
