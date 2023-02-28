---
title: Class PageSettings
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.Saving.PageSettings sınıf. Bir sayfa için düzen ayarlarını temsil eder.
type: docs
weight: 820
url: /tr/net/aspose.note.saving/pagesettings/
---
## PageSettings class

Bir sayfa için düzen ayarlarını temsil eder.

```csharp
public class PageSettings
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| static [A4](../../aspose.note.saving/pagesettings/a4/) { get; } | A4 biçimli sayfa için ayarları alır. |
| static [A4NoHeightLimit](../../aspose.note.saving/pagesettings/a4noheightlimit/) { get; } | Sınırsız yüksekliğe sahip A4 biçimli sayfa için ayarları alır. |
| static [Letter](../../aspose.note.saving/pagesettings/letter/) { get; } | Letter biçimli sayfa için ayarları alır. |
| static [LetterNoHeightLimit](../../aspose.note.saving/pagesettings/letternoheightlimit/) { get; } | Sınırsız yüksekliğe sahip Letter biçimli sayfa için ayarları alır. |

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

* ad alanı [Aspose.Note.Saving](../../aspose.note.saving/)
* toplantı [Aspose.Note](../../)


