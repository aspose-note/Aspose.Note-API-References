---
title: "ITag"
second_title: "Aspose.Note for Java API 参考"
description: "各种标签的接口。"
type: docs
weight: 109
url: /zh/java/com.aspose.note/itag/
---
```
public interface ITag
```

各种标签的接口。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getCompletedTime()](#getCompletedTime--) | 获取完成时间。 |
| [getCreationTime()](#getCreationTime--) | 获取创建时间。 |
| [getIcon()](#getIcon--) | 获取图标。 |
| [getLabel()](#getLabel--) | 获取标签文本。 |
| [getStatus()](#getStatus--) | 获取状态。 |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | 设置创建时间。 |
### getCompletedTime() {#getCompletedTime--}
```
public abstract Date getCompletedTime()
```


获取完成时间。

值：该 `Nullable\{DateTime\}`。

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public abstract Date getCreationTime()
```


获取创建时间。

值：该 java.util.Date。

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


获取图标。

值：该 [TagIcon](../../com.aspose.note.infrastructure/tagicon)。

**Returns:**
int
### getLabel() {#getLabel--}
```
public abstract String getLabel()
```


获取标签文本。

**Returns:**
java.lang.String
### getStatus() {#getStatus--}
```
public abstract int getStatus()
```


获取状态。

值：该 [TagStatus](../../com.aspose.note/tagstatus)。

**Returns:**
int
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public abstract void setCreationTime(Date value)
```


设置创建时间。

值：该 java.util.Date。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date |  |

