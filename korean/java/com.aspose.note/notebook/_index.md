---
title: "노트북"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "Aspose.Note 노트북을 나타냅니다."
type: docs
weight: 56
url: /ko/java/com.aspose.note/notebook/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class Notebook implements INotebookChildNode, System.Collections.Generic.IGenericEnumerable<INotebookChildNode>
```

Aspose.Note 노트북을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Notebook()](#Notebook--) | `Notebook` 클래스의 새 인스턴스를 초기화합니다. |
| [Notebook(String filePath)](#Notebook-java.lang.String-) | `Notebook` 클래스의 새 인스턴스를 초기화합니다. |
| [Notebook(String filePath, NotebookLoadOptions loadOptions)](#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | `Notebook` 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | 노드 유형별로 모든 자식 노드를 가져옵니다. |
| [appendChild(INotebookChildNode newChild)](#appendChild-com.aspose.note.INotebookChildNode-) | 노드를 목록 끝에 추가합니다. |
| [getColor()](#getColor--) | 색상을 가져오거나 설정합니다. |
| [getCount()](#getCount--) | `Notebook`에 포함된 요소 수를 가져옵니다. |
| [getDisplayName()](#getDisplayName--) | 표시 이름을 가져오거나 설정합니다. |
| [getFileFormat()](#getFileFormat--) | 파일 형식을 가져옵니다 (OneNote 2010, OneNote Online). |
| [getGuid()](#getGuid--) | 객체의 전역 고유 ID를 가져옵니다. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [get_Item(int index)](#get-Item-int-) | 지정된 인덱스로 노트북 자식 노드를 가져옵니다. |
| [isHistoryEnabled()](#isHistoryEnabled--) | 히스토리가 활성화되어 있는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [iterator()](#iterator--) | `Notebook`의 자식 노드를 순회하는 열거자를 반환합니다. |
| [loadChildDocument(InputStream stream)](#loadChildDocument-java.io.InputStream-) | 자식 문서 노드를 추가합니다. |
| [loadChildDocument(InputStream stream, LoadOptions loadOptions)](#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-) | 자식 문서 노드를 추가합니다. |
| [loadChildDocument(String filePath)](#loadChildDocument-java.lang.String-) | 자식 문서 노드를 추가합니다. |
| [loadChildDocument(String filePath, LoadOptions loadOptions)](#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-) | 자식 문서 노드를 추가합니다. |
| [loadChildNotebook(String filePath)](#loadChildNotebook-java.lang.String-) | 자식 노트북 노드를 추가합니다. |
| [loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)](#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | 자식 노트북 노드를 추가합니다. |
| [removeChild(INotebookChildNode oldChild)](#removeChild-com.aspose.note.INotebookChildNode-) | 자식 노드를 제거합니다. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | OneNote 문서를 스트림에 저장합니다. |
| [save(OutputStream stream, NotebookSaveOptions options)](#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-) | 지정된 저장 옵션을 사용하여 OneNote 문서를 스트림에 저장합니다. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | 지정된 형식으로 OneNote 문서를 스트림에 저장합니다. |
| [save(String fileName)](#save-java.lang.String-) | OneNote 문서를 파일에 저장합니다. |
| [save(String fileName, NotebookSaveOptions options)](#save-java.lang.String-com.aspose.note.NotebookSaveOptions-) | 지정된 저장 옵션을 사용하여 OneNote 문서를 파일에 저장합니다. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | 지정된 형식으로 OneNote 문서를 파일에 저장합니다. |
| [setColor(Color value)](#setColor-java.awt.Color-) | 색상을 가져오거나 설정합니다. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | 표시 이름을 가져오거나 설정합니다. |
| [setHistoryEnabled(boolean value)](#setHistoryEnabled-boolean-) | 히스토리가 활성화되어 있는지 여부를 나타내는 값을 가져오거나 설정합니다. |
### Notebook() {#Notebook--}
```
public Notebook()
```


`Notebook` 클래스의 새 인스턴스를 초기화합니다.

### Notebook(String filePath) {#Notebook-java.lang.String-}
```
public Notebook(String filePath)
```


`Notebook` 클래스의 새 인스턴스를 초기화합니다. 파일에서 기존 OneNote 노트북을 엽니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | java.lang.String | 파일 경로. |

### Notebook(String filePath, NotebookLoadOptions loadOptions) {#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public Notebook(String filePath, NotebookLoadOptions loadOptions)
```


새 `Notebook` 클래스의 인스턴스를 초기화합니다. 파일에서 기존 OneNote 노트북을 엽니다. "lazy"/instant와 같은 추가 옵션을 지정할 수 있습니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | java.lang.String | 파일 경로. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | 로드 옵션입니다. |

### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


노드 유형별로 모든 자식 노드를 가져옵니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - 자식 노드의 목록입니다.

