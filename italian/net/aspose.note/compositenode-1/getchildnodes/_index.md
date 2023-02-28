---
title: CompositeNode1.GetChildNodes
second_title: Aspose.Note per .NET API Reference
description: CompositeNode metodo. Ottieni tutti i nodi figli in base al tipo di nodo.
type: docs
weight: 70
url: /it/net/aspose.note/compositenode-1/getchildnodes/
---
## CompositeNode&lt;T&gt;.GetChildNodes&lt;T1&gt; method

Ottieni tutti i nodi figli in base al tipo di nodo.

```csharp
public override List<T1> GetChildNodes<T1>()
    where T1 : class, INode
```

| Parametro | Descrizione |
| --- | --- |
| T1 | Il tipo di elementi nell'elenco restituito. |

### Valore di ritorno

Un elenco di nodi figlio.

### Esempi

Mostra come ottenere un'immagine da un documento.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Images();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Ottieni tutti i nodi Immagine
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Salva i byte dell'immagine in un file
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

Mostra come ottenere le meta informazioni dell'immagine.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Images();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Ottieni tutti i nodi Immagine
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

### Guarda anche

* interface [INode](../../inode/)
* class [CompositeNode&lt;T&gt;](../)
* spazio dei nomi [Aspose.Note](../../compositenode-1/)
* assemblea [Aspose.Note](../../../)


