---
title: HtmlSaveOptions.ExportImages
second_title: Aspose.Note for .NET API リファレンス
description: HtmlSaveOptions 財産. 画像のエクスポート方法を取得または設定します
type: docs
weight: 70
url: /ja/net/aspose.note.saving/htmlsaveoptions/exportimages/
---
## HtmlSaveOptions.ExportImages property

画像のエクスポート方法を取得または設定します。

```csharp
public ResourceExportType ExportImages { get; set; }
```

### 例

すべてのリソース (css/fonts/images) を別のファイルに保存して、ドキュメントを HTML 形式で保存する方法を示します。

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

すべてのリソース (css/fonts/images) を埋め込んで、ドキュメントを HTML 形式でストリームに保存する方法を示します。

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

### 関連項目

* enum [ResourceExportType](../../../aspose.note.saving.html/resourceexporttype/)
* class [HtmlSaveOptions](../)
* 名前空間 [Aspose.Note.Saving](../../htmlsaveoptions/)
* 組み立て [Aspose.Note](../../../)


