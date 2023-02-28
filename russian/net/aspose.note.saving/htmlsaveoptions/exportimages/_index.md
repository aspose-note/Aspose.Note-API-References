---
title: HtmlSaveOptions.ExportImages
second_title: Справочник по API Aspose.Note для .NET
description: HtmlSaveOptions свойство. Получает или задает способ экспорта изображений.
type: docs
weight: 70
url: /ru/net/aspose.note.saving/htmlsaveoptions/exportimages/
---
## HtmlSaveOptions.ExportImages property

Получает или задает способ экспорта изображений.

```csharp
public ResourceExportType ExportImages { get; set; }
```

### Примеры

Показывает, как сохранить документ в формате html с сохранением всех ресурсов (css/шрифты/изображения) в отдельные файлы.

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

Показывает, как сохранить документ в поток в формате html с встраиванием всех ресурсов (css/шрифты/изображения).

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

### Смотрите также

* enum [ResourceExportType](../../../aspose.note.saving.html/resourceexporttype/)
* class [HtmlSaveOptions](../)
* пространство имен [Aspose.Note.Saving](../../htmlsaveoptions/)
* сборка [Aspose.Note](../../../)


