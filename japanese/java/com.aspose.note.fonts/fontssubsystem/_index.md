---
title: "FontsSubsystem"
second_title: "Aspose.Note for Java API リファレンス"
description: "com.aspose.note.IFontsSubsystem インターフェイスを実装する基底クラスです。"
type: docs
weight: 11
url: /ja/java/com.aspose.note.fonts/fontssubsystem/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.fonts.IFontsSubsystem](../../com.aspose.note.fonts/ifontssubsystem)
```
public abstract class FontsSubsystem implements IFontsSubsystem
```

com.aspose.note.IFontsSubsystem インターフェイスを実装する基底クラス。デフォルトフォントとフォントの置換機能を提供します。派生クラスで com.aspose.note.FontsSubsystem.fetchFontFamily の protected メンバー関数をオーバーライドして、Font オブジェクトの取得ロジックを実装します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [addFont(InputStream stream)](#addFont-java.io.InputStream-) | フォントを追加します。 |
| [addFont(String file)](#addFont-java.lang.String-) | フォントを追加します。 |
| [addFontSubstitution(String substituted, String substitution)](#addFontSubstitution-java.lang.String-java.lang.String-) | フォントの置換を追加します。 |
| [getDefaultFont()](#getDefaultFont--) | デフォルトフォントを取得します。 |
| [getFontFamily(String fontName)](#getFontFamily-java.lang.String-) | フォントを取得します。 |
| [loadFontsFromFolder(String folder)](#loadFontsFromFolder-java.lang.String-) | 指定されたフォルダーからすべての TrueType フォントを内部コレクションにロードします。 |
### addFont(InputStream stream) {#addFont-java.io.InputStream-}
```
public final void addFont(InputStream stream)
```


フォントを追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.InputStream | フォントを含むストリームです。 |

### addFont(String file) {#addFont-java.lang.String-}
```
public final void addFont(String file)
```


フォントを追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ファイル | java.lang.String | フォントを含むファイルへのパスです。 |

### addFontSubstitution(String substituted, String substitution) {#addFontSubstitution-java.lang.String-java.lang.String-}
```
public final void addFontSubstitution(String substituted, String substitution)
```


フォントの置換を追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 置換された | java.lang.String | 置換されたフォント名です。 |
| 置換 | java.lang.String | 置換フォント名です。 |

### getDefaultFont() {#getDefaultFont--}
```
public Font getDefaultFont()
```


デフォルトフォントを取得します。

**Returns:**
java.awt.Font
### getFontFamily(String fontName) {#getFontFamily-java.lang.String-}
```
public Font getFontFamily(String fontName)
```


フォントを取得します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fontName | java.lang.String | フォント名です。 |

**Returns:**
java.awt.Font - フォントです。
### loadFontsFromFolder(String folder) {#loadFontsFromFolder-java.lang.String-}
```
public final void loadFontsFromFolder(String folder)
```


指定されたフォルダーからすべての TrueType フォントを内部コレクションにロードします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| フォルダー | java.lang.String | フォントを含むフォルダーです。 |

