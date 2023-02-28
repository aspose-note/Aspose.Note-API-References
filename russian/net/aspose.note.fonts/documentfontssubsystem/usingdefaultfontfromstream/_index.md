---
title: DocumentFontsSubsystem.UsingDefaultFontFromStream
second_title: Справочник по API Aspose.Note для .NET
description: DocumentFontsSubsystem метод. Создать новый экземпляр DocumentFontsSubsystem используя шрифт из указанного потока по умолчанию.
type: docs
weight: 50
url: /ru/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/
---
## DocumentFontsSubsystem.UsingDefaultFontFromStream method

Создать новый экземпляр DocumentFontsSubsystem, используя шрифт из указанного потока по умолчанию.

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromStream(Stream defaultFontStream, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| defaultFontStream | Stream | Поток, содержащий имя шрифта по умолчанию. |
| fontsSubstitutions | Dictionary`2 | Замена шрифтов. |

### Возвращаемое значение

[`DocumentFontsSubsystem`](../) .

### Примеры

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

* class [DocumentFontsSubsystem](../)
* пространство имен [Aspose.Note.Fonts](../../documentfontssubsystem/)
* сборка [Aspose.Note](../../../)


