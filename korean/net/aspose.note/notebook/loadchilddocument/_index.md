---
title: Notebook.LoadChildDocument
second_title: .NET API 참조용 Aspose.Note
description: Notebook 방법. 하위 문서 노드를 추가합니다. 파일에서 기존 OneNote 문서를 엽니다.
type: docs
weight: 120
url: /ko/net/aspose.note/notebook/loadchilddocument/
---
## LoadChildDocument(string) {#loadchilddocument_2}

하위 문서 노드를 추가합니다. 파일에서 기존 OneNote 문서를 엽니다.

```csharp
public void LoadChildDocument(string filePath)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | String | 파일 경로. |

### 예

스트림에서 노트북을 로드하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

### 또한보십시오

* class [Notebook](../)
* 네임스페이스 [Aspose.Note](../../notebook/)
* 집회 [Aspose.Note](../../../)

---

## LoadChildDocument(string, LoadOptions) {#loadchilddocument_3}

하위 문서 노드를 추가합니다. 파일에서 기존 OneNote 문서를 엽니다. 추가 로드 옵션을 지정할 수 있습니다.

```csharp
public void LoadChildDocument(string filePath, LoadOptions loadOptions)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | String | 파일 경로. |
| loadOptions | LoadOptions | 로드 옵션입니다. |

### 또한보십시오

* class [LoadOptions](../../loadoptions/)
* class [Notebook](../)
* 네임스페이스 [Aspose.Note](../../notebook/)
* 집회 [Aspose.Note](../../../)

---

## LoadChildDocument(Stream) {#loadchilddocument}

하위 문서 노드를 추가합니다. 스트림에서 기존 OneNote 문서를 엽니다.

```csharp
public void LoadChildDocument(Stream stream)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| stream | Stream | 스트림. |

### 예

스트림에서 노트북을 로드하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

### 또한보십시오

* class [Notebook](../)
* 네임스페이스 [Aspose.Note](../../notebook/)
* 집회 [Aspose.Note](../../../)

---

## LoadChildDocument(Stream, LoadOptions) {#loadchilddocument_1}

하위 문서 노드를 추가합니다. 스트림에서 기존 OneNote 문서를 엽니다. 추가 로드 옵션을 지정할 수 있습니다.

```csharp
public void LoadChildDocument(Stream stream, LoadOptions loadOptions)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| stream | Stream | 스트림. |
| loadOptions | LoadOptions | 로드 옵션입니다. |

### 또한보십시오

* class [LoadOptions](../../loadoptions/)
* class [Notebook](../)
* 네임스페이스 [Aspose.Note](../../notebook/)
* 집회 [Aspose.Note](../../../)


