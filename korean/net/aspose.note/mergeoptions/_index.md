---
title: Class MergeOptions
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.MergeOptions 수업. 페이지 모음을 병합하기 위한 옵션입니다.
type: docs
weight: 340
url: /ko/net/aspose.note/mergeoptions/
---
## MergeOptions class

페이지 모음을 병합하기 위한 옵션입니다.

```csharp
public class MergeOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [MergeOptions](mergeoptions/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [ImportAsSinglePage](../../aspose.note/mergeoptions/importassinglepage/) { get; set; } | 제공된 페이지를 단일 페이지로 가져올지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [InsertAsChild](../../aspose.note/mergeoptions/insertaschild/) { get; set; } | 삽입된 페이지를 이전 페이지의 자식으로 추가해야 하는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [InsertAt](../../aspose.note/mergeoptions/insertat/) { get; set; } | 가져온 페이지가 삽입될 위치를 가져오거나 설정합니다. |
| [PageSpacing](../../aspose.note/mergeoptions/pagespacing/) { get; set; } | 단일 페이지로 가져올 때 페이지 사이의 간격을 가져오거나 설정합니다. |

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

* 네임스페이스 [Aspose.Note](../../aspose.note/)
* 집회 [Aspose.Note](../../)


