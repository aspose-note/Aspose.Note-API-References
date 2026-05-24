---
title: "ExtendedApsDocument"
second_title: "Aspose.Note for Java API 参考"
description: "表示一个完整的单页文档，由页面转换为页面集组成。"
type: docs
weight: 23
url: /zh/java/com.aspose.note/extendedapsdocument/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsDocument extends ApsNode implements System.Collections.Generic.IGenericEnumerable<ApsPage>
```

表示完整的 OneNote 文档，由转换为页面集的页面组成。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ExtendedApsDocument()](#ExtendedApsDocument--) | 初始化 `ExtendedApsDocument` 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [accept(ApsDocumentVisitor visitor)](#accept-com.aspose.foundation.rendering.ApsDocumentVisitor-) | 接受 ApsDocumentVisitor 到此元素。 |
| [addPage(ApsPage page)](#addPage-com.aspose.foundation.rendering.ApsPage-) | 向文档添加页面集。 |
| [getPageList()](#getPageList--) | 获取页面集列表。 |
| [iterator()](#iterator--) | 返回枚举器。 |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) |  |
### ExtendedApsDocument() {#ExtendedApsDocument--}
```
public ExtendedApsDocument()
```


初始化 `ExtendedApsDocument` 类的新实例。

### accept(ApsDocumentVisitor visitor) {#accept-com.aspose.foundation.rendering.ApsDocumentVisitor-}
```
public void accept(ApsDocumentVisitor visitor)
```


接受 ApsDocumentVisitor 到此元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 访问者 | com.aspose.foundation.rendering.ApsDocumentVisitor | 访问者。 |

### addPage(ApsPage page) {#addPage-com.aspose.foundation.rendering.ApsPage-}
```
public void addPage(ApsPage page)
```


向文档添加页面集。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 页面 | com.aspose.foundation.rendering.ApsPage | 页面集。 |

### getPageList() {#getPageList--}
```
public System.Collections.Generic.List<ApsPage> getPageList()
```


获取页面集列表。

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.foundation.rendering.ApsPage&gt;
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsPage> iterator()
```


返回枚举器。

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsPage&gt;
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```




**Returns:**
com.aspose.ms.System.Collections.IEnumerator
