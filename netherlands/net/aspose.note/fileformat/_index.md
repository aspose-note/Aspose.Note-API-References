---
title: Enum FileFormat
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.FileFormat opsomming. Vertegenwoordigt OneNotebestandsindeling.
type: docs
weight: 90
url: /nl/net/aspose.note/fileformat/
---
## FileFormat enumeration

Vertegenwoordigt OneNote-bestandsindeling.

```csharp
public enum FileFormat
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Unknown | `0` | Onbekend bestandsformaat. |
| OneNote2007 | `1` | OneNote 2010. |
| OneNote2010 | `2` | OneNote 2010. |
| OneNoteOnline | `3` | OneNote online. |

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


