---
title: "KeepPartAndCloneSolidObjectToNextPageAlgorithm"
second_title: "Aspose.Note for Java API 参考"
description: "将对象的顶部部分添加到页面底部，并在对象无法适应原页面时将完整对象克隆到下一页。"
type: docs
weight: 42
url: /zh/java/com.aspose.note/keeppartandclonesolidobjecttonextpagealgorithm/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
```
public class KeepPartAndCloneSolidObjectToNextPageAlgorithm extends PageSplittingAlgorithm
```

将对象的顶部添加到页面底部，并在对象不适合原始页面时将完整对象克隆到下一页。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm()](#KeepPartAndCloneSolidObjectToNextPageAlgorithm--) | 使用克隆部分的默认高度限制初始化 `KeepPartAndCloneSolidObjectToNextPageAlgorithm` 类的新实例。 |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm(float heightLimitOfClonedPart)](#KeepPartAndCloneSolidObjectToNextPageAlgorithm-float-) | 使用克隆部分的特定高度限制初始化 `KeepPartAndCloneSolidObjectToNextPageAlgorithm` 类的新实例。 |
## 字段

| 字段 | 描述 |
| --- | --- |
| [DEFAULT_HEIGHT_LIMIT_OF_CLONED_PART](#DEFAULT-HEIGHT-LIMIT-OF-CLONED-PART) | 克隆部分的默认最大尺寸。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getHeightLimitOfClonedPart()](#getHeightLimitOfClonedPart--) | 获取克隆部分的高度限制。 |
### KeepPartAndCloneSolidObjectToNextPageAlgorithm() {#KeepPartAndCloneSolidObjectToNextPageAlgorithm--}
```
public KeepPartAndCloneSolidObjectToNextPageAlgorithm()
```


使用克隆部分的默认高度限制初始化 `KeepPartAndCloneSolidObjectToNextPageAlgorithm` 类的新实例。

### KeepPartAndCloneSolidObjectToNextPageAlgorithm(float heightLimitOfClonedPart) {#KeepPartAndCloneSolidObjectToNextPageAlgorithm-float-}
```
public KeepPartAndCloneSolidObjectToNextPageAlgorithm(float heightLimitOfClonedPart)
```


使用克隆部分的特定高度限制初始化 `KeepPartAndCloneSolidObjectToNextPageAlgorithm` 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| heightLimitOfClonedPart | float | 克隆部分的最大高度。 |

### DEFAULT_HEIGHT_LIMIT_OF_CLONED_PART {#DEFAULT-HEIGHT-LIMIT-OF-CLONED-PART}
```
public static final float DEFAULT_HEIGHT_LIMIT_OF_CLONED_PART
```


克隆部分的默认最大尺寸。

### getHeightLimitOfClonedPart() {#getHeightLimitOfClonedPart--}
```
public float getHeightLimitOfClonedPart()
```


获取克隆部分的高度限制。

**Returns:**
float
