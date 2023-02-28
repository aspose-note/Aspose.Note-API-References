---
title: Class NotebookSaveOptionsTDocumentSaveOptions
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.Saving.NotebookSaveOptions1TDocumentSaveOptions sınıf. Belirli bir format için not defteri kaydetme seçeneklerini temsil eden ve tüm belge alt düğümleri için ortak kaydetme seçenekleri sağlayan soyut bir temel sınıf.
type: docs
weight: 800
url: /tr/net/aspose.note.saving/notebooksaveoptions-1/
---
## NotebookSaveOptions&lt;TDocumentSaveOptions&gt; class

Belirli bir format için not defteri kaydetme seçeneklerini temsil eden ve tüm belge alt düğümleri için ortak kaydetme seçenekleri sağlayan soyut bir temel sınıf.

```csharp
public abstract class NotebookSaveOptions<TDocumentSaveOptions> : NotebookSaveOptions
    where TDocumentSaveOptions : SaveOptions
```

| Parametre | Tanım |
| --- | --- |
| TDocumentSaveOptions | Not defterinin tüm alt belgeleri için kaydetme seçenekleri. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [DeferredSaving](../../aspose.note.saving/notebooksaveoptions/deferredsaving/) { get; set; } | Alt belgeler 'nin açıkça kaydedilip kaydedilmeyeceğini belirten bir değer alır veya ayarlar. |
| [DocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/documentsaveoptions/) { get; } | Not defterinin tüm alt belgeleri için kaydetme seçeneklerini alır veya ayarlar. |
| [Flatten](../../aspose.note.saving/notebooksaveoptions/flatten/) { get; set; } | Not defteri alt hiyerarşisinin düzleştirilmiş olarak kaydedilip kaydedilmediğini gösteren bir değer alır veya ayarlar. |
| override [SaveFormat](../../aspose.note.saving/notebooksaveoptions-1/saveformat/) { get; } | Not defterinin kaydedildiği biçimi alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| override [GetDocumentSaveOptions](../../aspose.note.saving/notebooksaveoptions-1/getdocumentsaveoptions/)() | Not defterinin tüm alt belgeleri için kaydetme seçeneklerini alır. |

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

* class [NotebookSaveOptions](../notebooksaveoptions/)
* class [SaveOptions](../saveoptions/)
* ad alanı [Aspose.Note.Saving](../../aspose.note.saving/)
* toplantı [Aspose.Note](../../)


