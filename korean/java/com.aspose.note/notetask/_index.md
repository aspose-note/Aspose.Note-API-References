---
title: "NoteTask"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "노트 작업을 나타냅니다."
type: docs
weight: 55
url: /ko/java/com.aspose.note/notetask/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended, [com.aspose.note.CheckBox](../../com.aspose.note/checkbox)
```
public final class NoteTask extends CheckBox
```

노트 작업을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [createCustomFollowUpDate(Date dueDate)](#createCustomFollowUpDate-java.util.Date-) | NoFollowUpDateFlag 아이콘과 지정된 마감일을 사용하여 새 노트 작업을 생성합니다. |
| [createFollowUpNextWeek()](#createFollowUpNextWeek--) | * 다음 주 FollowUpNextWeekFlag 아이콘으로 새 노트 태그를 생성합니다. |
| [createFollowUpThisWeek()](#createFollowUpThisWeek--) | * 이번 주 FollowUpThisWeekFlag 아이콘으로 새 노트 태그를 생성합니다. |
| [createFollowUpToday()](#createFollowUpToday--) | * 오늘 FollowUpTodayFlag 아이콘으로 새 노트 태그를 생성합니다. |
| [createFollowUpTomorrow()](#createFollowUpTomorrow--) | * 내일 FollowUpTomorrowFlag 아이콘으로 새 노트 태그를 생성합니다. |
| [createNoFollowUpDate()](#createNoFollowUpDate--) | * NoFollowUpDateFlag 아이콘으로 새 노트 태그를 생성합니다. |
| [equals(NoteTask other)](#equals-com.aspose.note.NoteTask-) | 지정된 객체가 현재 객체와 같은지 여부를 결정합니다. |
| [equals(Object obj)](#equals-java.lang.Object-) | 지정된 객체가 현재 객체와 같은지 여부를 결정합니다. |
| [getDueDate()](#getDueDate--) | 마감일을 가져오거나 설정합니다. |
| [getIcon()](#getIcon--) | 아이콘을 가져오거나 설정합니다. |
| [getLabel()](#getLabel--) |  |
| [hashCode()](#hashCode--) | 해당 유형에 대한 해시 함수로 사용됩니다. |
| [setDueDate(Date value)](#setDueDate-java.util.Date-) | 마감일을 가져오거나 설정합니다. |
| [setOpen()](#setOpen--) | 태그를 열림 상태로 설정합니다. |
### createCustomFollowUpDate(Date dueDate) {#createCustomFollowUpDate-java.util.Date-}
```
public static NoteTask createCustomFollowUpDate(Date dueDate)
```


NoFollowUpDateFlag 아이콘과 지정된 마감일을 사용하여 새 노트 작업을 생성합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| dueDate | java.util.Date | 마감일. |

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpNextWeek() {#createFollowUpNextWeek--}
```
public static NoteTask createFollowUpNextWeek()
```


* 다음 주 FollowUpNextWeekFlag 아이콘으로 새 노트 태그를 생성합니다.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpThisWeek() {#createFollowUpThisWeek--}
```
public static NoteTask createFollowUpThisWeek()
```


* 이번 주 FollowUpThisWeekFlag 아이콘으로 새 노트 태그를 생성합니다.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpToday() {#createFollowUpToday--}
```
public static NoteTask createFollowUpToday()
```


* 오늘 FollowUpTodayFlag 아이콘으로 새 노트 태그를 생성합니다.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpTomorrow() {#createFollowUpTomorrow--}
```
public static NoteTask createFollowUpTomorrow()
```


* 내일 FollowUpTomorrowFlag 아이콘으로 새 노트 태그를 생성합니다.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createNoFollowUpDate() {#createNoFollowUpDate--}
```
public static NoteTask createNoFollowUpDate()
```


* NoFollowUpDateFlag 아이콘으로 새 노트 태그를 생성합니다.

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### equals(NoteTask other) {#equals-com.aspose.note.NoteTask-}
```
public boolean equals(NoteTask other)
```


지정된 객체가 현재 객체와 같은지 여부를 결정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| other | [NoteTask](../../com.aspose.note/notetask) | 객체입니다. |

**Returns:**
boolean - `bool`입니다.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


지정된 객체가 현재 객체와 같은지 여부를 결정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| obj | java.lang.Object | 객체입니다. |

**Returns:**
boolean - `bool`입니다.
### getDueDate() {#getDueDate--}
```
public Date getDueDate()
```


마감일을 가져오거나 설정합니다.

값: `DateTime`.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public int getIcon()
```


아이콘을 가져오거나 설정합니다.

값: [TagIcon](../../com.aspose.note.infrastructure/tagicon)입니다.

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


해당 유형에 대한 해시 함수로 사용됩니다.

**Returns:**
int - `int`입니다.
### setDueDate(Date value) {#setDueDate-java.util.Date-}
```
public void setDueDate(Date value)
```


마감일을 가져오거나 설정합니다.

값: `DateTime`.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


태그를 열림 상태로 설정합니다.

