---
title: AttachedFile.Bytes
second_title: Aspose.Note voor .NET API-referentie
description: AttachedFile eigendom. Haalt de binaire gegevens op voor een ingesloten bestand.
type: docs
weight: 50
url: /nl/net/aspose.note/attachedfile/bytes/
---
## AttachedFile.Bytes property

Haalt de binaire gegevens op voor een ingesloten bestand.

```csharp
public byte[] Bytes { get; }
```

### Voorbeelden

Laat zien hoe u de inhoud van een bijgevoegd bestand kunt ophalen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Attachments();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// Krijg een lijst met bijgevoegde bestandsknooppunten
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Doorloop alle knooppunten
foreach (AttachedFile file in nodes)
{
    // Laad bijgevoegd bestand naar een streamobject
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Maak een lokaal bestand
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Bestandsstroom kopiëren
            CopyStream(outputStream, fileStream);
        }
    }
}
```

### Zie ook

* class [AttachedFile](../)
* naamruimte [Aspose.Note](../../attachedfile/)
* montage [Aspose.Note](../../../)


