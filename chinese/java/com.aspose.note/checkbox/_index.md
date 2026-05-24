---
title: "CheckBox"
second_title: "Aspose.Note for Java API 参考"
description: "可在完成和未完成状态之间切换的标签的基类。"
type: docs
weight: 13
url: /zh/java/com.aspose.note/checkbox/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended
```
public abstract class CheckBox extends TagExtended
```

可在完成和未完成状态之间切换的标签的基类。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getChecked()](#getChecked--) | 获取一个值，指示 CheckBox 是否处于选中状态。 |
| [getCompletedTime()](#getCompletedTime--) | 获取或设置完成时间。 |
| [getCreationTime()](#getCreationTime--) | 获取或设置创建时间。 |
| [getIcon()](#getIcon--) | 获取或设置图标。 |
| [getStatus()](#getStatus--) | 获取或设置状态。 |
| [setCompleted()](#setCompleted--) | 使用当前时间作为完成时间，将 tag 设置为已完成状态。 |
| [setCompleted(Date completedTime)](#setCompleted-java.util.Date-) | 将 tag 设置为已完成状态。 |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | 获取或设置创建时间。 |
| [setOpen()](#setOpen--) | 将标签设置为打开状态。 |
### getChecked() {#getChecked--}
```
public final boolean getChecked()
```


获取一个值，指示 CheckBox 是否处于选中状态。

**Returns:**
boolean
### getCompletedTime() {#getCompletedTime--}
```
public final Date getCompletedTime()
```


获取或设置完成时间。

值：该 `Nullable\{DateTime\}`。

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


获取或设置创建时间。

值：该 java.util.Date。

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


获取或设置图标。

值：该 [TagIcon](../../com.aspose.note.infrastructure/tagicon)。

**Returns:**
int
### getStatus() {#getStatus--}
```
public final int getStatus()
```


获取或设置状态。

值：该 [TagStatus](../../com.aspose.note/tagstatus)。

**Returns:**
int
### setCompleted() {#setCompleted--}
```
public final void setCompleted()
```


使用当前时间作为完成时间，将 tag 设置为已完成状态。

### setCompleted(Date completedTime) {#setCompleted-java.util.Date-}
```
public final void setCompleted(Date completedTime)
```


将 tag 设置为已完成状态。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| completedTime | java.util.Date | 完成时间。 |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public final void setCreationTime(Date value)
```


获取或设置创建时间。

值：该 java.util.Date。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


将标签设置为打开状态。

