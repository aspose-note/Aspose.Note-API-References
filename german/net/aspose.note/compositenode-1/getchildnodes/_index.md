---
title: CompositeNode1.GetChildNodes
second_title: Aspose.Note für .NET-API-Referenz
description: CompositeNode methode. Alle untergeordneten Knoten nach Knotentyp abrufen.
type: docs
weight: 70
url: /de/net/aspose.note/compositenode-1/getchildnodes/
---
## CompositeNode&lt;T&gt;.GetChildNodes&lt;T1&gt; method

Alle untergeordneten Knoten nach Knotentyp abrufen.

```csharp
public override List<T1> GetChildNodes<T1>()
    where T1 : class, INode
```

| Parameter | Beschreibung |
| --- | --- |
| T1 | Der Typ der Elemente in der zurückgegebenen Liste. |

### Rückgabewert

Eine Liste von untergeordneten Knoten.

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

* interface [INode](../../inode/)
* class [CompositeNode&lt;T&gt;](../)
* namensraum [Aspose.Note](../../compositenode-1/)
* Montage [Aspose.Note](../../../)


