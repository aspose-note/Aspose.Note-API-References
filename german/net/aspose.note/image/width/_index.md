---
title: Image.Width
second_title: Aspose.Note für .NET-API-Referenz
description: Image eigendom. Holt oder setzt die Breite. Dies ist die tatsächliche Breite des Bilds im MS OneNoteDokument.
type: docs
weight: 180
url: /de/net/aspose.note/image/width/
---
## Image.Width property

Holt oder setzt die Breite. Dies ist die tatsächliche Breite des Bilds im MS OneNote-Dokument.

```csharp
public float Width { get; set; }
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

Zeigt, wie ein Bild aus einer Datei zu einem Dokument mit benutzerdefinierten Eigenschaften hinzugefügt wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Images();

// Dokument aus dem Stream laden.
Document doc = new Document(dataDir + "Aspose.one");

// Holen Sie sich die erste Seite des Dokuments.
Aspose.Note.Page page = doc.FirstChild;

// Laden Sie ein Bild aus der Datei.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Ändern Sie die Größe des Bildes nach Ihren Bedürfnissen (optional).
                              Width = 100,
                              Height = 100,

                              // Legen Sie die Position des Bildes auf der Seite fest (optional).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Bildausrichtung festlegen
                              Alignment = HorizontalAlignment.Right
                          };

// Bild zur Seite hinzufügen.
page.AppendChildLast(image);
```

### Siehe auch

* class [Image](../)
* namensraum [Aspose.Note](../../image/)
* Montage [Aspose.Note](../../../)


