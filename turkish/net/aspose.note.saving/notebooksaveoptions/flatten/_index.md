---
title: NotebookSaveOptions.Flatten
second_title: Aspose.Note for .NET API Referansı
description: NotebookSaveOptions mülk. Not defteri alt hiyerarşisinin düzleştirilmiş olarak kaydedilip kaydedilmediğini gösteren bir değer alır veya ayarlar.
type: docs
weight: 20
url: /tr/net/aspose.note.saving/notebooksaveoptions/flatten/
---
## NotebookSaveOptions.Flatten property

Not defteri alt hiyerarşisinin düzleştirilmiş olarak kaydedilip kaydedilmediğini gösteren bir değer alır veya ayarlar.

```csharp
public bool Flatten { get; set; }
```

### Örnekler

Düzleştirilmiş not defterinin pdf formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Bir OneNote Not Defteri yükleyin
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Not Defterini Kaydet
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

Düzleştirilmiş not defterinin resim olarak nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Bir OneNote Not Defteri yükleyin
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Not Defterini Kaydet
notebook.Save(dataDir, notebookSaveOptions);
```

### Ayrıca bakınız

* class [NotebookSaveOptions](../)
* ad alanı [Aspose.Note.Saving](../../notebooksaveoptions/)
* toplantı [Aspose.Note](../../../)


