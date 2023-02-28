---
title: Class PdfImporter
second_title: .NET API 참조용 Aspose.Note
description: Aspose.Note.Importing.PdfImporter 수업. PDF 형식의 문서에서 콘텐츠를 가져올 수 있는 API를 제공하는 클래스입니다. API는 지정된 옵션을 사용하여 파일 또는 스트림에 있는 PDF 문서에서 가져올 수 있습니다. 가져오기 옵션은PdfImportOptions .
type: docs
weight: 270
url: /ko/net/aspose.note.importing/pdfimporter/
---
## PdfImporter class

PDF 형식의 문서에서 콘텐츠를 가져올 수 있는 API를 제공하는 클래스입니다. API는 지정된 옵션을 사용하여 파일 또는 스트림에 있는 PDF 문서에서 가져올 수 있습니다. 가져오기 옵션은[`PdfImportOptions`](../pdfimportoptions/) .

```csharp
public static class PdfImporter
```

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import)(Stream, PdfImportOptions) | 제공된 스트림에서 PDF 문서의 내용을 가져옵니다. |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import_1)(string, PdfImportOptions) | 지정된 파일에서 PDF 문서의 내용을 가져옵니다. |

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

* 네임스페이스 [Aspose.Note.Importing](../../aspose.note.importing/)
* 집회 [Aspose.Note](../../)


