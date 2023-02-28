---
title: Document.Merge
second_title: .NET API 참조용 Aspose.Note
description: Document 방법. 페이지 집합을 문서에 병합합니다.
type: docs
weight: 120
url: /ko/net/aspose.note/document/merge/
---
## Document.Merge method

페이지 집합을 문서에 병합합니다.

```csharp
public Document Merge(IEnumerable<Page> pages, MergeOptions mergeOptions = null)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| pages | IEnumerable`1 | 페이지 세트. |
| mergeOptions | MergeOptions | 제공된 페이지를 병합하는 방법 옵션을 지정합니다. |

### 반환 값

문서에 대한 참조를 반환합니다.

### 예

5페이지마다 PDF 문서 그룹화에서 모든 페이지를 단일 OneNote 페이지로 가져오는 방법을 보여줍니다.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

var mergeOptions = new MergeOptions() { ImportAsSinglePage = true, PageSpacing = 100 };

IEnumerable<Page> pages = PdfImporter.Import(Path.Combine(dataDir, "SampleGrouping.pdf"));
while (pages.Any())
{
    d.Merge(pages.Take(5), mergeOptions);
    pages = pages.Skip(5);
}

d.Save(Path.Combine(dataDir, "sample_CustomMerge.one"));
```

### 또한보십시오

* class [Page](../../page/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* 네임스페이스 [Aspose.Note](../../document/)
* 집회 [Aspose.Note](../../../)


