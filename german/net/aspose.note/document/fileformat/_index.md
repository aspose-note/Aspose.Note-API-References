---
title: Document.FileFormat
second_title: Aspose.Note für .NET-API-Referenz
description: Document eigendom. Ruft das Dateiformat ab OneNote 2010 OneNote Online.
type: docs
weight: 60
url: /de/net/aspose.note/document/fileformat/
---
## Document.FileFormat property

Ruft das Dateiformat ab (OneNote 2010, OneNote Online).

```csharp
public FileFormat FileFormat { get; }
```

### Beispiele

Zeigt, wie man das Dateiformat eines Dokuments erhält.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // OneNote 2010 verarbeiten
        break;
    case FileFormat.OneNoteOnline:
        // OneNote online verarbeiten
        break;
}
```

### Siehe auch

* enum [FileFormat](../../fileformat/)
* class [Document](../)
* namensraum [Aspose.Note](../../document/)
* Montage [Aspose.Note](../../../)