`T1`: 반환된 목록에 있는 요소의 유형입니다.
### appendChild(INotebookChildNode newChild) {#appendChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode appendChild(INotebookChildNode newChild)
```


노드를 목록 끝에 추가합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| newChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | 추가할 노드입니다. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The added node.
### getColor() {#getColor--}
```
public Color getColor()
```


색상을 가져오거나 설정합니다.

**Returns:**
java.awt.Color
### getCount() {#getCount--}
```
public int getCount()
```


`Notebook`에 포함된 요소 수를 가져옵니다.

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


표시 이름을 가져오거나 설정합니다.

**Returns:**
java.lang.String
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


파일 형식을 가져옵니다 (OneNote 2010, OneNote Online).

**Returns:**
int
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


객체의 전역 고유 ID를 가져옵니다.

값: GUID입니다.

**Returns:**
java.util.UUID
### getGuidInternal() {#getGuidInternal--}
```
public System.Guid getGuidInternal()
```




**Returns:**
com.aspose.ms.System.Guid
### get_Item(int index) {#get-Item-int-}
```
public INotebookChildNode get_Item(int index)
```


지정된 인덱스로 노트북 자식 노드를 가져옵니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| index | int | 자식 노드의 인덱스입니다. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The child node on the `index` position.
### isHistoryEnabled() {#isHistoryEnabled--}
```
public boolean isHistoryEnabled()
```


히스토리가 활성화되어 있는지 여부를 나타내는 값을 가져오거나 설정합니다.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<INotebookChildNode> iterator()
```


`Notebook`의 자식 노드를 순회하는 열거자를 반환합니다.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.INotebookChildNode&gt; - `IEnumerator`입니다.
### loadChildDocument(InputStream stream) {#loadChildDocument-java.io.InputStream-}
```
public void loadChildDocument(InputStream stream)
```


자식 문서 노드를 추가합니다. 스트림에서 기존 OneNote 문서를 엽니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.InputStream | 스트림입니다. |

### loadChildDocument(InputStream stream, LoadOptions loadOptions) {#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(InputStream stream, LoadOptions loadOptions)
```


자식 문서 노드를 추가합니다. 스트림에서 기존 OneNote 문서를 엽니다. 추가 로드 옵션을 지정할 수 있습니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.InputStream | 스트림입니다. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | 로드 옵션입니다. |

### loadChildDocument(String filePath) {#loadChildDocument-java.lang.String-}
```
public void loadChildDocument(String filePath)
```


자식 문서 노드를 추가합니다. 파일에서 기존 OneNote 문서를 엽니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | java.lang.String | 파일 경로. |

### loadChildDocument(String filePath, LoadOptions loadOptions) {#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(String filePath, LoadOptions loadOptions)
```


자식 문서 노드를 추가합니다. 파일에서 기존 OneNote 문서를 엽니다. 추가 로드 옵션을 지정할 수 있습니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | java.lang.String | 파일 경로. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | 로드 옵션입니다. |

### loadChildNotebook(String filePath) {#loadChildNotebook-java.lang.String-}
```
public void loadChildNotebook(String filePath)
```


자식 노트북 노드를 추가합니다. 파일에서 기존 OneNote 노트북을 엽니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | java.lang.String | 파일 경로. |

### loadChildNotebook(String filePath, NotebookLoadOptions loadOptions) {#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public void loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)
```


자식 노트북 노드를 추가합니다. 파일에서 기존 OneNote 노트북을 엽니다. 추가 로드 옵션을 지정할 수 있습니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | java.lang.String | 파일 경로. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | 로드 옵션입니다. |

### removeChild(INotebookChildNode oldChild) {#removeChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode removeChild(INotebookChildNode oldChild)
```


자식 노드를 제거합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| oldChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | 제거할 노드입니다. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The removed node.
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


OneNote 문서를 스트림에 저장합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.OutputStream | 스트림입니다. |

### save(OutputStream stream, NotebookSaveOptions options) {#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-}
```
public void save(OutputStream stream, NotebookSaveOptions options)
```


지정된 저장 옵션을 사용하여 OneNote 문서를 스트림에 저장합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.OutputStream | 스트림입니다. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | 문서를 저장하는 옵션을 지정합니다. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


지정된 형식으로 OneNote 문서를 스트림에 저장합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.OutputStream | 스트림입니다. |
| format | int | 문서를 저장할 형식. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


OneNote 문서를 파일에 저장합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 파일이름 | java.lang.String | 파일의 전체 이름입니다. 지정된 전체 이름을 가진 파일이 이미 존재하면 기존 파일이 덮어쓰기됩니다. |

### save(String fileName, NotebookSaveOptions options) {#save-java.lang.String-com.aspose.note.NotebookSaveOptions-}
```
public void save(String fileName, NotebookSaveOptions options)
```


지정된 저장 옵션을 사용하여 OneNote 문서를 파일에 저장합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 파일이름 | java.lang.String | 파일의 전체 이름입니다. 지정된 전체 이름을 가진 파일이 이미 존재하면 기존 파일이 덮어쓰기됩니다. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | 문서가 파일에 저장되는 옵션을 지정합니다. |

### save(String fileName, int format) {#save-java.lang.String-int-}
```
public void save(String fileName, int format)
```


지정된 형식으로 OneNote 문서를 파일에 저장합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 파일이름 | java.lang.String | 파일의 전체 이름입니다. 지정된 전체 이름을 가진 파일이 이미 존재하면 기존 파일이 덮어쓰기됩니다. |
| format | int | 문서를 저장할 형식. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


색상을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.awt.Color |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


표시 이름을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String |  |

### setHistoryEnabled(boolean value) {#setHistoryEnabled-boolean-}
```
public void setHistoryEnabled(boolean value)
```


히스토리가 활성화되어 있는지 여부를 나타내는 값을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean |  |

