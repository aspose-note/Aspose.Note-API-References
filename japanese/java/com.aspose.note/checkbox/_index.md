---
title: "CheckBox"
second_title: "Aspose.Note for Java API リファレンス"
description: "完了と未完了の状態を切り替えることができるタグの基底クラスです。"
type: docs
weight: 13
url: /ja/java/com.aspose.note/checkbox/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended
```
public abstract class CheckBox extends TagExtended
```

完了と未完了の状態を切り替えることができるタグの基底クラスです。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getChecked()](#getChecked--) | CheckBox がチェックされた状態かどうかを示す値を取得します。 |
| [getCompletedTime()](#getCompletedTime--) | 完了時間を取得または設定します。 |
| [getCreationTime()](#getCreationTime--) | 作成時間を取得または設定します。 |
| [getIcon()](#getIcon--) | アイコンを取得または設定します。 |
| [getStatus()](#getStatus--) | ステータスを取得または設定します。 |
| [setCompleted()](#setCompleted--) | 現在時刻を完了時刻として使用し、タグを完了状態に設定します。 |
| [setCompleted(Date completedTime)](#setCompleted-java.util.Date-) | タグを完了状態に設定します。 |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | 作成時間を取得または設定します。 |
| [setOpen()](#setOpen--) | タグを開いた状態に設定します。 |
### getChecked() {#getChecked--}
```
public final boolean getChecked()
```


CheckBox がチェックされた状態かどうかを示す値を取得します。

**Returns:**
boolean
### getCompletedTime() {#getCompletedTime--}
```
public final Date getCompletedTime()
```


完了時間を取得または設定します。

値: `Nullable\{DateTime\}`です。

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


作成時間を取得または設定します。

値: java.util.Dateです。

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


アイコンを取得または設定します。

値: [TagIcon](../../com.aspose.note.infrastructure/tagicon)です。

**Returns:**
int
### getStatus() {#getStatus--}
```
public final int getStatus()
```


ステータスを取得または設定します。

値: [TagStatus](../../com.aspose.note/tagstatus)です。

**Returns:**
int
### setCompleted() {#setCompleted--}
```
public final void setCompleted()
```


現在時刻を完了時刻として使用し、タグを完了状態に設定します。

### setCompleted(Date completedTime) {#setCompleted-java.util.Date-}
```
public final void setCompleted(Date completedTime)
```


タグを完了状態に設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| completedTime | java.util.Date | 完了時刻です。 |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public final void setCreationTime(Date value)
```


作成時間を取得または設定します。

値: java.util.Dateです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


タグを開いた状態に設定します。

