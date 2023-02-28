---
title: PdfSaveOptions.JpegQuality
second_title: Справочник по API Aspose.Note для .NET
description: PdfSaveOptions свойство. Получает или задает значение определяющее качество изображений JPEG внутри документа PDF. Значение может варьироваться от 0 до 100 где 0 означает худшее качество но максимальное сжатие а 100 означает лучшее качество но минимальное сжатие.
type: docs
weight: 30
url: /ru/net/aspose.note.saving/pdfsaveoptions/jpegquality/
---
## PdfSaveOptions.JpegQuality property

Получает или задает значение, определяющее качество изображений JPEG внутри документа PDF. Значение может варьироваться от 0 до 100, где 0 означает худшее качество, но максимальное сжатие, а 100 означает лучшее качество, но минимальное сжатие.

```csharp
public int JpegQuality { get; set; }
```

### Примечания

Значение по умолчанию: 90.

### Примеры

Показывает, как сохранить документ в формате pdf, используя определенные настройки.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Инициализировать объект PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Использовать сжатие JPEG
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Качество сжатия JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

### Смотрите также

* class [PdfSaveOptions](../)
* пространство имен [Aspose.Note.Saving](../../pdfsaveoptions/)
* сборка [Aspose.Note](../../../)


