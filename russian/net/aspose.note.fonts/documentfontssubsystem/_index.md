---
title: DocumentFontsSubsystem
second_title: Справочник по API Aspose.Note для .NET
description: Простая реализация Aspose.Note.Fonts.FontsSubsystem. Извлекает объектFontFamilyиз ОС.
type: docs
weight: 100
url: /ru/net/aspose.note.fonts/documentfontssubsystem/
---
## DocumentFontsSubsystem class

Простая реализация Aspose.Note.Fonts.FontsSubsystem. Извлекает объектFontFamilyиз ОС.

```csharp
public class DocumentFontsSubsystem : FontsSubsystem
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [DocumentFontsSubsystem](documentfontssubsystem#constructor)(Dictionary&lt;string, string&gt;) | Инициализирует новый экземпляр класса[`DocumentFontsSubsystem`](../documentfontssubsystem). |
| [DocumentFontsSubsystem](documentfontssubsystem#constructor_1)(Stream, Dictionary&lt;string, string&gt;) | Инициализирует новый экземпляр класса[`DocumentFontsSubsystem`](../documentfontssubsystem). |
| [DocumentFontsSubsystem](documentfontssubsystem#constructor_2)(string, Dictionary&lt;string, string&gt;) | Инициализирует новый экземпляр класса[`DocumentFontsSubsystem`](../documentfontssubsystem). |

## Характеристики

| Имя | Описание |
| --- | --- |
| static [Default](../../aspose.note.fonts/documentfontssubsystem/default) { get; set; } | Получает или задает статический экземпляр по умолчанию. |
| [DefaultFont](../../aspose.note.fonts/fontssubsystem/defaultfont) { get; } | Получает или устанавливает шрифт по умолчанию. |

## Методы

| Имя | Описание |
| --- | --- |
| static [UsingDefaultFont](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfont)(string, Dictionary&lt;string, string&gt;) | Создать новый экземпляр DocumentFontsSubsystem, используя указанное имя шрифта по умолчанию. |
| static [UsingDefaultFontFromFile](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile)(string, Dictionary&lt;string, string&gt;) | Создать новый экземпляр DocumentFontsSubsystem, используя по умолчанию шрифт из указанного файла. |
| static [UsingDefaultFontFromStream](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream)(Stream, Dictionary&lt;string, string&gt;) | Создать новый экземпляр DocumentFontsSubsystem, используя по умолчанию шрифт из указанного потока. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont)(Stream) | Добавить шрифт. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont)(string) | Добавить шрифт. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont)(Stream, string) | Добавить шрифт. |
| [AddFontSubstitution](../../aspose.note.fonts/fontssubsystem/addfontsubstitution)(string, string) | Добавляет замену шрифта. |
| virtual [GetFontFamily](../../aspose.note.fonts/fontssubsystem/getfontfamily)(string) | Получает семейство шрифтов. |
| [LoadFontsFromFolder](../../aspose.note.fonts/fontssubsystem/loadfontsfromfolder)(string) | Загружает все шрифты TrueType из указанной папки во внутреннюю коллекцию. |

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

Показывает, как сохранить документ в формате pdf, используя шрифт по умолчанию из файла.

Показывает, как сохранить документ в формате pdf, используя шрифт по умолчанию из потока.

### Смотрите также

* class [FontsSubsystem](../fontssubsystem)
* пространство имен [Aspose.Note.Fonts](../../aspose.note.fonts)
* сборка [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
