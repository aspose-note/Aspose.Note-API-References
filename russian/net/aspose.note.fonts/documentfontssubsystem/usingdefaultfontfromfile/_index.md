---
title: DocumentFontsSubsystem.UsingDefaultFontFromFile
second_title: Справочник по API Aspose.Note для .NET
description: DocumentFontsSubsystem метод. Создать новый экземпляр DocumentFontsSubsystem используя шрифт из указанного файла по умолчанию.
type: docs
weight: 40
url: /ru/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/
---
## DocumentFontsSubsystem.UsingDefaultFontFromFile method

Создать новый экземпляр DocumentFontsSubsystem, используя шрифт из указанного файла по умолчанию.

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromFile(string filePath, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | String | Файл, содержащий имя шрифта по умолчанию. |
| fontsSubstitutions | Dictionary`2 | Замена шрифтов. |

### Возвращаемое значение

[`DocumentFontsSubsystem`](../) .

### Примеры

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

### Смотрите также

* class [DocumentFontsSubsystem](../)
* пространство имен [Aspose.Note.Fonts](../../documentfontssubsystem/)
* сборка [Aspose.Note](../../../)


