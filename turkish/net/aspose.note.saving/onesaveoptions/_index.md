---
title: Class OneSaveOptions
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.Saving.OneSaveOptions sınıf. Belgeyi OneNote biçiminde kaydederken ek seçenekler belirlemeye izin verir.
type: docs
weight: 810
url: /tr/net/aspose.note.saving/onesaveoptions/
---
## OneSaveOptions class

Belgeyi OneNote biçiminde kaydederken ek seçenekler belirlemeye izin verir.

```csharp
public sealed class OneSaveOptions : SaveOptions
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [OneSaveOptions](onesaveoptions/)() | Default_Constructor |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [DocumentPassword](../../aspose.note.saving/onesaveoptions/documentpassword/) { get; set; } | Belge içeriğini şifrelemek için bir parola alır veya ayarlar. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Kaydederken kullanılacak yazı tipi ayarlarını alır veya ayarlar |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Kaydedilecek sayfa sayısını alır veya ayarlar. varsayılan olarakMaxValue , bu, belgenin tüm sayfalarının oluşturulacağı anlamına gelir. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Kaydedilecek ilk sayfanın dizinini alır veya ayarlar. Varsayılan olarak 0. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Belgenin kaydedildiği biçimi alır. |

### Örnekler

Dokümanın şifreli olarak nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

OneSaveOptions kullanılarak bir belgenin nasıl kaydedileceğini gösterir.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

### Ayrıca bakınız

* class [SaveOptions](../saveoptions/)
* ad alanı [Aspose.Note.Saving](../../aspose.note.saving/)
* toplantı [Aspose.Note](../../)


