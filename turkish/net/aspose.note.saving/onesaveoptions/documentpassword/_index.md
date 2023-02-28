---
title: OneSaveOptions.DocumentPassword
second_title: Aspose.Note for .NET API Referansı
description: OneSaveOptions mülk. Belge içeriğini şifrelemek için bir parola alır veya ayarlar.
type: docs
weight: 20
url: /tr/net/aspose.note.saving/onesaveoptions/documentpassword/
---
## OneSaveOptions.DocumentPassword property

Belge içeriğini şifrelemek için bir parola alır veya ayarlar.

```csharp
public string DocumentPassword { get; set; }
```

### Örnekler

Dokümanın şifreli olarak nasıl kaydedileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

### Ayrıca bakınız

* class [OneSaveOptions](../)
* ad alanı [Aspose.Note.Saving](../../onesaveoptions/)
* toplantı [Aspose.Note](../../../)


