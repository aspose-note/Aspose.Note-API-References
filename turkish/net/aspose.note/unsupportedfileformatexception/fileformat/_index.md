---
title: UnsupportedFileFormatException.FileFormat
second_title: Aspose.Note for .NET API Referansı
description: UnsupportedFileFormatException mülk. Algılanırsa iletilen verilerin dosya biçimini alır.
type: docs
weight: 10
url: /tr/net/aspose.note/unsupportedfileformatexception/fileformat/
---
## UnsupportedFileFormatException.FileFormat property

Algılanırsa iletilen verilerin dosya biçimini alır.

```csharp
public FileFormat FileFormat { get; }
```

### Örnekler

OneNote 2007 formatı desteklenmediği için belge yüklemenin başarısız olup olmadığının nasıl kontrol edileceğini gösterir.

```csharp
// Belgeler dizininin yolu.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "OneNote2007.one");

try
{
    new Document(fileName);
}
catch (UnsupportedFileFormatException e)
{
    if (e.FileFormat == FileFormat.OneNote2007)
    {
        Console.WriteLine("It looks like the provided file is in OneNote 2007 format that is not supported.");
    }
    else
        throw;
}
```

### Ayrıca bakınız

* enum [FileFormat](../../fileformat/)
* class [UnsupportedFileFormatException](../)
* ad alanı [Aspose.Note](../../unsupportedfileformatexception/)
* toplantı [Aspose.Note](../../../)


