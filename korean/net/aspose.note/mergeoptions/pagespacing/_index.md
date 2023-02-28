---
title: MergeOptions.PageSpacing
second_title: .NET API 참조용 Aspose.Note
description: MergeOptions 재산. 단일 페이지로 가져올 때 페이지 사이의 간격을 가져오거나 설정합니다.
type: docs
weight: 50
url: /ko/net/aspose.note/mergeoptions/pagespacing/
---
## MergeOptions.PageSpacing property

단일 페이지로 가져올 때 페이지 사이의 간격을 가져오거나 설정합니다.

```csharp
public float PageSpacing { get; set; }
```

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

* class [MergeOptions](../)
* 네임스페이스 [Aspose.Note](../../mergeoptions/)
* 집회 [Aspose.Note](../../../)


