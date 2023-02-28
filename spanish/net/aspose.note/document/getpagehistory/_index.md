---
title: Document.GetPageHistory
second_title: Aspose.Note para la referencia de la API de .NET
description: Document método. Obtiene elPageHistory que contiene el historial completo de cada página presentada en un documento la más antigua en el índice 0. Se puede acceder a la revisión de la página actual comoCurrent y contenido por separado de la colección de versiones históricas.
type: docs
weight: 100
url: /es/net/aspose.note/document/getpagehistory/
---
## Document.GetPageHistory method

Obtiene el[`PageHistory`](../../pagehistory/) que contiene el historial completo de cada página presentada en un documento (la más antigua en el índice 0). Se puede acceder a la revisión de la página actual como[`Current`](../../pagehistory/current/) y contenido por separado de la colección de versiones históricas.

```csharp
public PageHistory GetPageHistory(Page page)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| page | Page | La revisión actual de una página. |

### Valor_devuelto

El[`PageHistory`](../../pagehistory/) .

### Ejemplos

Muestra cómo restaurar la versión anterior de una página.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Pages();

// Cargue el documento de OneNote y obtenga el primer hijo           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

Muestra cómo editar el historial de la página.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Pages();

// Cargue el documento de OneNote y obtenga el primer hijo           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
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

* class [PageHistory](../../pagehistory/)
* class [Page](../../page/)
* class [Document](../)
* espacio de nombres [Aspose.Note](../../document/)
* asamblea [Aspose.Note](../../../)


