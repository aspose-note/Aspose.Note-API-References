---
title: Page.IsConflictPage
second_title: Aspose.Note para la referencia de la API de .NET
description: Page propiedad. Obtiene o establece un valor que indica si esta página es una página en conflicto.
type: docs
weight: 50
url: /es/net/aspose.note/page/isconflictpage/
---
## Page.IsConflictPage property

Obtiene o establece un valor que indica si esta página es una página en conflicto.

```csharp
public bool IsConflictPage { get; set; }
```

### Observaciones

La página de conflicto surge cuando dos usuarios intentan actualizar el mismo contenido. En este caso, los cambios del primer usuario se escriben como de costumbre. Pero los cambios de otro usuario no se pueden fusionar. Así que solo se crea una copia de la página y marcado como conflicto.

En esta versión, los conflictos se resuelven a favor de los cambios del primer usuario. Entonces, si el documento tiene páginas en conflicto, se mostrarán en el historial pero se omitirán al guardar. Es posible restablecer este indicador para guardar estas páginas en la historia como los de siempre.

Puede encontrar una muestra detallada de la página de manipulación por conflicto en la documentación en línea.

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

* class [Page](../)
* espacio de nombres [Aspose.Note](../../page/)
* asamblea [Aspose.Note](../../../)


