---
title: "NotebookLoadOptions"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "노트북을 로드하는 데 사용되는 옵션입니다."
type: docs
weight: 58
url: /ko/java/com.aspose.note/notebookloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class NotebookLoadOptions
```

노트북을 로드하는 데 사용되는 옵션입니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [NotebookLoadOptions()](#NotebookLoadOptions--) | 새 `NotebookLoadOptions` 클래스의 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getDeferredLoading()](#getDeferredLoading--) | 자식 문서를 나중에 명시적으로 로드해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [getInstantLoading()](#getInstantLoading--) | 부모 문서가 로드되는 동안 자식 문서를 로드해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [setDeferredLoading(boolean value)](#setDeferredLoading-boolean-) | 자식 문서를 나중에 명시적으로 로드해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [setInstantLoading(boolean value)](#setInstantLoading-boolean-) | 부모 문서가 로드되는 동안 자식 문서를 로드해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. |
### NotebookLoadOptions() {#NotebookLoadOptions--}
```
public NotebookLoadOptions()
```


새 `NotebookLoadOptions` 클래스의 인스턴스를 초기화합니다.

### getDeferredLoading() {#getDeferredLoading--}
```
public final boolean getDeferredLoading()
```


자식 문서를 나중에 명시적으로 로드해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다.

--------------------

기본값은 `false`이며, 따라서 하위 문서는 암시적으로 로드됩니다. 값 `true`는 사용자가 `Notebook.loadChildDocument`를 호출하거나 노트북 자체가 로드된 후 각 노트북의 하위 노드를 호출해야 함을 나타냅니다. 값이 `true`이면 `NotebookLoadOptions.instantLoading` 옵션은 무시됩니다. 노트북이 스트림에서 로드되는 경우, 값은 사용자가 `false`로 명시적으로 설정했더라도 항상 `true`입니다.

**Returns:**
boolean
### getInstantLoading() {#getInstantLoading--}
```
public boolean getInstantLoading()
```


부모 문서가 로드되는 동안 자식 문서를 로드해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다.

--------------------

기본값은 `false`이며, 하위 문서는 지연 로드됩니다. 즉, 특정 하위 항목에 직접 접근할 때까지 로드를 연기해야 합니다. 값 `true`는 로드를 즉시 수행해야 함을 나타냅니다.

**Returns:**
boolean
### setDeferredLoading(boolean value) {#setDeferredLoading-boolean-}
```
public final void setDeferredLoading(boolean value)
```


자식 문서를 나중에 명시적으로 로드해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다.

--------------------

기본값은 `false`이며, 따라서 하위 문서는 암시적으로 로드됩니다. 값 `true`는 사용자가 `Notebook.loadChildDocument`를 호출하거나 노트북 자체가 로드된 후 각 노트북의 하위 노드를 호출해야 함을 나타냅니다. 값이 `true`이면 `NotebookLoadOptions.instantLoading` 옵션은 무시됩니다. 노트북이 스트림에서 로드되는 경우, 값은 사용자가 `false`로 명시적으로 설정했더라도 항상 `true`입니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean |  |

### setInstantLoading(boolean value) {#setInstantLoading-boolean-}
```
public void setInstantLoading(boolean value)
```


부모 문서가 로드되는 동안 자식 문서를 로드해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다.

--------------------

기본값은 `false`이며, 하위 문서는 지연 로드됩니다. 즉, 특정 하위 항목에 직접 접근할 때까지 로드를 연기해야 합니다. 값 `true`는 로드를 즉시 수행해야 함을 나타냅니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean |  |

