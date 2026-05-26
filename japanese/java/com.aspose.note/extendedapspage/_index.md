---
title: "ExtendedApsPage"
second_title: "Aspose.Note for Java API リファレンス"
description: "標準の ApsGlyphs のラッパーを表し、描画動作の一部を拡張します。"
type: docs
weight: 27
url: /ja/java/com.aspose.note/extendedapspage/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode, com.aspose.foundation.rendering.ApsCompositeNode, com.aspose.foundation.rendering.ApsPage

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsPage extends ApsPage implements System.Collections.Generic.IGenericEnumerable<ApsNode>
```

標準 ApsGlyphs のラッパーを表し、描画動作の一部を拡張します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)](#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-) | `ExtendedApsPage` クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getContentSize()](#getContentSize--) | 余白を除いたページサイズを取得します。 |
| [getMargin()](#getMargin--) | このページの余白を取得します。 |
| [getPageEndInNotePage()](#getPageEndInNotePage--) | MS OneNote ページが複数の aps ページに分割される場合、MS OneNote ページ内でのページ末端の位置を取得します。 |
| [getPageSize()](#getPageSize--) | 最終的なページサイズを取得します。 |
| [getPageStartInNotePage()](#getPageStartInNotePage--) | MS OneNote ページが複数の aps ページに分割される場合、MS OneNote ページ内でのページ開始位置を取得します。 |
| [iterator()](#iterator--) | このページのすべてのノードを反復処理する列挙子を返します。 |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) | 取得列挙子です。 |
### ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin) {#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-}
```
public ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)
```


`ExtendedApsPage` クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| pageSize | com.aspose.ms.System.Drawing.SizeF | ページサイズです。 |
| pageStartInNotePage | float | 元の MS OneNote ページでのページ開始位置です。 |
| margin | com.aspose.foundation.layout.Margin | 拡張されたページ余白。 |

### getContentSize() {#getContentSize--}
```
public System.Drawing.SizeF getContentSize()
```


余白を除いたページサイズを取得します。

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getMargin() {#getMargin--}
```
public Margin getMargin()
```


このページの余白を取得します。

**Returns:**
com.aspose.foundation.layout.Margin
### getPageEndInNotePage() {#getPageEndInNotePage--}
```
public float getPageEndInNotePage()
```


MS OneNote ページが複数の aps ページに分割される場合、MS OneNote ページ内でのページ末端の位置を取得します。

**Returns:**
float
### getPageSize() {#getPageSize--}
```
public System.Drawing.SizeF getPageSize()
```


最終的なページサイズを取得します。

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getPageStartInNotePage() {#getPageStartInNotePage--}
```
public float getPageStartInNotePage()
```


MS OneNote ページが複数の aps ページに分割される場合、MS OneNote ページ内でのページ開始位置を取得します。

**Returns:**
float
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsNode> iterator()
```


このページのすべてのノードを反復処理する列挙子を返します。

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsNode&gt; - この `IEnumerator`。
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```


取得列挙子です。

**Returns:**
com.aspose.ms.System.Collections.IEnumerator - この `IEnumerator`。
