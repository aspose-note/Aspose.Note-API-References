---
title: "RichText"
second_title: "Aspose.Note for Java API リファレンス"
description: "リッチテキストを表します。"
type: docs
weight: 82
url: /ja/java/com.aspose.note/richtext/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class RichText extends Node implements IOutlineElementChildNode, ITaggable, System.Collections.Generic.IGenericEnumerable<Character>
```

リッチテキストを表します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [RichText()](#RichText--) | [RichText](../../com.aspose.note/richtext) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | ノードのビジターを受け入れます。 |
| [append(String value)](#append-java.lang.String-) | 最後のテキスト範囲に文字列を追加します。 |
| [append(String value, TextStyle style)](#append-java.lang.String-com.aspose.note.TextStyle-) | 文字列を末尾に追加します。 |
| [appendFront(String value)](#appendFront-java.lang.String-) | 文字列を最初のテキスト範囲の先頭に追加します。 |
| [appendFront(String value, TextStyle style)](#appendFront-java.lang.String-com.aspose.note.TextStyle-) | 文字列を先頭に追加します。 |
| [clear()](#clear--) | このインスタンスの内容をクリアします。 |
| [getAlignment()](#getAlignment--) | 配置を取得します。 |
| [getLastModifiedTime()](#getLastModifiedTime--) | 最終更新時刻を取得します。 |
| [getLength()](#getLength--) |  |
| [getLineSpacing()](#getLineSpacing--) | 行間隔を取得します。 |
| [getParagraphStyle()](#getParagraphStyle--) | 段落スタイルを取得します。 |
| [getSpaceAfter()](#getSpaceAfter--) | 後ろの最小余白を取得します。 |
| [getSpaceBefore()](#getSpaceBefore--) | 前の最小余白を取得します。 |
| [getStyles()](#getStyles--) | スタイルを取得します。 |
| [getTags()](#getTags--) | 段落のすべてのタグの一覧を取得します。 |
| [getText()](#getText--) | テキストを取得します。 |
| [getTextRuns()](#getTextRuns--) |  |
| [indexOf(char value)](#indexOf-char-) | この文字列内で指定された Unicode 文字が最初に出現するゼロベースのインデックスを返します。 |
| [indexOf(char value, int startIndex)](#indexOf-char-int-) | この文字列内で指定された Unicode 文字が最初に出現するゼロベースのインデックスを返します。 |
| [indexOf(char value, int startIndex, int count)](#indexOf-char-int-int-) | このインスタンス内で指定された文字が最初に出現するゼロベースのインデックスを返します。 |
| [indexOf(String value)](#indexOf-java.lang.String-) | このインスタンス内で指定された文字列が最初に出現するゼロベースのインデックスを返します。 |
| [indexOf(String value, int startIndex)](#indexOf-java.lang.String-int-) | このインスタンス内で指定された文字列が最初に出現するゼロベースのインデックスを返します。 |
| [indexOf(String value, int startIndex, int count)](#indexOf-java.lang.String-int-int-) | このインスタンス内で指定された文字列が最初に出現するゼロベースのインデックスを返します。 |
| [indexOf(String value, int startIndex, int count, short comparisonType)](#indexOf-java.lang.String-int-int-short-) | 現在のインスタンス内で指定された文字列が最初に出現するゼロベースのインデックスを返します。 |
| [indexOf(String value, short comparisonType)](#indexOf-java.lang.String-short-) | 現在のインスタンス内で指定された文字列が最初に出現するゼロベースのインデックスを返します。 |
| [indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)](#indexOf-Rename-Namesake-java.lang.String-int-short-) | 現在のインスタンス内で指定された文字列が最初に出現するゼロベースのインデックスを返します。 |
| [insert(int startIndex, String value)](#insert-int-java.lang.String-) | このインスタンスの指定されたインデックス位置に指定された文字列を挿入します。 |
| [insert(int startIndex, String value, TextStyle style)](#insert-int-java.lang.String-com.aspose.note.TextStyle-) | このインスタンスの指定されたインデックス位置に、指定されたスタイルを持つ文字列を挿入します。 |
| [iterator()](#iterator--) |  |
| [remove(int startIndex)](#remove-int-) | 現在のインスタンスで、指定された位置から最後の位置までのすべての文字を削除します。 |
| [remove(int startIndex, int count)](#remove-int-int-) | 現在のインスタンスで、指定された位置から指定された数の文字を削除します。 |
| [replace(char oldChar, char newChar)](#replace-char-char-) | このインスタンス内の指定された Unicode 文字のすべての出現を、別の指定された Unicode 文字に置き換えます。 |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | 現在のインスタンス内の指定された文字列のすべての出現を、別の指定された文字列に置き換えます。 |
| [replace(String oldValue, String newValue, TextStyle style)](#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-) | 現在のインスタンス内の指定された文字列のすべての出現を、指定されたスタイルの別の文字列に置き換えます。 |
| [setAlignment(int value)](#setAlignment-int-) | 配置を設定します。 |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 最終更新日時を設定します。 |
| [setLineSpacing(float value)](#setLineSpacing-float-) |  |
| [setLineSpacing(Float value)](#setLineSpacing-java.lang.Float-) | 行間隔を設定します。 |
| [setParagraphStyle(ParagraphStyle value)](#setParagraphStyle-com.aspose.note.ParagraphStyle-) | 段落スタイルを設定します。 |
| [setSpaceAfter(float value)](#setSpaceAfter-float-) |  |
| [setSpaceAfter(Float value)](#setSpaceAfter-java.lang.Float-) | 後ろの最小余白を設定します。 |
| [setSpaceBefore(float value)](#setSpaceBefore-float-) |  |
| [setSpaceBefore(Float value)](#setSpaceBefore-java.lang.Float-) | 前に設定する最小スペース量を設定します。 |
| [setText(String value)](#setText-java.lang.String-) | テキストを設定します。 |
| [trim()](#trim--) | 先頭と末尾のすべての空白文字を削除します。 |
| [trim(char trimChar)](#trim-char-) | 文字の先頭と末尾のすべての出現を削除します。 |
| [trim(char[] trimChars)](#trim-char...-) | 配列で指定された文字セットの先頭と末尾のすべての出現を削除します。 |
| [trimEnd()](#trimEnd--) | 末尾のすべての空白文字を削除します。 |
| [trimEnd(char trimChar)](#trimEnd-char-) | 文字の末尾のすべての出現を削除します。 |
| [trimEnd(char[] trimChars)](#trimEnd-char...-) | 配列で指定された文字セットの末尾のすべての出現を削除します。 |
| [trimStart()](#trimStart--) | 先頭のすべての空白文字を削除します。 |
| [trimStart(char trimChar)](#trimStart-char-) | 指定された文字の先頭のすべての出現を削除します。 |
| [trimStart(char[] trimChars)](#trimStart-char...-) | 配列で指定された文字セットの先頭のすべての出現を削除します。 |
### RichText() {#RichText--}
```
public RichText()
```


[RichText](../../com.aspose.note/richtext) クラスの新しいインスタンスを初期化します。

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


ノードのビジターを受け入れます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | [DocumentVisitor](../../com.aspose.note/documentvisitor) から派生したクラスのオブジェクトです。 |

### append(String value) {#append-java.lang.String-}
```
public RichText append(String value)
```


最後のテキスト範囲に文字列を追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 追加された値です。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### append(String value, TextStyle style) {#append-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText append(String value, TextStyle style)
```


