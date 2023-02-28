---
title: Page.GetChildNodes
second_title: Aspose.Note per .NET API Reference
description: Page metodo. Ottieni tutti i nodi figli della pagina in base al tipo di nodo.
type: docs
weight: 150
url: /it/net/aspose.note/page/getchildnodes/
---
## Page.GetChildNodes&lt;T1&gt; method

Ottieni tutti i nodi figli della pagina in base al tipo di nodo.

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

Mostra come ottenere tutto il testo dal documento.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Text();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Recupera il testo
string text = string.Join(Environment.NewLine, oneFile.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;

// Stampa il testo sullo schermo di output
Console.WriteLine(text);
```

Mostra come ottenere tutto il testo dalla pagina.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Text();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Ottieni l'elenco dei nodi della pagina
var page = oneFile.GetChildNodes<Page>().FirstOrDefault();

if (page != null)
{
    // Recupera il testo
    string text = string.Join(Environment.NewLine, page.GetChildNodes<RichText>().Select(e => e.Text)) + Environment.NewLine;
    // Stampa il testo sullo schermo di output
    Console.WriteLine(text);
}
```

Mostra come scorrere tutte le pagine e fare una sostituzione nel testo.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("Some task here", "New Text Here");

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Ottieni tutti i nodi RichText
IList<RichText> textNodes = oneFile.GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Sostituisci il testo di una forma
        richText.Replace(kvp.Key, kvp.Value);
    }
}

dataDir = dataDir + "ReplaceTextOnAllPages_out.pdf";

// Salva in qualsiasi formato di file supportato
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Mostra come passare attraverso il testo della pagina ed effettuare una sostituzione.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// Ottieni tutti i nodi RichText
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Sostituisci il testo di una forma
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// Salva in qualsiasi formato di file supportato
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

### Guarda anche

* interface [INode](../../inode/)
* class [Page](../)
* spazio dei nomi [Aspose.Note](../../page/)
* assemblea [Aspose.Note](../../../)


