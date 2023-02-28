---
title: AttachedFile.Bytes
second_title: Aspose.Note für .NET-API-Referenz
description: AttachedFile eigendom. Ruft die Binärdaten für eine eingebettete Datei ab.
type: docs
weight: 50
url: /de/net/aspose.note/attachedfile/bytes/
---
## AttachedFile.Bytes property

Ruft die Binärdaten für eine eingebettete Datei ab.

```csharp
public byte[] Bytes { get; }
```

### Beispiele

Zeigt, wie der Inhalt einer angehängten Datei abgerufen wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Attachments();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// Holen Sie sich eine Liste der angehängten Dateiknoten
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Durch alle Knoten iterieren
foreach (AttachedFile file in nodes)
{
    // Angehängte Datei in ein Stream-Objekt laden
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Erstellen Sie eine lokale Datei
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Dateistream kopieren
            CopyStream(outputStream, fileStream);
        }
    }
}
```

### Siehe auch

* class [AttachedFile](../)
* namensraum [Aspose.Note](../../attachedfile/)
* Montage [Aspose.Note](../../../)