文字列を末尾に追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 追加された値です。 |
| style | [TextStyle](../../com.aspose.note/textstyle) | 追加された文字列のスタイルです。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value) {#appendFront-java.lang.String-}
```
public RichText appendFront(String value)
```


文字列を最初のテキスト範囲の先頭に追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 追加された値です。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value, TextStyle style) {#appendFront-java.lang.String-com.aspose.note.TextStyle-}
```
public RichText appendFront(String value, TextStyle style)
```


文字列を先頭に追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 追加された値です。 |
| style | [TextStyle](../../com.aspose.note/textstyle) | 追加された文字列のスタイルです。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### clear() {#clear--}
```
public final RichText clear()
```


このインスタンスの内容をクリアします。

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


配置を取得します。

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


最終更新時刻を取得します。

**Returns:**
java.util.Date
### getLength() {#getLength--}
```
public final int getLength()
```




**Returns:**
int
### getLineSpacing() {#getLineSpacing--}
```
public Float getLineSpacing()
```


行間隔を取得します。

**Returns:**
java.lang.Float
### getParagraphStyle() {#getParagraphStyle--}
```
public final ParagraphStyle getParagraphStyle()
```


段落スタイルを取得します。これらの設定は、[getStyles](../../com.aspose.note/richtext\#getStyles) コレクションに一致する TextStyle オブジェクトが存在しない場合、またはこのオブジェクトが必要な設定を指定していない場合に使用されます。

**Returns:**
[ParagraphStyle](../../com.aspose.note/paragraphstyle)
### getSpaceAfter() {#getSpaceAfter--}
```
public Float getSpaceAfter()
```


後ろの最小余白を取得します。

**Returns:**
java.lang.Float
### getSpaceBefore() {#getSpaceBefore--}
```
public Float getSpaceBefore()
```


前の最小余白を取得します。

**Returns:**
java.lang.Float
### getStyles() {#getStyles--}
```
public System.Collections.Generic.IGenericEnumerable<TextStyle> getStyles()
```


スタイルを取得します。

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextStyle&gt;
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


段落のすべてのタグの一覧を取得します。

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public final String getText()
```


テキストを取得します。文字列は値 10（改行）の文字を含んではいけません。

**Returns:**
java.lang.String
### getTextRuns() {#getTextRuns--}
```
public final System.Collections.Generic.IGenericEnumerable<TextRun> getTextRuns()
```




**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextRun&gt;
### indexOf(char value) {#indexOf-char-}
```
public final int indexOf(char value)
```


この文字列内で指定された Unicode 文字が最初に出現するゼロベースのインデックスを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | char | 値です。 |

**Returns:**
int - `int`です。
### indexOf(char value, int startIndex) {#indexOf-char-int-}
```
public final int indexOf(char value, int startIndex)
```


この文字列内で指定された Unicode 文字の最初の出現のゼロベースインデックスを返します。検索は指定された文字位置から開始します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | char | 値です。 |
| startIndex | int | 検索開始位置 |

**Returns:**
int - `int`です。
### indexOf(char value, int startIndex, int count) {#indexOf-char-int-int-}
```
public final int indexOf(char value, int startIndex, int count)
```


このインスタンス内で指定された文字の最初の出現のゼロベースインデックスを返します。検索は指定された文字位置から開始し、指定された文字数だけ調べます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | char | 値です。 |
| startIndex | int | 検索開始位置 |
| count | int | カウントです。 |

**Returns:**
int - `int`です。
### indexOf(String value) {#indexOf-java.lang.String-}
```
public final int indexOf(String value)
```


このインスタンス内で指定された文字列が最初に出現するゼロベースのインデックスを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 値です。 |

**Returns:**
int - `int`です。
### indexOf(String value, int startIndex) {#indexOf-java.lang.String-int-}
```
public final int indexOf(String value, int startIndex)
```


このインスタンスで指定された文字列が最初に出現する位置のゼロベースインデックスを返します。検索は指定された文字位置から開始します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 値です。 |
| startIndex | int | 検索開始位置 |

**Returns:**
int - `int`です。
### indexOf(String value, int startIndex, int count) {#indexOf-java.lang.String-int-int-}
```
public final int indexOf(String value, int startIndex, int count)
```


このインスタンスで指定された文字列が最初に出現する位置のゼロベースインデックスを返します。検索は指定された文字位置から開始し、指定された文字数だけ調べます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 値です。 |
| startIndex | int | 検索開始位置 |
| count | int | カウントです。 |

**Returns:**
int - `int`です。
### indexOf(String value, int startIndex, int count, short comparisonType) {#indexOf-java.lang.String-int-int-short-}
```
public final int indexOf(String value, int startIndex, int count, short comparisonType)
```


現在のインスタンス内で指定された文字列が最初に出現するゼロベースのインデックスを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 値です。 |
| startIndex | int | 検索開始位置 |
| count | int | カウントです。 |
| comparisonType | short | 指定された文字列に使用する検索の種類 |

**Returns:**
int - `int`です。
### indexOf(String value, short comparisonType) {#indexOf-java.lang.String-short-}
```
public final int indexOf(String value, short comparisonType)
```


現在のインスタンスで指定された文字列が最初に出現する位置のゼロベースインデックスを返します。パラメータは指定された文字列に使用する検索の種類を指定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 値です。 |
| comparisonType | short | 指定された文字列に使用する検索の種類 |

**Returns:**
int - `int`です。
### indexOf_Rename_Namesake(String value, int startIndex, short comparisonType) {#indexOf-Rename-Namesake-java.lang.String-int-short-}
```
public final int indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)
```


現在のインスタンスで指定された文字列が最初に出現する位置のゼロベースインデックスを返します。パラメータは現在の文字列における検索開始位置と、指定された文字列に使用する検索の種類を指定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | 値です。 |
| startIndex | int | 検索開始位置 |
| comparisonType | short | 指定された文字列に使用する検索の種類 |

**Returns:**
int - `int`です。
### insert(int startIndex, String value) {#insert-int-java.lang.String-}
```
public final RichText insert(int startIndex, String value)
```


このインスタンスの指定されたインデックス位置に指定された文字列を挿入します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| startIndex | int | 開始インデックス。 |
| 値 | java.lang.String | 値です。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### insert(int startIndex, String value, TextStyle style) {#insert-int-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText insert(int startIndex, String value, TextStyle style)
```


このインスタンスの指定されたインデックス位置に、指定されたスタイルを持つ文字列を挿入します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| startIndex | int | 開始インデックス。 |
| 値 | java.lang.String | 値です。 |
| style | [TextStyle](../../com.aspose.note/textstyle) | スタイル。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Character> iterator()
```




**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;java.lang.Character&gt;
### remove(int startIndex) {#remove-int-}
```
public final RichText remove(int startIndex)
```


現在のインスタンスで、指定された位置から最後の位置までのすべての文字を削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| startIndex | int | 開始インデックス。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### remove(int startIndex, int count) {#remove-int-int-}
```
public final RichText remove(int startIndex, int count)
```


現在のインスタンスで、指定された位置から指定された数の文字を削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| startIndex | int | 開始インデックス。 |
| count | int | カウントです。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public final RichText replace(char oldChar, char newChar)
```


このインスタンス内の指定された Unicode 文字のすべての出現を、別の指定された Unicode 文字に置き換えます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| oldChar | char | 古い文字。 |
| newChar | char | 新しい文字。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public final RichText replace(String oldValue, String newValue)
```


現在のインスタンス内の指定された文字列のすべての出現を、別の指定された文字列に置き換えます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| oldValue | java.lang.String | 古い値。 |
| newValue | java.lang.String | 新しい値。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue, TextStyle style) {#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText replace(String oldValue, String newValue, TextStyle style)
```


現在のインスタンス内の指定された文字列のすべての出現を、指定されたスタイルの別の文字列に置き換えます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| oldValue | java.lang.String | 古い値。 |
| newValue | java.lang.String | 新しい値。 |
| style | [TextStyle](../../com.aspose.note/textstyle) | 新しい値のスタイル。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


配置を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


最終更新日時を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date |  |

### setLineSpacing(float value) {#setLineSpacing-float-}
```
public void setLineSpacing(float value)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | float |  |

### setLineSpacing(Float value) {#setLineSpacing-java.lang.Float-}
```
public void setLineSpacing(Float value)
```


行間隔を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.Float |  |

### setParagraphStyle(ParagraphStyle value) {#setParagraphStyle-com.aspose.note.ParagraphStyle-}
```
public final void setParagraphStyle(ParagraphStyle value)
```


段落のスタイルを設定します。これらの設定は、[getStyles](../../com.aspose.note/richtext\#getStyles) コレクションに一致する TextStyle オブジェクトが存在しない場合、またはこのオブジェクトが必要な設定を指定していない場合に使用されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [ParagraphStyle](../../com.aspose.note/paragraphstyle) |  |

### setSpaceAfter(float value) {#setSpaceAfter-float-}
```
public void setSpaceAfter(float value)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | float |  |

### setSpaceAfter(Float value) {#setSpaceAfter-java.lang.Float-}
```
public void setSpaceAfter(Float value)
```


後ろの最小余白を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.Float |  |

### setSpaceBefore(float value) {#setSpaceBefore-float-}
```
public void setSpaceBefore(float value)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | float |  |

### setSpaceBefore(Float value) {#setSpaceBefore-java.lang.Float-}
```
public void setSpaceBefore(Float value)
```


前に設定する最小スペース量を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.Float |  |

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


テキストを設定します。文字列は値10（改行）に相当する文字を含んではいけません。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String |  |

### trim() {#trim--}
```
public final RichText trim()
```


先頭と末尾のすべての空白文字を削除します。

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char trimChar) {#trim-char-}
```
public final RichText trim(char trimChar)
```


文字の先頭と末尾のすべての出現を削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| trimChar | char | トリム文字。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char[] trimChars) {#trim-char...-}
```
public final RichText trim(char[] trimChars)
```


配列で指定された文字セットの先頭と末尾のすべての出現を削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| trimChars | char[] | トリム文字です。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd() {#trimEnd--}
```
public final RichText trimEnd()
```


末尾のすべての空白文字を削除します。

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char trimChar) {#trimEnd-char-}
```
public final RichText trimEnd(char trimChar)
```


文字の末尾のすべての出現を削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| trimChar | char | トリム文字。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char[] trimChars) {#trimEnd-char...-}
```
public final RichText trimEnd(char[] trimChars)
```


配列で指定された文字セットの末尾のすべての出現を削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| trimChars | char[] | トリム文字です。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart() {#trimStart--}
```
public final RichText trimStart()
```


先頭のすべての空白文字を削除します。

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char trimChar) {#trimStart-char-}
```
public final RichText trimStart(char trimChar)
```


指定された文字の先頭のすべての出現を削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| trimChar | char | トリム文字。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char[] trimChars) {#trimStart-char...-}
```
public final RichText trimStart(char[] trimChars)
```


配列で指定された文字セットの先頭のすべての出現を削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| trimChars | char[] | トリム文字です。 |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
