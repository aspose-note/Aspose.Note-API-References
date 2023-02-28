---
title: ImageSaveOptions.Resolution
second_title: Aspose.Note for .NET API Referansı
description: ImageSaveOptions mülk. Oluşturulan görüntülerin çözünürlüğünü inç başına nokta cinsinden alır veya ayarlar.
type: docs
weight: 50
url: /tr/net/aspose.note.saving/imagesaveoptions/resolution/
---
## ImageSaveOptions.Resolution property

Oluşturulan görüntülerin çözünürlüğünü inç başına nokta cinsinden alır veya ayarlar.

```csharp
public float Resolution { get; set; }
```

### Notlar

Varsayılan değer 96. 'dir.

### Örnekler

Belgeyi görüntü olarak kaydederken görüntü çözünürlüğünün nasıl ayarlanacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Belgeyi kaydedin.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

Not defterini belirtilen seçeneklerle resim olarak nasıl kaydedeceğinizi gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Bir OneNote Not Defteri yükleyin
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// Not Defterini Kaydet
notebook.Save(dataDir, notebookSaveOptions);
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

* class [ImageSaveOptions](../)
* ad alanı [Aspose.Note.Saving](../../imagesaveoptions/)
* toplantı [Aspose.Note](../../../)


