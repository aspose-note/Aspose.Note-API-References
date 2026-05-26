---
title: "ITag"
second_title: "Aspose.Note for Java API リファレンス"
description: "あらゆる種類のタグのインターフェイスです。"
type: docs
weight: 109
url: /ja/java/com.aspose.note/itag/
---
```
public interface ITag
```

あらゆる種類のタグのインターフェイスです。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getCompletedTime()](#getCompletedTime--) | 完了時刻を取得します。 |
| [getCreationTime()](#getCreationTime--) | 作成時刻を取得します。 |
| [getIcon()](#getIcon--) | アイコンを取得します。 |
| [getLabel()](#getLabel--) | ラベルテキストを取得します。 |
| [getStatus()](#getStatus--) | ステータスを取得します。 |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | 作成時刻を設定します。 |
### getCompletedTime() {#getCompletedTime--}
```
public abstract Date getCompletedTime()
```


完了時刻を取得します。

値: `Nullable\{DateTime\}`です。

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public abstract Date getCreationTime()
```


作成時刻を取得します。

値: java.util.Dateです。

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


アイコンを取得します。

値: [TagIcon](../../com.aspose.note.infrastructure/tagicon)です。

**Returns:**
int
### getLabel() {#getLabel--}
```
public abstract String getLabel()
```


ラベルテキストを取得します。

**Returns:**
java.lang.String
### getStatus() {#getStatus--}
```
public abstract int getStatus()
```


ステータスを取得します。

値: [TagStatus](../../com.aspose.note/tagstatus)です。

**Returns:**
int
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public abstract void setCreationTime(Date value)
```


作成時刻を設定します。

値: java.util.Dateです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date |  |

