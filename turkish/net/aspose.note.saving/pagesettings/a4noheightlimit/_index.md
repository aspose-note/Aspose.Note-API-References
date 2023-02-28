---
title: PageSettings.A4NoHeightLimit
second_title: Aspose.Note for .NET API Referansı
description: PageSettings mülk. Sınırsız yüksekliğe sahip A4 biçimli sayfa için ayarları alır.
type: docs
weight: 20
url: /tr/net/aspose.note.saving/pagesettings/a4noheightlimit/
---
## PageSettings.A4NoHeightLimit property

Sınırsız yüksekliğe sahip A4 biçimli sayfa için ayarları alır.

```csharp
public static PageSettings A4NoHeightLimit { get; }
```

### Örnekler

Bir belgenin A4 sayfa düzeninde yükseklik sınırı olmaksızın PDF formatında nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Belgeyi Aspose.Note'a yükleyin.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// Belgeyi kaydedin.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

### Ayrıca bakınız

* class [PageSettings](../)
* ad alanı [Aspose.Note.Saving](../../pagesettings/)
* toplantı [Aspose.Note](../../../)


