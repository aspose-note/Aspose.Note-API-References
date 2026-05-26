---
title: "NotebookSaveOptionsGeneric"
second_title: "Aspose.Note for Java API リファレンス"
description: "特定の形式向けのノートブック保存オプションを表し、すべてのドキュメント子ノードに共通の保存オプションを提供する抽象基底クラスです。"
type: docs
weight: 62
url: /ja/java/com.aspose.note/notebooksaveoptionsgeneric/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions)
```
public abstract class NotebookSaveOptionsGeneric<TDocumentSaveOptions> extends NotebookSaveOptions
```

特定の形式向けのノートブック保存オプションを表し、すべてのドキュメント子ノードに共通の保存オプションを提供する抽象基底クラスです。

`TDocumentSaveOptions`: すべてのノートブックの子ドキュメントの保存オプションです。

TDocumentSaveOptions :
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [NotebookSaveOptionsGeneric()](#NotebookSaveOptionsGeneric--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getDocumentSaveOptions()](#getDocumentSaveOptions--) | すべてのノートブックの子ドキュメントの保存オプションを取得または設定します。 |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | ノートブックのすべての子ドキュメントの保存オプションを取得します。 |
| [getSaveFormat()](#getSaveFormat--) | ノートブックが保存される形式を取得します。 |
### NotebookSaveOptionsGeneric() {#NotebookSaveOptionsGeneric--}
```
public NotebookSaveOptionsGeneric()
```


### getDocumentSaveOptions() {#getDocumentSaveOptions--}
```
public TDocumentSaveOptions getDocumentSaveOptions()
```


すべてのノートブックの子ドキュメントの保存オプションを取得または設定します。

**Returns:**
TDocumentSaveOptions
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public SaveOptions getDocumentSaveOptionsInternal()
```


ノートブックのすべての子ドキュメントの保存オプションを取得します。

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


ノートブックが保存される形式を取得します。

**Returns:**
int
