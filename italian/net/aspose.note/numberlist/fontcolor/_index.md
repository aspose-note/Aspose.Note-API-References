---
title: NumberList.FontColor
second_title: Aspose.Note per .NET API Reference
description: NumberList proprietà. Ottiene o imposta il colore del carattere.
type: docs
weight: 30
url: /it/net/aspose.note/numberlist/fontcolor/
---
## NumberList.FontColor property

Ottiene o imposta il colore del carattere.

```csharp
public Color FontColor { get; set; }
```

### Esempi

Mostra come recuperare informazioni sulla formattazione dell'elenco.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// Recupera i nodi di una raccolta dell'elemento di contorno
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// Itera attraverso ogni nodo
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // Recupera il nome del carattere
        Console.WriteLine("Font Name: " + list.Font);

        // Recupera la lunghezza del carattere
        Console.WriteLine("Font Length: " + list.Font.Length);

        // Recupera la dimensione del carattere
        Console.WriteLine("Font Size: " + list.FontSize);

        // Recupera il colore del carattere
        Console.WriteLine("Font Color: " + list.FontColor);

        // Recupera il formato
        Console.WriteLine("Font format: " + list.Format);

        // Seleziona il grassetto
        Console.WriteLine("Is bold: " + list.IsBold);

        // Controlla il corsivo
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

### Guarda anche

* class [NumberList](../)
* spazio dei nomi [Aspose.Note](../../numberlist/)
* assemblea [Aspose.Note](../../../)


