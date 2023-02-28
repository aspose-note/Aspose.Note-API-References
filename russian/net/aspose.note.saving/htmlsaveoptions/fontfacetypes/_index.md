---
title: HtmlSaveOptions.FontFaceTypes
second_title: Справочник по API Aspose.Note для .NET
description: HtmlSaveOptions свойство. Получает или задает типы шрифта.
type: docs
weight: 80
url: /ru/net/aspose.note.saving/htmlsaveoptions/fontfacetypes/
---
## HtmlSaveOptions.FontFaceTypes property

Получает или задает типы шрифта.

```csharp
public FontFaceType FontFaceTypes { get; set; }
```

### Стоимость имущества

Типы начертания шрифта.

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

Показывает, как сохранить документ в формате html с сохранением всех ресурсов (css/шрифты/изображения) с помощью пользовательских обратных вызовов.

```csharp
// Код ниже создает папку «documentFolder», содержащую document.html, папку «css» с файлом «style.css», папку «images» с изображениями и папку «fonts» со шрифтами.
// Файл 'style.css' будет содержать в конце следующую строку "/* Эта строка добавляется к потоку вручную пользователем */"
var savingCallbacks = new UserSavingCallbacks()
                          {
                              RootFolder = "documentFolder",
                              CssFolder = "css",
                              KeepCssStreamOpened = true,
                              ImagesFolder = "images",
                              FontsFolder = "fonts"
                          };
var options = new HtmlSaveOptions
              {
                  FontFaceTypes = FontFaceType.Ttf,
                  CssSavingCallback = savingCallbacks,
                  FontSavingCallback = savingCallbacks,
                  ImageSavingCallback = savingCallbacks
              };

if (!Directory.Exists(savingCallbacks.RootFolder))
{
    Directory.CreateDirectory(savingCallbacks.RootFolder);
}

string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
var document = new Document(Path.Combine(dataDir, "Aspose.one"));

using (var stream = File.Create(Path.Combine(savingCallbacks.RootFolder, "document.html")))
{
    document.Save(stream, options);
}

using (var writer = new StreamWriter(savingCallbacks.CssStream))
{
    writer.WriteLine();
    writer.WriteLine("/* This line is appended to stream manually by user */");
}
```

### Смотрите также

* enum [FontFaceType](../../../aspose.note.saving.html/fontfacetype/)
* class [HtmlSaveOptions](../)
* пространство имен [Aspose.Note.Saving](../../htmlsaveoptions/)
* сборка [Aspose.Note](../../../)


