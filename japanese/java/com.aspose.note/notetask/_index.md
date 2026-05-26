---
title: "NoteTask"
second_title: "Aspose.Note for Java API リファレンス"
description: "ノートタスクを表します。"
type: docs
weight: 55
url: /ja/java/com.aspose.note/notetask/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended, [com.aspose.note.CheckBox](../../com.aspose.note/checkbox)
```
public final class NoteTask extends CheckBox
```

ノートタスクを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [createCustomFollowUpDate(Date dueDate)](#createCustomFollowUpDate-java.util.Date-) | NoFollowUpDateFlag アイコンと指定された期限日で新しいノートタスクを作成します。 |
| [createFollowUpNextWeek()](#createFollowUpNextWeek--) | \* FollowUpNextWeekFlag アイコンで新しいノートタグを作成します。 |
| [createFollowUpThisWeek()](#createFollowUpThisWeek--) | \* FollowUpThisWeekFlag アイコンで新しいノートタグを作成します。 |
| [createFollowUpToday()](#createFollowUpToday--) | \* FollowUpTodayFlag アイコンで新しいノートタグを作成します。 |
| [createFollowUpTomorrow()](#createFollowUpTomorrow--) | \* FollowUpTomorrowFlag アイコンで新しいノートタグを作成します。 |
| [createNoFollowUpDate()](#createNoFollowUpDate--) | \* NoFollowUpDateFlag アイコンで新しいノートタグを作成します。 |
| [equals(NoteTask other)](#equals-com.aspose.note.NoteTask-) | 指定されたオブジェクトが現在のオブジェクトと等しいかどうかを判断します。 |
| [equals(Object obj)](#equals-java.lang.Object-) | 指定されたオブジェクトが現在のオブジェクトと等しいかどうかを判断します。 |
| [getDueDate()](#getDueDate--) | 期限日を取得または設定します。 |
| [getIcon()](#getIcon--) | アイコンを取得または設定します。 |
| [getLabel()](#getLabel--) |  |
| [hashCode()](#hashCode--) | 型のハッシュ関数として機能します。 |
| [setDueDate(Date value)](#setDueDate-java.util.Date-) | 期限日を取得または設定します。 |
| [setOpen()](#setOpen--) | タグを開いた状態に設定します。 |
### createCustomFollowUpDate(Date dueDate) {#createCustomFollowUpDate-java.util.Date-}
```
public static NoteTask createCustomFollowUpDate(Date dueDate)
```


NoFollowUpDateFlag アイコンと指定された期限日で新しいノートタスクを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dueDate | java.util.Date | 期限日。 |

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpNextWeek() {#createFollowUpNextWeek--}
```
public static NoteTask createFollowUpNextWeek()
```


\* FollowUpNextWeekFlag アイコンで新しいノートタグを作成します。

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpThisWeek() {#createFollowUpThisWeek--}
```
public static NoteTask createFollowUpThisWeek()
```


\* FollowUpThisWeekFlag アイコンで新しいノートタグを作成します。

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpToday() {#createFollowUpToday--}
```
public static NoteTask createFollowUpToday()
```


\* FollowUpTodayFlag アイコンで新しいノートタグを作成します。

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createFollowUpTomorrow() {#createFollowUpTomorrow--}
```
public static NoteTask createFollowUpTomorrow()
```


\* FollowUpTomorrowFlag アイコンで新しいノートタグを作成します。

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### createNoFollowUpDate() {#createNoFollowUpDate--}
```
public static NoteTask createNoFollowUpDate()
```


\* NoFollowUpDateFlag アイコンで新しいノートタグを作成します。

**Returns:**
[NoteTask](../../com.aspose.note/notetask) - The [NoteTask](../../com.aspose.note/notetask).
### equals(NoteTask other) {#equals-com.aspose.note.NoteTask-}
```
public boolean equals(NoteTask other)
```


指定されたオブジェクトが現在のオブジェクトと等しいかどうかを判断します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| other | [NoteTask](../../com.aspose.note/notetask) | オブジェクトです。 |

**Returns:**
boolean - `bool`です。
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


指定されたオブジェクトが現在のオブジェクトと等しいかどうかを判断します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| obj | java.lang.Object | オブジェクトです。 |

**Returns:**
boolean - `bool`です。
### getDueDate() {#getDueDate--}
```
public Date getDueDate()
```


期限日を取得または設定します。

値: `DateTime`。

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public int getIcon()
```


アイコンを取得または設定します。

値: [TagIcon](../../com.aspose.note.infrastructure/tagicon)です。

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


型のハッシュ関数として機能します。

**Returns:**
int - `int`です。
### setDueDate(Date value) {#setDueDate-java.util.Date-}
```
public void setDueDate(Date value)
```


期限日を取得または設定します。

値: `DateTime`。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


タグを開いた状態に設定します。

