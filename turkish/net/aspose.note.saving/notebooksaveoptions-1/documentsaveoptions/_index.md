---
title: NotebookSaveOptions1.DocumentSaveOptions
second_title: Aspose.Note for .NET API Referansı
description: NotebookSaveOptions mülk. Not defterinin tüm alt belgeleri için kaydetme seçeneklerini alır veya ayarlar.
type: docs
weight: 10
url: /tr/net/aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt;.DocumentSaveOptions property

Not defterinin tüm alt belgeleri için kaydetme seçeneklerini alır veya ayarlar.

```csharp
public TDocumentSaveOptions DocumentSaveOptions { get; }
```

### Örnekler

Not defterinin belirtilen seçeneklerle pdf formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Bir OneNote Not Defteri yükleyin
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookPdfSaveOptions();

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Not Defterini Kaydet
notebook.Save(dataDir, notebookSaveOptions);
```

### Ayrıca bakınız

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../)
* ad alanı [Aspose.Note.Saving](../../notebooksaveoptions-1/)
* toplantı [Aspose.Note](../../../)


