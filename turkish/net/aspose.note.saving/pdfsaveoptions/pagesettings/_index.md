---
title: PdfSaveOptions.PageSettings
second_title: Aspose.Note for .NET API Referansı
description: PdfSaveOptions mülk. Belgedeki her sayfa için sayfa ayarlarını alır veya ayarlar. Varsayılan olarak CurrentUICulturea bağlıdır ABD kültürlerinin harf ayarı vardır diğerlerinin A4 ayarları vardır.
type: docs
weight: 40
url: /tr/net/aspose.note.saving/pdfsaveoptions/pagesettings/
---
## PdfSaveOptions.PageSettings property

Belgedeki her sayfa için sayfa ayarlarını alır veya ayarlar. Varsayılan olarak CurrentUICulture'a bağlıdır, *ABD kültürlerinin harf ayarı vardır, diğerlerinin A4 ayarları vardır.

```csharp
public PageSettings PageSettings { get; set; }
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

* class [PageSettings](../../pagesettings/)
* class [PdfSaveOptions](../)
* ad alanı [Aspose.Note.Saving](../../pdfsaveoptions/)
* toplantı [Aspose.Note](../../../)


