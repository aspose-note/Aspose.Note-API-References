---
title: MergeOptions.InsertAt
second_title: .NET API 참조용 Aspose.Note
description: MergeOptions 재산. 가져온 페이지가 삽입될 위치를 가져오거나 설정합니다.
type: docs
weight: 40
url: /ko/net/aspose.note/mergeoptions/insertat/
---
## MergeOptions.InsertAt property

가져온 페이지가 삽입될 위치를 가져오거나 설정합니다.

```csharp
public int InsertAt { get; set; }
```

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentOutOfRangeException |  |

### 비고

값이 대상 문서의 페이지 수보다 크면 가져온 페이지가 문서 끝에 추가됩니다.

### 예

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

### 또한보십시오

* class [MergeOptions](../)
* 네임스페이스 [Aspose.Note](../../mergeoptions/)
* 집회 [Aspose.Note](../../../)


