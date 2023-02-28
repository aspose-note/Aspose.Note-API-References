---
title: Class Notebook
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.Notebook 수업. Aspose.Note 노트북을 나타냅니다.
type: docs
weight: 410
url: /ko/net/aspose.note/notebook/
---
## Notebook class

Aspose.Note 노트북을 나타냅니다.

```csharp
public class Notebook : IEnumerable<INotebookChildNode>, INotebookChildNode
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Notebook](notebook/#constructor)() | 의 새 인스턴스를 초기화합니다.`Notebook` 클래스. |
| [Notebook](notebook/#constructor_1)(Stream) | 의 새 인스턴스를 초기화합니다.`Notebook` class. 스트림에서 기존 OneNote 전자 필기장을 엽니다. |
| [Notebook](notebook/#constructor_3)(string) | 의 새 인스턴스를 초기화합니다.`Notebook` class. 파일에서 기존 OneNote 전자 필기장을 엽니다. |
| [Notebook](notebook/#constructor_2)(Stream, NotebookLoadOptions) | 의 새 인스턴스를 초기화합니다.`Notebook` class. 스트림에서 기존 OneNote 노트북을 엽니다. 추가 로딩 옵션을 지정할 수 있습니다. |
| [Notebook](notebook/#constructor_4)(string, NotebookLoadOptions) | 의 새 인스턴스를 초기화합니다.`Notebook` class. 파일에서 기존 OneNote 전자 필기장을 엽니다. 하위 로딩 전략("lazy"/instant)과 같은 추가 옵션을 지정할 수 있습니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Color](../../aspose.note/notebook/color/) { get; set; } | 색상을 가져오거나 설정합니다. |
| [Count](../../aspose.note/notebook/count/) { get; } | 에 포함된 요소 수를 가져옵니다.`Notebook` . |
| [DisplayName](../../aspose.note/notebook/displayname/) { get; set; } | 표시 이름을 가져오거나 설정합니다. |
| [FileFormat](../../aspose.note/notebook/fileformat/) { get; } | 파일 형식 가져오기(OneNote 2010, OneNote Online). |
| [Guid](../../aspose.note/notebook/guid/) { get; } | 개체의 전역 고유 ID를 가져옵니다. |
| [IsHistoryEnabled](../../aspose.note/notebook/ishistoryenabled/) { get; set; } | 기록이 활성화되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Item](../../aspose.note/notebook/item/) { get; } | 지정된 인덱스로 노트북 자식 노드를 가져옵니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [AppendChild](../../aspose.note/notebook/appendchild/)(INotebookChildNode) | 목록 끝에 노드를 추가합니다. |
| [GetChildNodes&lt;T1&gt;](../../aspose.note/notebook/getchildnodes/)() | 노드 유형별로 모든 하위 노드를 가져옵니다. |
| [GetEnumerator](../../aspose.note/notebook/getenumerator/)() | 의 자식 노드를 반복하는 열거자를 반환합니다.`Notebook` . |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument)(Stream) | 하위 문서 노드를 추가합니다. 스트림에서 기존 OneNote 문서를 엽니다. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_2)(string) | 하위 문서 노드를 추가합니다. 파일에서 기존 OneNote 문서를 엽니다. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_1)(Stream, LoadOptions) | 하위 문서 노드를 추가합니다. 스트림에서 기존 OneNote 문서를 엽니다. 추가 로드 옵션을 지정할 수 있습니다. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument/#loadchilddocument_3)(string, LoadOptions) | 하위 문서 노드를 추가합니다. 파일에서 기존 OneNote 문서를 엽니다. 추가 로드 옵션을 지정할 수 있습니다. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook)(Stream) | 하위 노트북 노드를 추가합니다. 스트림에서 기존 OneNote 노트북을 엽니다. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_2)(string) | 하위 노트북 노드를 추가합니다. 파일에서 기존 OneNote 노트북을 엽니다. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_1)(Stream, NotebookLoadOptions) | 자식 노트북 노드를 추가합니다. 스트림에서 기존 OneNote 노트북을 엽니다. 추가 로드 옵션을 지정할 수 있습니다. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook/#loadchildnotebook_3)(string, NotebookLoadOptions) | 자식 노트북 노드를 추가합니다. 파일에서 기존 OneNote 노트북을 엽니다. 추가 로드 옵션을 지정할 수 있습니다. |
| [RemoveChild](../../aspose.note/notebook/removechild/)(INotebookChildNode) | 자식 노드를 제거합니다. |
| [Save](../../aspose.note/notebook/save/#save)(Stream) | OneNote 문서를 스트림에 저장합니다. |
| [Save](../../aspose.note/notebook/save/#save_3)(string) | OneNote 문서를 파일에 저장합니다. |
| [Save](../../aspose.note/notebook/save/#save_2)(Stream, NotebookSaveOptions) | 지정된 저장 옵션을 사용하여 OneNote 문서를 스트림에 저장합니다. |
| [Save](../../aspose.note/notebook/save/#save_1)(Stream, SaveFormat) | OneNote 문서를 지정된 형식의 스트림에 저장합니다. |
| [Save](../../aspose.note/notebook/save/#save_5)(string, NotebookSaveOptions) | 지정된 저장 옵션을 사용하여 OneNote 문서를 파일로 저장합니다. |
| [Save](../../aspose.note/notebook/save/#save_4)(string, SaveFormat) | OneNote 문서를 지정된 형식의 파일로 저장합니다. |

### 예

노트북을 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook();

dataDir = dataDir + "test_out.onetoc2";

// 노트북 저장
notebook.Save(dataDir);
```

