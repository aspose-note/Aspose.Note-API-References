---
title: Document.FileFormat
second_title: Aspose.Note for .NET API Referansı
description: Document mülk. Dosya biçimini alır OneNote 2010 OneNote Çevrimiçi.
type: docs
weight: 60
url: /tr/net/aspose.note/document/fileformat/
---
## Document.FileFormat property

Dosya biçimini alır (OneNote 2010, OneNote Çevrimiçi).

```csharp
public FileFormat FileFormat { get; }
```

### Örnekler

Bir belgenin dosya formatının nasıl alınacağını gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // OneNote 2010'u işle
        break;
    case FileFormat.OneNoteOnline:
        // OneNote'u Çevrimiçi İşle
        break;
}
```

### Ayrıca bakınız

* enum [FileFormat](../../fileformat/)
* class [Document](../)
* ad alanı [Aspose.Note](../../document/)
* toplantı [Aspose.Note](../../../)


