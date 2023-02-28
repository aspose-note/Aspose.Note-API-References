---
title: HtmlSaveOptions.ExportCss
second_title: .NET API 참조용 Aspose.Note
description: HtmlSaveOptions 재산. CSS를 내보내는 방법을 가져오거나 설정합니다.
type: docs
weight: 50
url: /ko/net/aspose.note.saving/htmlsaveoptions/exportcss/
---
## HtmlSaveOptions.ExportCss property

CSS를 내보내는 방법을 가져오거나 설정합니다.

```csharp
public ResourceExportType ExportCss { get; set; }
```

### 예

모든 리소스(css/fonts/images)를 별도의 파일에 저장하여 문서를 html 형식으로 저장하는 방법을 보여줍니다.

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportAsStream,
                 ExportFonts = ResourceExportType.ExportAsStream,
                 ExportImages = ResourceExportType.ExportAsStream,
                 FontFaceTypes = FontFaceType.Ttf
             };
document.Save(dataDir + "document_out.html", options);
```

모든 리소스(css/fonts/images)를 포함하여 html 형식의 스트림에 문서를 저장하는 방법을 보여줍니다.

```csharp
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

var options = new HtmlSaveOptions()
             {
                 ExportCss = ResourceExportType.ExportEmbedded,
                 ExportFonts = ResourceExportType.ExportEmbedded,
                 ExportImages = ResourceExportType.ExportEmbedded,
                 FontFaceTypes = FontFaceType.Ttf
             };

var r = new MemoryStream();
document.Save(r, options);
```

### 또한보십시오

* enum [ResourceExportType](../../../aspose.note.saving.html/resourceexporttype/)
* class [HtmlSaveOptions](../)
* 네임스페이스 [Aspose.Note.Saving](../../htmlsaveoptions/)
* 집회 [Aspose.Note](../../../)


