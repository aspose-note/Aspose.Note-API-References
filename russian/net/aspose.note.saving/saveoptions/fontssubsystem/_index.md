---
title: SaveOptions.FontsSubsystem
second_title: Справочник по API Aspose.Note для .NET
description: SaveOptions свойство. Получает или задает настройки шрифта которые будут использоваться при сохранении
type: docs
weight: 10
url: /ru/net/aspose.note.saving/saveoptions/fontssubsystem/
---
## SaveOptions.FontsSubsystem property

Получает или задает настройки шрифта, которые будут использоваться при сохранении

```csharp
public FontsSubsystem FontsSubsystem { get; set; }
```

### Примеры

Показывает, как сохранить документ в формате pdf, используя указанный шрифт по умолчанию.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Сохраняем документ как PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

Показывает, как сохранить документ в формате pdf, используя шрифт по умолчанию из файла.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Сохраняем документ как PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

Показывает, как сохранить документ в формате pdf, используя шрифт по умолчанию из потока.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Сохраняем документ как PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### Смотрите также

* class [FontsSubsystem](../../../aspose.note.fonts/fontssubsystem/)
* class [SaveOptions](../)
* пространство имен [Aspose.Note.Saving](../../saveoptions/)
* сборка [Aspose.Note](../../../)


