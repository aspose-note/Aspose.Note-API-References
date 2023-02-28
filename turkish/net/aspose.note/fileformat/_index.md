---
title: Enum FileFormat
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.FileFormat Sıralama. OneNote dosya biçimini temsil eder.
type: docs
weight: 90
url: /tr/net/aspose.note/fileformat/
---
## FileFormat enumeration

OneNote dosya biçimini temsil eder.

```csharp
public enum FileFormat
```

### değerler

| İsim | Değer | Tanım |
| --- | --- | --- |
| Unknown | `0` | Bilinmeyen dosya biçimi. |
| OneNote2007 | `1` | OneNote 2010. |
| OneNote2010 | `2` | OneNote 2010. |
| OneNoteOnline | `3` | OneNote Çevrimiçi. |

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


