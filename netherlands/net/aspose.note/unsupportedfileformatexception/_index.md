---
title: Class UnsupportedFileFormatException
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.UnsupportedFileFormatException klas. Wordt gegenereerd tijdens het laden van documenten wanneer de bestandsindeling niet wordt herkend of niet wordt ondersteund door Aspose.Note.
type: docs
weight: 990
url: /nl/net/aspose.note/unsupportedfileformatexception/
---
## UnsupportedFileFormatException class

Wordt gegenereerd tijdens het laden van documenten, wanneer de bestandsindeling niet wordt herkend of niet wordt ondersteund door Aspose.Note.

```csharp
public class UnsupportedFileFormatException : Exception
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [FileFormat](../../aspose.note/unsupportedfileformatexception/fileformat/) { get; } | Haalt het bestandsformaat op van doorgegeven gegevens indien gedetecteerd. |

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

* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


