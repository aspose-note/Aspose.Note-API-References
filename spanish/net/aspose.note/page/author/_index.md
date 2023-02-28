---
title: Page.Author
second_title: Aspose.Note para la referencia de la API de .NET
description: Page propiedad. Obtiene o establece el autor.
type: docs
weight: 20
url: /es/net/aspose.note/page/author/
---
## Page.Author property

Obtiene o establece el autor.

```csharp
public string Author { get; set; }
```

### Ejemplos

Muestra cómo obtener metainformación sobre una página.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Pages();

// Cargue el documento en Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

foreach (Page page in oneFile)
{
    Console.WriteLine("LastModifiedTime: {0}", page.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", page.CreationTime);
    Console.WriteLine("Title: {0}", page.Title);
    Console.WriteLine("Level: {0}", page.Level);
    Console.WriteLine("Author: {0}", page.Author);
    Console.WriteLine();
}
```

Muestra cómo obtener el historial de la página.

```csharp
// La ruta al directorio de documentos.
string dataDir = RunExamples.GetDataDir_Pages();

// Cargar documento de OneNote
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Obtener la primera página
Page firstPage = document.FirstChild;
foreach (Page pageRevision in document.GetPageHistory(firstPage))
{
    /*Use pageRevision like a regular page.*/
    Console.WriteLine("LastModifiedTime: {0}", pageRevision.LastModifiedTime);
    Console.WriteLine("CreationTime: {0}", pageRevision.CreationTime);
    Console.WriteLine("Title: {0}", pageRevision.Title);
    Console.WriteLine("Level: {0}", pageRevision.Level);
    Console.WriteLine("Author: {0}", pageRevision.Author);
    Console.WriteLine();
}
```

### Ver también

* class [Page](../)
* espacio de nombres [Aspose.Note](../../page/)
* asamblea [Aspose.Note](../../../)


