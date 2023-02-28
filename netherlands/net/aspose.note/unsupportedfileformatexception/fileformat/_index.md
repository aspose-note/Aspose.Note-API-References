---
title: UnsupportedFileFormatException.FileFormat
second_title: Aspose.Note voor .NET API-referentie
description: UnsupportedFileFormatException eigendom. Haalt het bestandsformaat op van doorgegeven gegevens indien gedetecteerd.
type: docs
weight: 10
url: /nl/net/aspose.note/unsupportedfileformatexception/fileformat/
---
## UnsupportedFileFormatException.FileFormat property

Haalt het bestandsformaat op van doorgegeven gegevens indien gedetecteerd.

```csharp
public FileFormat FileFormat { get; }
```

### Voorbeelden

Laat zien hoe u kunt controleren of het laden van een document is mislukt omdat de OneNote 2007-indeling niet wordt ondersteund.

```csharp
// Het pad naar de documentenmap.
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

### Zie ook

* enum [FileFormat](../../fileformat/)
* class [UnsupportedFileFormatException](../)
* naamruimte [Aspose.Note](../../unsupportedfileformatexception/)
* montage [Aspose.Note](../../../)


