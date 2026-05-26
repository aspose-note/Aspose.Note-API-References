---
title: "NotebookSaveOptionsGeneric"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "특정 형식에 대한 노트북 저장 옵션을 나타내고 모든 문서 하위 노드에 대한 공통 저장 옵션을 제공하는 추상 기본 클래스입니다."
type: docs
weight: 62
url: /ko/java/com.aspose.note/notebooksaveoptionsgeneric/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions)
```
public abstract class NotebookSaveOptionsGeneric<TDocumentSaveOptions> extends NotebookSaveOptions
```

특정 형식에 대한 노트북 저장 옵션을 나타내고 모든 문서 하위 노드에 대한 공통 저장 옵션을 제공하는 추상 기본 클래스입니다.

`TDocumentSaveOptions`: 모든 노트북의 하위 문서에 대한 저장 옵션입니다.

TDocumentSaveOptions :
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [NotebookSaveOptionsGeneric()](#NotebookSaveOptionsGeneric--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getDocumentSaveOptions()](#getDocumentSaveOptions--) | 모든 노트북 하위 문서에 대한 저장 옵션을 가져오거나 설정합니다. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | 노트북의 모든 자식 문서에 대한 저장 옵션을 가져옵니다. |
| [getSaveFormat()](#getSaveFormat--) | 노트북이 저장되는 형식을 가져옵니다. |
### NotebookSaveOptionsGeneric() {#NotebookSaveOptionsGeneric--}
```
public NotebookSaveOptionsGeneric()
```


### getDocumentSaveOptions() {#getDocumentSaveOptions--}
```
public TDocumentSaveOptions getDocumentSaveOptions()
```


모든 노트북 하위 문서에 대한 저장 옵션을 가져오거나 설정합니다.

**Returns:**
TDocumentSaveOptions
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public SaveOptions getDocumentSaveOptionsInternal()
```


노트북의 모든 자식 문서에 대한 저장 옵션을 가져옵니다.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


노트북이 저장되는 형식을 가져옵니다.

**Returns:**
int
