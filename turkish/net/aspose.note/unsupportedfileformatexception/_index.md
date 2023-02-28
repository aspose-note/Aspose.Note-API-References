---
title: Class UnsupportedFileFormatException
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.UnsupportedFileFormatException sınıf. Belge yükleme sırasında dosya formatı Aspose.Note. tarafından tanınmadığında veya desteklenmediğinde atılır.
type: docs
weight: 990
url: /tr/net/aspose.note/unsupportedfileformatexception/
---
## UnsupportedFileFormatException class

Belge yükleme sırasında, dosya formatı Aspose.Note. tarafından tanınmadığında veya desteklenmediğinde atılır.

```csharp
public class UnsupportedFileFormatException : Exception
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [FileFormat](../../aspose.note/unsupportedfileformatexception/fileformat/) { get; } | Algılanırsa iletilen verilerin dosya biçimini alır. |

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

* ad alanı [Aspose.Note](../../aspose.note/)
* toplantı [Aspose.Note](../../)


