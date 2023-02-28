---
title: Document.FileFormat
second_title: Aspose.Note voor .NET API-referentie
description: Document eigendom. Krijgt bestandsindeling OneNote 2010 OneNote Online.
type: docs
weight: 60
url: /nl/net/aspose.note/document/fileformat/
---
## Document.FileFormat property

Krijgt bestandsindeling (OneNote 2010, OneNote Online).

```csharp
public FileFormat FileFormat { get; }
```

### Voorbeelden

Laat zien hoe u de bestandsindeling van een document kunt krijgen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // Verwerk OneNote 2010
        break;
    case FileFormat.OneNoteOnline:
        // Verwerk OneNote online
        break;
}
```

### Zie ook

* enum [FileFormat](../../fileformat/)
* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)


