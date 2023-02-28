---
title: Image.OriginalWidth
second_title: Aspose.Note für .NET-API-Referenz
description: Image eigendom. Ruft die ursprüngliche Breite ab. Dies ist die ursprüngliche Breite des Bildes vor der Größenänderung.
type: docs
weight: 150
url: /de/net/aspose.note/image/originalwidth/
---
## Image.OriginalWidth property

Ruft die ursprüngliche Breite ab. Dies ist die ursprüngliche Breite des Bildes vor der Größenänderung.

```csharp
public float OriginalWidth { get; }
```

### Beispiele

Zeigt, wie die Metainformationen des Bildes abgerufen werden.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Images();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Alle Image-Knoten abrufen
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

### Siehe auch

* class [Image](../)
* namensraum [Aspose.Note](../../image/)
* Montage [Aspose.Note](../../../)


