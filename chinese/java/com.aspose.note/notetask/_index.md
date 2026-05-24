---
title: "NoteTask"
second_title: "Aspose.Note for Java API 参考"
description: "表示笔记任务。"
type: docs
weight: 55
url: /zh/java/com.aspose.note/notetask/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended, [com.aspose.note.CheckBox](../../com.aspose.note/checkbox)
```
public final class NoteTask extends CheckBox
```

表示笔记任务。
## 方法

| 方法 | 描述 |
| --- | --- |
| [createCustomFollowUpDate(Date dueDate)](#createCustomFollowUpDate-java.util.Date-) | 创建一个带有 NoFollowUpDateFlag 图标和指定截止日期的新笔记任务。 |
| [createFollowUpNextWeek()](#createFollowUpNextWeek--) | * 创建一个带有 FollowUpNextWeekFlag 图标的新笔记标签。 |
| [createFollowUpThisWeek()](#createFollowUpThisWeek--) | * 创建一个带有 FollowUpThisWeekFlag 图标的新笔记标签。 |
| [createFollowUpToday()](#createFollowUpToday--) | * 创建一个带有 FollowUpTodayFlag 图标的新笔记标签。 |
| [createFollowUpTomorrow()](#createFollowUpTomorrow--) | * 创建一个带有 FollowUpTomorrowFlag 图标的新笔记标签。 |
| [createNoFollowUpDate()](#createNoFollowUpDate--) | * 创建一个带有 NoFollowUpDateFlag 图标的新笔记标签。 |
| [equals(NoteTask other)](#equals-com.aspose.note.NoteTask-) | 确定指定的对象是否等于当前对象。 |
| [equals(Object obj)](#equals-java.lang.Object-) | 确定指定的对象是否等于当前对象。 |
| [getDueDate()](#getDueDate--) | 获取或设置截止日期。 |
| [getIcon()](#getIcon--) | 获取或设置图标。 |
| [getLabel()](#getLabel--) |  |
| [hashCode()](#hashCode--) | 作为该类型的哈希函数。 |
| [setDueDate(Date value)](#setDueDate-java.util.Date-) | 获取或设置截止日期。 |
| [setOpen()](#setOpen--) | 将标签设置为打开状态。 |
### createCustomFollowUpDate(Date dueDate) {#createCustomFollowUpDate-java.util.Date-}
```
public static NoteTask createCustomFollowUpDate(Date dueDate)
```


创建一个带有 NoFollowUpDateFlag 图标和指定截止日期的新笔记任务。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dueDate | java.util.Date | 截止日期。 |

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpNextWeek() {#createFollowUpNextWeek--}
```
public static NoteTask createFollowUpNextWeek()
```


* 创建一个带有 FollowUpNextWeekFlag 图标的新笔记标签。

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpThisWeek() {#createFollowUpThisWeek--}
```
public static NoteTask createFollowUpThisWeek()
```


* 创建一个带有 FollowUpThisWeekFlag 图标的新笔记标签。

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpToday() {#createFollowUpToday--}
```
public static NoteTask createFollowUpToday()
```


* 创建一个带有 FollowUpTodayFlag 图标的新笔记标签。

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpTomorrow() {#createFollowUpTomorrow--}
```
public static NoteTask createFollowUpTomorrow()
```


* 创建一个带有 FollowUpTomorrowFlag 图标的新笔记标签。

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createNoFollowUpDate() {#createNoFollowUpDate--}
```
public static NoteTask createNoFollowUpDate()
```


* 创建一个带有 NoFollowUpDateFlag 图标的新笔记标签。

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### equals(NoteTask other) {#equals-com.aspose.note.NoteTask-}
```
public boolean equals(NoteTask other)
```


确定指定的对象是否等于当前对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | [NoteTask](../../com.aspose.note/notetask) | 对象。 |

**Returns:**
boolean - 该 `bool`。
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


确定指定的对象是否等于当前对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 对象 | java.lang.Object | 对象。 |

**Returns:**
boolean - 该 `bool`。
### getDueDate() {#getDueDate--}
```
public Date getDueDate()
```


获取或设置截止日期。

值：`DateTime`。

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public int getIcon()
```


获取或设置图标。

值：该 [TagIcon](../../com.aspose.note.infrastructure/tagicon)。

**Returns:**
int
### getLabel() {#getLabel--}
```
public String getLabel()
```




**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public int hashCode()
```


作为该类型的哈希函数。

**Returns:**
int - 该 `int`。
### setDueDate(Date value) {#setDueDate-java.util.Date-}
```
public void setDueDate(Date value)
```


获取或设置截止日期。

值：`DateTime`。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


将标签设置为打开状态。

