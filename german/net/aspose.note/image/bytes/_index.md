---
title: Image.Bytes
second_title: Aspose.Note für .NET-API-Referenz
description: Image eigendom. Ruft den Bilddatenspeicher ab.
type: docs
weight: 50
url: /de/net/aspose.note/image/bytes/
---
## Image.Bytes property

Ruft den Bilddatenspeicher ab.

```csharp
public byte[] Bytes { get; }
```

### Beispiele

Zeigt, wie ein Bild aus einem Dokument abgerufen wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Images();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Alle Image-Knoten abrufen
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Bildbytes in einer Datei speichern
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

### Siehe auch

* class [Image](../)
* namensraum [Aspose.Note](../../image/)
* Montage [Aspose.Note](../../../)


