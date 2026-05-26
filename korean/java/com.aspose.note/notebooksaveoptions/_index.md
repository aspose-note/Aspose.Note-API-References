---
title: "NotebookSaveOptions"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "특정 형식에 대한 노트북 저장 옵션을 나타내는 추상 기본 클래스입니다."
type: docs
weight: 61
url: /ko/java/com.aspose.note/notebooksaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class NotebookSaveOptions
```

특정 형식에 대한 노트북 저장 옵션을 나타내는 추상 기본 클래스입니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getDeferredSaving()](#getDeferredSaving--) | 자식 문서를 명시적으로 저장해야 하는지를 나타내는 값을 가져오거나 설정합니다. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | 노트북의 모든 자식 문서에 대한 저장 옵션을 가져옵니다. |
| [getFlatten()](#getFlatten--) | 노트북 자식 계층 구조가 평탄화되어 저장되는지를 나타내는 값을 가져오거나 설정합니다. |
| [getSaveFormat()](#getSaveFormat--) | 노트북이 저장되는 형식을 가져옵니다. |
| [setDeferredSaving(boolean value)](#setDeferredSaving-boolean-) | 자식 문서를 명시적으로 저장해야 하는지를 나타내는 값을 가져오거나 설정합니다. |
| [setFlatten(boolean value)](#setFlatten-boolean-) | 노트북 자식 계층 구조가 평탄화되어 저장되는지를 나타내는 값을 가져오거나 설정합니다. |
### getDeferredSaving() {#getDeferredSaving--}
```
public boolean getDeferredSaving()
```


자식 문서를 명시적으로 저장해야 하는지를 나타내는 값을 가져오거나 설정합니다.

--------------------

기본값은 `false`이며, 따라서 하위 문서는 암시적으로 저장됩니다. `true` 값은 사용자가 각 노트북의 하위 노드를 명시적으로 저장해야 함을 나타냅니다. 노트북을 스트림에 저장하는 경우, 사용자가 `false`로 명시적으로 설정했더라도 값은 항상 `true`입니다.

**Returns:**
boolean
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public abstract SaveOptions getDocumentSaveOptionsInternal()
```


노트북의 모든 자식 문서에 대한 저장 옵션을 가져옵니다.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getFlatten() {#getFlatten--}
```
public boolean getFlatten()
```


노트북 자식 계층 구조가 평탄화되어 저장되는지를 나타내는 값을 가져오거나 설정합니다.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public abstract int getSaveFormat()
```


노트북이 저장되는 형식을 가져옵니다.

**Returns:**
int
### setDeferredSaving(boolean value) {#setDeferredSaving-boolean-}
```
public void setDeferredSaving(boolean value)
```


자식 문서를 명시적으로 저장해야 하는지를 나타내는 값을 가져오거나 설정합니다.

--------------------

기본값은 `false`이며, 따라서 하위 문서는 암시적으로 저장됩니다. `true` 값은 사용자가 각 노트북의 하위 노드를 명시적으로 저장해야 함을 나타냅니다. 노트북을 스트림에 저장하는 경우, 사용자가 `false`로 명시적으로 설정했더라도 값은 항상 `true`입니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean |  |

### setFlatten(boolean value) {#setFlatten-boolean-}
```
public void setFlatten(boolean value)
```


노트북 자식 계층 구조가 평탄화되어 저장되는지를 나타내는 값을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean |  |

