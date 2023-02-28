---
title: Notebook.Save
second_title: .NET API 참조용 Aspose.Note
description: Notebook 방법. OneNote 문서를 파일에 저장합니다.
type: docs
weight: 150
url: /ko/net/aspose.note/notebook/save/
---
## Save(string) {#save_3}

OneNote 문서를 파일에 저장합니다.

```csharp
public void Save(string fileName)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| fileName | String | 파일의 전체 이름입니다. 지정된 전체 이름을 가진 파일이 이미 존재하는 경우 기존 파일을 덮어씁니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 문서 구조가 사양을 위반합니다. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 요청한 저장 형식이 지원되지 않습니다. |

### 또한보십시오

* class [Notebook](../)
* 네임스페이스 [Aspose.Note](../../notebook/)
* 집회 [Aspose.Note](../../../)

---

## Save(Stream) {#save}

OneNote 문서를 스트림에 저장합니다.

```csharp
public void Save(Stream stream)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| stream | Stream | 스트림. |

### 예외

| 예외 | 상태 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 문서 구조가 사양을 위반합니다. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 요청한 저장 형식이 지원되지 않습니다. |

### 또한보십시오

* class [Notebook](../)
* 네임스페이스 [Aspose.Note](../../notebook/)
* 집회 [Aspose.Note](../../../)

---

## Save(string, SaveFormat) {#save_4}

OneNote 문서를 지정된 형식의 파일로 저장합니다.

```csharp
public void Save(string fileName, SaveFormat format)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| fileName | String | 파일의 전체 이름입니다. 지정된 전체 이름을 가진 파일이 이미 존재하는 경우 기존 파일을 덮어씁니다. |
| format | SaveFormat | 문서를 저장할 형식입니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 문서 구조가 사양을 위반합니다. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 요청한 저장 형식이 지원되지 않습니다. |

### 또한보십시오

* enum [SaveFormat](../../saveformat/)
* class [Notebook](../)
* 네임스페이스 [Aspose.Note](../../notebook/)
* 집회 [Aspose.Note](../../../)

---

## Save(Stream, SaveFormat) {#save_1}

OneNote 문서를 지정된 형식의 스트림에 저장합니다.

```csharp
public void Save(Stream stream, SaveFormat format)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| stream | Stream | 스트림. |
| format | SaveFormat | 문서를 저장할 형식입니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 문서 구조가 사양을 위반합니다. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 요청한 저장 형식이 지원되지 않습니다. |

### 또한보십시오

* enum [SaveFormat](../../saveformat/)
* class [Notebook](../)
* 네임스페이스 [Aspose.Note](../../notebook/)
* 집회 [Aspose.Note](../../../)

---

## Save(string, NotebookSaveOptions) {#save_5}

지정된 저장 옵션을 사용하여 OneNote 문서를 파일로 저장합니다.

```csharp
public void Save(string fileName, NotebookSaveOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| fileName | String | 파일의 전체 이름입니다. 지정된 전체 이름을 가진 파일이 이미 존재하는 경우 기존 파일을 덮어씁니다. |
| options | NotebookSaveOptions | 문서가 파일에 저장되는 옵션을 지정합니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 문서 구조가 사양을 위반합니다. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 요청한 저장 형식이 지원되지 않습니다. |

### 또한보십시오

* class [NotebookSaveOptions](../../../aspose.note.saving/notebooksaveoptions/)
* class [Notebook](../)
* 네임스페이스 [Aspose.Note](../../notebook/)
* 집회 [Aspose.Note](../../../)

---

## Save(Stream, NotebookSaveOptions) {#save_2}

지정된 저장 옵션을 사용하여 OneNote 문서를 스트림에 저장합니다.

```csharp
public void Save(Stream stream, NotebookSaveOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| stream | Stream | 스트림. |
| options | NotebookSaveOptions | 문서 저장 방법 옵션을 지정합니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 문서 구조가 사양을 위반합니다. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 요청한 저장 형식이 지원되지 않습니다. |

### 또한보십시오

* class [NotebookSaveOptions](../../../aspose.note.saving/notebooksaveoptions/)
* class [Notebook](../)
* 네임스페이스 [Aspose.Note](../../notebook/)
* 집회 [Aspose.Note](../../../)


