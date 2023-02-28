---
title: Image.Alignment
second_title: Aspose.Note für .NET-API-Referenz
description: Image eigendom. Ruft die Ausrichtung ab oder legt sie fest.
type: docs
weight: 20
url: /de/net/aspose.note/image/alignment/
---
## Image.Alignment property

Ruft die Ausrichtung ab oder legt sie fest.

```csharp
public HorizontalAlignment Alignment { get; set; }
```

### Beispiele

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

Zeigt, wie ein Bild aus einem Stream zu einem Dokument hinzugefügt wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Images();

// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Document();

// Seitenklassenobjekt initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Laden Sie das zweite Bild unter Verwendung des Bildnamens, der Erweiterung und des Streams.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Bildausrichtung festlegen
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Zeigt, wie Sie einem Dokument ein Bild aus einer Datei hinzufügen.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Images();

// Erstellen Sie ein Objekt der Document-Klasse
Document doc = new Document();

// Seitenklassenobjekt initialisieren
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Outline-Klassenobjekt initialisieren und Offset-Eigenschaften festlegen
Outline outline = new Outline(doc);

// OutlineElement-Klassenobjekt initialisieren
OutlineElement outlineElem = new OutlineElement(doc);

// Laden Sie ein Bild über den Dateipfad.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Bildausrichtung festlegen
                              Alignment = HorizontalAlignment.Right
                          };

// Bild hinzufügen
outlineElem.AppendChildLast(image);

// Gliederungselemente hinzufügen
outline.AppendChildLast(outlineElem);

// Outline-Knoten hinzufügen
page.AppendChildLast(outline);

// Seitenknoten hinzufügen
doc.AppendChildLast(page);

// OneNote-Dokument speichern
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

### Siehe auch

* enum [HorizontalAlignment](../../horizontalalignment/)
* class [Image](../)
* namensraum [Aspose.Note](../../image/)
* Montage [Aspose.Note](../../../)