노트북을 PDF 형식으로 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote 전자 필기장 로드
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToPDF_out.pdf";

// 노트북 저장
notebook.Save(dataDir);
```

노트북을 이미지로 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote 전자 필기장 로드
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToImage_out.png";

// 노트북 저장
notebook.Save(dataDir);
```

노트북에서 모든 텍스트를 가져오는 방법을 보여줍니다.

```csharp
string inputFile = "notebook.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

Notebook rootNotebook = new Notebook(dataDir + inputFile);

IList<RichText> allRichTextNodes = rootNotebook.GetChildNodes<RichText>();
foreach (RichText richTextNode in allRichTextNodes)
{
    Console.WriteLine(richTextNode.Text);
}
```

결합된 노트북을 pdf 형식으로 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote 전자 필기장 로드
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// 노트북 저장
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

느리게 로드하는 노트북의 문서를 반복하는 방법을 보여줍니다.

```csharp
string inputFile = "Notizbuch öffnen.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

// 기본적으로 자식 로딩은 "lazy"입니다.
Notebook notebook = new Notebook(dataDir + inputFile);

foreach (var notebookChildNode in notebook.OfType<Document>()) 
{
    // 하위 문서의 실제 로드는 여기에서만 발생합니다.
    // 하위 문서로 작업 수행
}
```

노트북에 새 섹션을 추가하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote 전자 필기장 로드
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// 새 자식을 노트북에 추가
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// 노트북 저장
notebook.Save(dataDir);
```

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

노트북을 암호화하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

지정된 옵션을 사용하여 노트북을 이미지로 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote 전자 필기장 로드
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// 노트북 저장
notebook.Save(dataDir, notebookSaveOptions);
```

병합된 노트북을 이미지로 저장하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote 전자 필기장 로드
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// 노트북 저장
notebook.Save(dataDir, notebookSaveOptions);
```

전자 필기장에서 섹션을 제거하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_NoteBook();

// OneNote 전자 필기장 로드
var notebook = new Notebook(dataDir + "test.onetoc2");

// 원하는 자식 항목을 검색하기 위해 자식 노드를 통과합니다.
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // 노트북에서 하위 항목 제거
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// 노트북 저장
notebook.Save(dataDir);
```

노트북의 미리 로드된 문서를 반복하는 방법을 보여줍니다.

```csharp
// 기본적으로 자식 로딩은 "lazy"입니다.
// 따라서 인스턴트 로딩이 발생했기 때문에,
// NotebookLoadOptions.InstantLoading 플래그를 설정해야 합니다.
NotebookLoadOptions loadOptions = new NotebookLoadOptions { InstantLoading = true };

String inputFile = "Notizbuch öffnen.onetoc2";
String dataDir = RunExamples.GetDataDir_NoteBook();
Notebook notebook = new Notebook(dataDir + inputFile, loadOptions);

// 모든 하위 문서가 이미 로드되었습니다.
foreach (INotebookChildNode notebookChildNode in notebook.OfType<Document>()) 
{
   // 하위 문서로 작업 수행
}
```

노트북의 콘텐츠를 전달하는 방법을 보여줍니다.

```csharp
// 문서 디렉토리의 경로.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = "Open Notebook.onetoc2";
try
{
    var notebook = new Notebook(dataDir + fileName);
    foreach (var notebookChildNode in notebook)
    {
        Console.WriteLine(notebookChildNode.DisplayName);
        if (notebookChildNode is Document)
        {
            // 하위 문서로 작업 수행
        }
        else if (notebookChildNode is Notebook)
        {
            // 자식 노트북으로 작업 수행
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

### 또한보십시오

* interface [INotebookChildNode](../inotebookchildnode/)
* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


