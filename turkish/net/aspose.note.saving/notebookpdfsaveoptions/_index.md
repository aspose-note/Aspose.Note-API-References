---
title: Class NotebookPdfSaveOptions
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.Saving.NotebookPdfSaveOptions sınıf. Not defteri sayfalarını PDFye dönüştürürken ek seçenekler belirlemeye izin verir.
type: docs
weight: 780
url: /tr/net/aspose.note.saving/notebookpdfsaveoptions/
---
## NotebookPdfSaveOptions class

Not defteri sayfalarını PDF'ye dönüştürürken ek seçenekler belirlemeye izin verir.

```csharp
public class NotebookPdfSaveOptions : NotebookSaveOptions<PdfSaveOptions>
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [NotebookPdfSaveOptions](notebookpdfsaveoptions/)() | Default_Constructor |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | Alt belgeler 'nin açıkça kaydedilip kaydedilmeyeceğini belirten bir değer alır veya ayarlar. |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } |  |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | Not defteri alt hiyerarşisinin düzleştirilmiş olarak kaydedilip kaydedilmediğini gösteren bir değer alır veya ayarlar. |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } |  |

## yöntemler

| İsim | Tanım |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() |  |

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

* class [NotebookSaveOptions&lt;TDocumentSaveOptions&gt;](../notebooksaveoptions-1/)
* class [PdfSaveOptions](../pdfsaveoptions/)
* ad alanı [Aspose.Note.Saving](../../aspose.note.saving/)
* toplantı [Aspose.Note](../../)


