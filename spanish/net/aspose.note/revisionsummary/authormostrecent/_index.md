---
title: RevisionSummary.AuthorMostRecent
second_title: Aspose.Note para la referencia de la API de .NET
description: RevisionSummary propiedad. Obtiene o establece el autor más reciente.
type: docs
weight: 20
url: /es/net/aspose.note/revisionsummary/authormostrecent/
---
## RevisionSummary.AuthorMostRecent property

Obtiene o establece el autor más reciente.

```csharp
public string AuthorMostRecent { get; set; }
```

### Ejemplos

Muestra cómo editar la metainformación de la página.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Pages();

// Cargue el documento de OneNote y obtenga el primer hijo           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

// Lectura del resumen de la revisión del contenido de esta página
var pageRevisionInfo = page.PageContentRevisionSummary;

Console.WriteLine(string.Format(
    "Author:\t{0}\nModified:\t{1}",
    pageRevisionInfo.AuthorMostRecent,
    pageRevisionInfo.LastModifiedTime.ToString("dd.MM.yyyy HH:mm:ss")));

// Actualizar resumen de revisión de página para esta página
pageRevisionInfo.AuthorMostRecent = "New Author";
pageRevisionInfo.LastModifiedTime = DateTime.Now;

document.Save(dataDir + "WorkingWithPageRevisions_out.one");
```

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

* class [RevisionSummary](../)
* espacio de nombres [Aspose.Note](../../revisionsummary/)
* asamblea [Aspose.Note](../../../)


