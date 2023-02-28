---
title: PdfImporter.Import
second_title: .NET API 참조용 Aspose.Note
description: PdfImporter 방법. 제공된 스트림에서 PDF 문서의 내용을 가져옵니다.
type: docs
weight: 10
url: /ko/net/aspose.note.importing/pdfimporter/import/
---
## Import(Stream, PdfImportOptions) {#import}

제공된 스트림에서 PDF 문서의 내용을 가져옵니다.

```csharp
public static List<Page> Import(Stream stream, PdfImportOptions options = null)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| stream | Stream | 스트림. |
| options | PdfImportOptions | 옵션. |

### 반환 값

[`PdfImporter`](../) .

### 또한보십시오

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* 네임스페이스 [Aspose.Note.Importing](../../pdfimporter/)
* 집회 [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions) {#import_1}

지정된 파일에서 PDF 문서의 내용을 가져옵니다.

```csharp
public static List<Page> Import(string file, PdfImportOptions options = null)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| file | String | PDF 파일. |
| options | PdfImportOptions | 옵션. |

### 반환 값

[`PdfImporter`](../) .

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

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* 네임스페이스 [Aspose.Note.Importing](../../pdfimporter/)
* 집회 [Aspose.Note](../../../)


