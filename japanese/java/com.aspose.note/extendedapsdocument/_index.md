---
title: "ExtendedApsDocument"
second_title: "Aspose.Note for Java API リファレンス"
description: "ページから構成されページセットに変換された、完全なワンノートドキュメントを表します。"
type: docs
weight: 23
url: /ja/java/com.aspose.note/extendedapsdocument/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsDocument extends ApsNode implements System.Collections.Generic.IGenericEnumerable<ApsPage>
```

ページをページセットに変換して構成された完全な OneNote ドキュメントを表します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [ExtendedApsDocument()](#ExtendedApsDocument--) | 新しい `ExtendedApsDocument` クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [accept(ApsDocumentVisitor visitor)](#accept-com.aspose.foundation.rendering.ApsDocumentVisitor-) | この要素に ApsDocumentVisitor を受け入れます。 |
| [addPage(ApsPage page)](#addPage-com.aspose.foundation.rendering.ApsPage-) | ドキュメントにページセットを追加します。 |
| [getPageList()](#getPageList--) | ページセットのリストを取得します。 |
| [iterator()](#iterator--) | 列挙子を返します。 |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) |  |
### ExtendedApsDocument() {#ExtendedApsDocument--}
```
public ExtendedApsDocument()
```


新しい `ExtendedApsDocument` クラスのインスタンスを初期化します。

### accept(ApsDocumentVisitor visitor) {#accept-com.aspose.foundation.rendering.ApsDocumentVisitor-}
```
public void accept(ApsDocumentVisitor visitor)
```


この要素に ApsDocumentVisitor を受け入れます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ビジター | com.aspose.foundation.rendering.ApsDocumentVisitor | ビジターです。 |

### addPage(ApsPage page) {#addPage-com.aspose.foundation.rendering.ApsPage-}
```
public void addPage(ApsPage page)
```


ドキュメントにページセットを追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ページ | com.aspose.foundation.rendering.ApsPage | ページセットです。 |

### getPageList() {#getPageList--}
```
public System.Collections.Generic.List<ApsPage> getPageList()
```


ページセットのリストを取得します。

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.foundation.rendering.ApsPage&gt;
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsPage> iterator()
```


列挙子を返します。

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsPage&gt;
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```




**Returns:**
com.aspose.ms.System.Collections.IEnumerator
