---
title: "SaveOptions"
second_title: "Aspose.Note for Java API リファレンス"
description: "特定の形式に対するドキュメント保存オプションを表す抽象基底クラスです。"
type: docs
weight: 85
url: /ja/java/com.aspose.note/saveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SaveOptions
```

特定の形式に対するドキュメント保存オプションを表す抽象基底クラスです。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getFontsSubsystem()](#getFontsSubsystem--) | 保存時に使用されるフォント設定を取得または設定します |
| [getPageCount()](#getPageCount--) | 保存するページ数を取得または設定します。 |
| [getPageIndex()](#getPageIndex--) | 保存する最初のページのインデックスを取得または設定します。 |
| [getSaveFormat()](#getSaveFormat--) | ドキュメントが保存される形式を取得または設定します。 |
| [setFontsSubsystem(FontsSubsystem value)](#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-) | 保存時に使用されるフォント設定を取得または設定します |
| [setPageCount(int value)](#setPageCount-int-) | 保存するページ数を取得または設定します。 |
| [setPageIndex(int value)](#setPageIndex-int-) | 保存する最初のページのインデックスを取得または設定します。 |
### getFontsSubsystem() {#getFontsSubsystem--}
```
public final FontsSubsystem getFontsSubsystem()
```


保存時に使用されるフォント設定を取得または設定します

**Returns:**
[FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


保存するページ数を取得または設定します。デフォルトは \{@link int\#Int32Extensions.MaxValue\} で、これはドキュメントのすべてのページがレンダリングされることを意味します。

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


保存する最初のページのインデックスを取得または設定します。デフォルトは 0 です。

**Returns:**
int
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


ドキュメントが保存される形式を取得または設定します。

**Returns:**
int
### setFontsSubsystem(FontsSubsystem value) {#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-}
```
public final void setFontsSubsystem(FontsSubsystem value)
```


保存時に使用されるフォント設定を取得または設定します

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem) |  |

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


保存するページ数を取得または設定します。デフォルトは \{@link int\#Int32Extensions.MaxValue\} で、これはドキュメントのすべてのページがレンダリングされることを意味します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


保存する最初のページのインデックスを取得または設定します。デフォルトは 0 です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int |  |

