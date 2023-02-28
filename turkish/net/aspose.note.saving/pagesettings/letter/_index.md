---
title: PageSettings.Letter
second_title: Aspose.Note for .NET API Referansı
description: PageSettings mülk. Letter biçimli sayfa için ayarları alır.
type: docs
weight: 30
url: /tr/net/aspose.note.saving/pagesettings/letter/
---
## PageSettings.Letter property

Letter biçimli sayfa için ayarları alır.

```csharp
public static PageSettings Letter { get; }
```

### Örnekler

Bir belgenin Letter sayfa düzeniyle PDF formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// Belgeyi kaydedin.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

### Ayrıca bakınız

* class [PageSettings](../)
* ad alanı [Aspose.Note.Saving](../../pagesettings/)
* toplantı [Aspose.Note](../../../)


