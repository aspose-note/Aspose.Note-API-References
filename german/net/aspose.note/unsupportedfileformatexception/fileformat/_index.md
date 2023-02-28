---
title: UnsupportedFileFormatException.FileFormat
second_title: Aspose.Note für .NET-API-Referenz
description: UnsupportedFileFormatException eigendom. Ruft das Dateiformat der übergebenen Daten ab falls erkannt.
type: docs
weight: 10
url: /de/net/aspose.note/unsupportedfileformatexception/fileformat/
---
## UnsupportedFileFormatException.FileFormat property

Ruft das Dateiformat der übergebenen Daten ab, falls erkannt.

```csharp
public FileFormat FileFormat { get; }
```

### Beispiele

Zeigt, wie überprüft wird, ob das Laden eines Dokuments fehlgeschlagen ist, weil das OneNote 2007-Format nicht unterstützt wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
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

### Siehe auch

* enum [FileFormat](../../fileformat/)
* class [UnsupportedFileFormatException](../)
* namensraum [Aspose.Note](../../unsupportedfileformatexception/)
* Montage [Aspose.Note](../../../)


