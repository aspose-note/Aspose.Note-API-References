---
title: Page.Clone
second_title: Aspose.Note per .NET API Reference
description: Page metodo. Clona la pagina.
type: docs
weight: 140
url: /it/net/aspose.note/page/clone/
---
## Page.Clone method

Clona la pagina.

```csharp
public Page Clone(bool cloneHistory = false)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cloneHistory | Boolean | Specifica se la cronologia della pagina deve essere clonata.. |

### Valore di ritorno

Un clone della pagina.

### Esempi

Mostra come inserire la versione corrente di una pagina nella cronologia.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Pages();

// Carica il documento OneNote e ottieni il primo figlio           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.Add(page.Clone());

document.Save(dataDir + "PushCurrentPageVersion_out.one");
```

Mostra come clonare una pagina.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_Pages();

// Carica il documento OneNote
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Clona in un nuovo documento senza cronologia
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// Clona in un nuovo documento con cronologia
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

### Guarda anche

* class [Page](../)
* spazio dei nomi [Aspose.Note](../../page/)
* assemblea [Aspose.Note](../../../)


