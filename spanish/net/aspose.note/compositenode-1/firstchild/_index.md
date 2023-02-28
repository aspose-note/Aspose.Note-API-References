---
title: CompositeNode1.FirstChild
second_title: Aspose.Note para la referencia de la API de .NET
description: CompositeNode propiedad. Obtiene el primer nodo secundario de este nodo.
type: docs
weight: 10
url: /es/net/aspose.note/compositenode-1/firstchild/
---
## CompositeNode&lt;T&gt;.FirstChild property

Obtiene el primer nodo secundario de este nodo.

```csharp
public T FirstChild { get; }
```

### Ejemplos

Muestra cómo verificar si una página es una página en conflicto (es decir, tiene cambios que OneNote no pudo fusionar automáticamente).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// Cargar documento de OneNote
Document doc = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

var history = doc.GetPageHistory(doc.FirstChild);
for (int i = 0; i < history.Count; i++)
{
    var historyPage = history[i];
    Console.Write("    {0}. Author: {1}, {2:dd.MM.yyyy hh.mm.ss}",
                    i,
                    historyPage.PageContentRevisionSummary.AuthorMostRecent,
                    historyPage.PageContentRevisionSummary.LastModifiedTime);
    Console.WriteLine(historyPage.IsConflictPage ? ", IsConflict: true" : string.Empty);

    // Por defecto, las páginas de conflicto simplemente se omiten al guardar.
    // Si lo marca como sin conflicto, se guardará como de costumbre en el historial.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### Ver también

* class [CompositeNode&lt;T&gt;](../)
* espacio de nombres [Aspose.Note](../../compositenode-1/)
* asamblea [Aspose.Note](../../../)


