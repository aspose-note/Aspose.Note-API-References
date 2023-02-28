---
title: Document.Import
second_title: .NET API 참조용 Aspose.Note
description: Document 방법. 제공된 PDF 문서에서 페이지 세트를 가져옵니다.
type: docs
weight: 110
url: /ko/net/aspose.note/document/import/
---
## Import(Stream, PdfImportOptions, MergeOptions) {#import}

제공된 PDF 문서에서 페이지 세트를 가져옵니다.

```csharp
public Document Import(Stream stream, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| stream | Stream | PDF 문서가 있는 스트림. |
| importOptions | PdfImportOptions | PDF 문서에서 페이지를 가져오는 방법을 지정합니다. |
| mergeOptions | MergeOptions | 제공된 페이지를 병합하는 방법 옵션을 지정합니다. |

### 반환 값

문서에 대한 참조를 반환합니다.

### 또한보십시오

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions, MergeOptions) {#import_1}

제공된 PDF 문서에서 페이지 세트를 가져옵니다.

```csharp
public Document Import(string file, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| file | String | PDF 문서가 포함된 파일. |
| importOptions | PdfImportOptions | PDF 문서에서 페이지를 가져오는 방법을 지정합니다. |
| mergeOptions | MergeOptions | 제공된 페이지를 병합하는 방법 옵션을 지정합니다. |

### 반환 값

문서에 대한 참조를 반환합니다.

### 예

페이지별로 PDF 문서 세트에서 모든 페이지를 가져오는 방법을 보여줍니다.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

d.Import(Path.Combine(dataDir, "sampleText.pdf"))
 .Import(Path.Combine(dataDir, "sampleImage.pdf"))
 .Import(Path.Combine(dataDir, "sampleTable.pdf"));

d.Save(Path.Combine(dataDir, "sample_SimpleMerge.one"));
```

모든 PDF 문서의 페이지를 최상위 OneNote 페이지의 자식으로 삽입하면서 PDF 문서 집합의 모든 페이지를 가져오는 방법을 보여줍니다.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

foreach (var file in new[] { "sampleText.pdf", "sampleImage.pdf", "sampleTable.pdf" })
{
    d.AppendChildLast(new Page()).Title = new Title() { TitleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append(file) };
    d.Import(Path.Combine(dataDir, file), new PdfImportOptions(), new MergeOptions() { InsertAt = int.MaxValue, InsertAsChild = true });
}

d.Save(Path.Combine(dataDir, "sample_StructuredMerge.one"));
```

모든 PDF 문서의 페이지를 단일 OneNote 페이지로 병합하는 동안 PDF 문서 세트에서 모든 콘텐츠를 가져오는 방법을 보여줍니다.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

var importOptions = new PdfImportOptions();
var mergeOptions = new MergeOptions() { ImportAsSinglePage = true, PageSpacing = 100 };

d.Import(Path.Combine(dataDir, "sampleText.pdf"), importOptions, mergeOptions)
 .Import(Path.Combine(dataDir, "sampleImage.pdf"), importOptions, mergeOptions)
 .Import(Path.Combine(dataDir, "sampleTable.pdf"), importOptions, mergeOptions);

d.Save(Path.Combine(dataDir, "sample_SinglePageMerge.one"));
```

### 또한보십시오

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)


