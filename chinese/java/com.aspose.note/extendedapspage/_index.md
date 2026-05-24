---
title: "ExtendedApsPage"
second_title: "Aspose.Note for Java API 参考"
description: "表示标准 ApsGlyphs 的包装器，扩展了一些绘图行为。"
type: docs
weight: 27
url: /zh/java/com.aspose.note/extendedapspage/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode, com.aspose.foundation.rendering.ApsCompositeNode, com.aspose.foundation.rendering.ApsPage

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsPage extends ApsPage implements System.Collections.Generic.IGenericEnumerable<ApsNode>
```

表示标准 ApsGlyphs 的包装器，扩展了一些绘图行为。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)](#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-) | 初始化 `ExtendedApsPage` 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getContentSize()](#getContentSize--) | 获取不包括页边距的页面尺寸。 |
| [getMargin()](#getMargin--) | 获取此页面的页边距。 |
| [getPageEndInNotePage()](#getPageEndInNotePage--) | 获取页面结束位置（在 MS OneNote 页面中），当一个 MS OneNote 页面被划分为多个 aps 页面时。 |
| [getPageSize()](#getPageSize--) | 获取最终页面尺寸。 |
| [getPageStartInNotePage()](#getPageStartInNotePage--) | 获取页面起始位置（在 MS OneNote 页面中），当一个 MS OneNote 页面被划分为多个 aps 页面时。 |
| [iterator()](#iterator--) | 返回遍历此页面所有节点的枚举器。 |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) | 获取枚举器。 |
### ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin) {#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-}
```
public ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)
```


初始化 `ExtendedApsPage` 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| pageSize | com.aspose.ms.System.Drawing.SizeF | 页面尺寸。 |
| pageStartInNotePage | float | 原始 MS OneNote 页面中的页面起始位置。 |
| margin | com.aspose.foundation.layout.Margin | 扩展的页面边距。 |

### getContentSize() {#getContentSize--}
```
public System.Drawing.SizeF getContentSize()
```


获取不包括页边距的页面尺寸。

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getMargin() {#getMargin--}
```
public Margin getMargin()
```


获取此页面的页边距。

**Returns:**
com.aspose.foundation.layout.Margin
### getPageEndInNotePage() {#getPageEndInNotePage--}
```
public float getPageEndInNotePage()
```


获取页面结束位置（在 MS OneNote 页面中），当一个 MS OneNote 页面被划分为多个 aps 页面时。

**Returns:**
float
### getPageSize() {#getPageSize--}
```
public System.Drawing.SizeF getPageSize()
```


获取最终页面尺寸。

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getPageStartInNotePage() {#getPageStartInNotePage--}
```
public float getPageStartInNotePage()
```


获取页面起始位置（在 MS OneNote 页面中），当一个 MS OneNote 页面被划分为多个 aps 页面时。

**Returns:**
float
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsNode> iterator()
```


返回遍历此页面所有节点的枚举器。

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsNode&gt; - `IEnumerator`。
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```


获取枚举器。

**Returns:**
com.aspose.ms.System.Collections.IEnumerator - `IEnumerator`。
